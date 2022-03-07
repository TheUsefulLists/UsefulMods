# Java arguments optimization
Java arguments that you can change to potentially get better performance.

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.<br><br>

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

<hr>

## Changing Java Arguments
Here's how to change your java arguments in the official Minecraft Launcher. 
1. Open the Minecraft Launcher, click on 'Installations', click on your profile and click on 'More Options'.
2. Under 'More Options', you will find 'JVM arguments'.
3. You can change or add your JVM arguments here.

<hr>

## Aikar's flags

These flags are made by Aikar and you can find the explanation for the flags
[here](https://aikar.co/mcflags.html).

Use these flags exactly, only changing Xmx and Xms. These flags work and scale accordingly to any size of memory.

``` 
java -Xms10G -Xmx10G -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true -jar paperclip.jar nogui 
```

If you want to make your own custom flags that suit your PC and your needs, keep reading.

<hr>

## Memory

``` -Xms<int> -Xmx<int> ```

Replace int with a value. For example: -Xmx<2G>, -Xms<512M>
Append the letter k or K to indicate kilobytes, m or M to indicate megabytes, g or G to indicate gigabytes

- ### Xms
    Sets the minimum and the initial size of the heap. It is best to set Xms equal to Xmx (the maximum heap size) to minimize garbage collections.

- ### Xmx
    Sets the maximum size of the heap. Setting it to higher amounts reduces the frequency of garbage collections but causes larger lag spikes when the garbage collector runs. It is best to set this value to about half of the memory available on your system. Allocating any more than that will slow down your system and is not recommended.

<hr>

## Changing your Java Virtual Machine (JVM)
There are many JVMs, out of which the most popular are HotSpot and OpenJ9. HotSpot is the open-source JVM implementation by Oracle while OpenJ9 is a high performance, scalable, JVM implementation by Eclipse Foundation. OpenJ9 tends to perform better under most conditions. Here are some of the reasons why OpenJ9 is better than HotSpot -
- 51% faster startup time
- 50% smaller footprint after startup
- 33% smaller footprint during load
 
However, the official Minecraft launcher and most other launchers use HotSpot. If you want to use OpenJ9 JVM, then follow these instructions:
1. Click [here](https://developer.ibm.com/languages/java/semeru-runtimes/downloads).
2. Choose your operating system and architechture.
3. Chose Java 17 for Minecraft versions 1.17+ and Java 8 for 1.16 and below.
4. Download the tar/zip file and extract it.
5. Open the Minecraft Launcher, click on 'Installations', click on your profile and click on 'More Options'.
6. Under 'Java Executable', click on 'Browse'. Then, find the location of the runtime you extracted. Open the 'bin' folder and select the 'javaw.exe' executable.
7. Click on 'Save'.

You will find the important arguments for both HotSpot and OpenJ9 below.  


<hr>

## HotSpot JVM arguments:

- ## Garbage Collectors
    There are many garbage collectors, out of which the Parallel collector, G1 garbage collector, Z garbage collector and Shenandoah garbage collector are best-suited for Minecraft.

    - ### Parallel Garbage Collector
        The parallel collector (also known as the throughput collector) performs minor collections in parallel, which can significantly reduce garbage collection overhead.
        <br> The parallel collector can be enabled with the option ```-XX:+UseParallelGC```. It is best suited for systems with few threads.

    - ### Garbage-First Garbage Collector
        The Garbage-First (G1) garbage collector attempts to meet garbage collection (GC) pause time goals with high probability while achieving high throughput.
        <br> The Garbage-First (G1) garbage collector is enabled using the command-line option ```-XX:+UseG1GC```. It is used by default in most launchers including the official one.

    - ### Z Garbage Collector
        The Z Garbage Collector, also known as ZGC, is a scalable low latency garbage collector designed to meet sub-millisecond max pause times, pause times that do not increase with the heap size and to handle heaps ranging from 8MB to 16TB in size.
        <br> The Z Garbage Collector is enabled using the command-line option ```-XX:+UseZGC```. It isn’t supported in Java 8, so only use it for Minecraft versions 1.17 and above.

    - ### Shenandoah Garbage Collector
        Shenandoah is the low pause time garbage collector that reduces GC pause times by performing more garbage collection work concurrently with the running Java program. Garbage collecting a 200 GB heap, or a 2 GB heap should have the similar low pause behaviour. 
        <br> The Shenandoah GC is enabled using the command-line option ```-XX:+UseShenandoahGC```. It does not ship in Oracle JDK builds, so you will have to use other vendors for your JDK builds like AdoptOpenJDK and Azul.

    <br> For me the Shenandoah GC works best but I would recommend that you try all of them and see which works best on your system.

<hr>

## OpenJ9 JVM arguments:

- ## GC Policies
    There are 6 GC policies - gencon, balanced, optavgpause, optthruput, metronome and nogc. Out of these, the gencon and balanced policies are best-suited for Minecraft.

    - ### gencon (default)
        This policy aims to minimize GC pause times without compromising throughput. This policy breaks the Java heap into a nursery and a tenured space. All objects are allocated initially into the nursery. If an object survives a certain number of collections while in the nursery, it will be moved into the tenured space, which is only collected when it is full.
        <br> The gencon policy is enabled with the command-line option ```-Xgcpolicy:gencon```. However, you don't need to specify it since it is the default policy.

    - ### balanced
        This policy divides the heap into a number of regions (1,000 - 2,000), each of which is individually managed and garbage-collected.
        <br> The balanced policy is enabled with the command-line option ```-Xgcpolicy:balanced```.

    <br> The default policy (gencon) is ideal for Minecraft versions 1.12 and below. However, for versions 1.13 and above, you should use the balanced policy as the gencon policy causes increased strain on the garbage collector subsystem.


- ## Nursery size

    This only applies if you are using the default GC policy (gencon).

    ``` -Xmns<int> -Xmnx<int>```
    
    Replace int with a value. For example: -Xmnx<2G>, -Xmns<512M>.
    Append the letter k or K to indicate kilobytes, m or M to indicate megabytes, g or G to indicate gigabytes

    - ### Xmns
        Sets the minimum size of the nursery. The default value is 25% of -Xms and that is a good value that doesn't need any changing.

    - ### Xmnx
        Sets the maximum size of the nursery. The default value is 25% of -Xmx and since -Xmx is equal to -Xms the nursery will never grow. Minecraft creates a lot of short-lived objects, so it is better to set this to a larger value like 50% of -Xmx.

<hr>

These are probably the only JVM arguments you will ever need to change. Be careful when messing around with JVM arguments as making some changes could cause Minecraft to crash on start-up.

Sources:
<br> [Oracle docs](https://docs.oracle.com/en/)
<br> [OpenJDK Wiki](https://wiki.openjdk.java.net/)
<br> [Eclipse OpenJ9 docs](https://www.eclipse.org/openj9/docs/)

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)
