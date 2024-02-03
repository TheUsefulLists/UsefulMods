# Java arguments optimization

Java arguments that you can change to potentially get better performance.

Any suggestions/complaints?

Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.

[![Bisect Hosting Image](https://raw.githubusercontent.com/TheUsefulLists/assets/main/Images/Promo.png)](https://bisecthosting.com/UsefulLists)
We have partnered with BisectHosting this is an exciting step for us. All money earned from this will go to the staff of UsefulLists, not including myself (Kevsky).

[![Home](https://raw.githubusercontent.com/TheUsefulLists/assets/main/Images/Buttons/Small/Home.png)](/README.md)

## Changing Java Arguments

Here's how to change your Java arguments in the official Minecraft Launcher.

1. Open the Minecraft Launcher, click on 'Installations', click on your profile and click on 'More Options'.
2. Under 'More Options', you will find 'JVM arguments'.
3. You can change or add your JVM arguments here.

**Don't know a lot about Java Args? use this [tool](https://simplymc.art/flags/)**

### Note about Pterodactyl

When running a server on an instance of [Pterodactyl](https://pterodactyl.io) do not set Xms to all of the available memory.
It is recommended when running on Pterodactyl you set Xms 1G to 1.5G less than Xmx to avoid the Out Of Memory Killer (OOMKiller) from terminating your server.

## Aikar's flags

These flags are made by Aikar and you can find the explanation for the flags [here](https://aikar.co/2018/07/02/tuning-the-jvm-g1gc-garbage-collector-flags-for-minecraft/).

Use these flags exactly, only changing Xmx and Xms. These flags work and scale accordingly to any size of memory. See section [More than 12G](#more-than-12g) below for additional large memory optimizations

If you're using these args, and it doesn't work, remove Java from the start. Some require Java at the start, others do not.

If using these flags in a script, for example to start a server. These flags should come before
`-jar someJarFile.jar`

```sh
java -Xms10G -Xmx10G -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true
```

### More than 12G

Aikar Notes if your using a Xmx value greater than 12G add/adjust the following flags. For bigger amount of memory these provide additional optimizations for GC

```sh
-XX:G1NewSizePercent=40
-XX:G1MaxNewSizePercent=50
-XX:G1HeapRegionSize=16M
-XX:G1ReservePercent=15
-XX:InitiatingHeapOccupancyPercent=20
```

## Custom Flags

If you want to make your own custom flags that suit your PC and your needs, keep reading.

We only cover the commonly changed options

### Memory

``` -Xms<int> -Xmx<int> ```

Replace int with a value. For example: -Xmx2G, -Xms512M
Append the letter k or K to indicate kilobytes, m or M to indicate megabytes, g or G to indicate gigabytes

- #### Xms

    Sets the minimum and the initial size of the heap. It is best to set Xms equal to Xmx (the maximum heap size) to minimize garbage collections.

    On Pterodactyl set Xms 1 to 1.5G less than Xmx

- #### Xmx

    Sets the maximum size of the heap. Setting it to higher amounts reduces the frequency of garbage collections but causes larger lag spikes when the garbage collector runs. It is best to set this value to about half of the memory available on your system. Allocating any more than that will slow down your system and is not recommended.

### Changing your Java Virtual Machine (JVM)

There are many JVMs, out of which the most popular are HotSpot and OpenJ9. HotSpot is the open-source JVM implementation by Oracle while OpenJ9 is a JVM implementation by Eclipse Foundation. While HotSpot tends to perform much better than OpenJ9, OpenJ9 only uses about half the memory HotSpot uses. So if you have a small amount of RAM on your system, I would recommend OpenJ9 while if you have plenty of RAM to allocate to Minecraft I would recommend HotSpot. I will be including arguments for both HotSpot and OpenJ9. If you want to use the OpenJ9 JVM, then follow these instructions:

1. Click [here](https://developer.ibm.com/languages/java/semeru-runtimes/downloads).
2. Choose your operating system and architecture.
3. Chose Java 17 for Minecraft versions 1.17+ and Java 8 for 1.16 and below.
4. Download the tar/zip file and extract it.
5. Open the Minecraft Launcher, click on 'Installations', click on your profile and click on 'More Options'.
6. Under 'Java Executable', click on 'Browse'. Then, find the location of the runtime you extracted. Open the 'bin' folder and select the 'javaw.exe' executable.
7. Click on 'Save'.

### HotSpot JVM arguments

- ### Garbage Collection

    There are many garbage collectors, out of which the Shenandoah garbage collector is best-suited for Minecraft.

    It is a low pause time garbage collector that reduces GC pause times by performing more garbage collection work concurrently with the running Java program. Garbage collecting a 200 GB heap, or a 2 GB heap should have the similar low pause behavior when using Shenandoah.
    It is enabled using the command-line option ```-XX:+UseShenandoahGC```. It isn't supported by all vendors, so check if your vendor supports it [here](https://wiki.openjdk.java.net/display/shenandoah/Main).

    The default GC used is G1, but the G1GC can cause pretty big lag spikes when collecting large heaps. For this reason, I would recommend that you use the Shenandoah GC instead of the G1GC. When I tested Shenandoah with 4GB of RAM allocated, there were zero noticeable stutters caused by the GC.

    There is also this option called AlwaysPreTouch (```-XX:+AlwaysPreTouch```) which you should use to improve performance.

### OpenJ9 JVM arguments

- ### GC Policies

    There are 6 GC policies - gencon, balanced, optavgpause, optthruput, metronome and nogc. Out of these, the gencon policy is best-suited for Minecraft. It is similiar in performance to the G1GC in HotSpot.

    This policy breaks the Java heap into a nursery and a tenured space. All objects are initially allocated into the nursery. If an object survives a certain number of collections while in the nursery, it will be moved into the tenured space, which is only collected when it is full.
    The gencon policy is enabled with the command-line option ```-Xgcpolicy:gencon```. However, you don't need to specify it since it is the default policy.

- ### Nursery size

    This only applies if you are using the default GC policy (gencon).

    ``` -Xmns<int> -Xmnx<int> ```

    Replace int with a value. For example: -Xmnx2G, -Xmns512M
    Append the letter k or K to indicate kilobytes, m or M to indicate megabytes, g or G to indicate gigabytes

  - **Xmns**

    Sets the minimum size of the nursery. The default value is 25% of -Xms and that is a good value that doesn't need any changing.

  - **Xmnx**

    Sets the maximum size of the nursery. The default value is 25% of -Xmx and when -Xmx is set to -Xms the nursery will never grow. Minecraft creates a lot of short-lived objects, so it is better to set this to a larger value like 40% of -Xmx.

These are probably the only JVM arguments you will ever need to change. Be careful when messing around with JVM arguments as making some changes could cause Minecraft to crash on start-up.

Sources:

[Oracle docs](https://docs.oracle.com/en/)

[OpenJDK Wiki](https://wiki.openjdk.java.net/)

[Eclipse OpenJ9 docs](https://www.eclipse.org/openj9/docs/)

[![Home](https://raw.githubusercontent.com/TheUsefulLists/assets/main/Images/Buttons/Small/Home.png)](/README.md)
