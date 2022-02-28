# Java arguments optimization
Java arguments that you can change to potentially get better performance.

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.<br><br>

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

<hr>

## Java Virtual Machines (JVMs)
There are many JVMs, out of which the most popular are HotSpot and OpenJ9. HotSpot is the open-source JVM implementation by Oracle. OpenJ9 is a high performance, scalable, JVM implementation by Eclipse Foundation. OpenJ9 tends to perform better under most conditions. Here are some of the reasons why OpenJ9 is better than HotSpot -
- 51% faster startup time
    By using shared classes cache and AOT technology, OpenJ9 starts in roughly half the time it takes HotSpot.
- 50% smaller footprint after startup
- 33% smaller footprint during load
    Consistent with the footprint results after startup, the OpenJ9 footprint remains much smaller than HotSpot when load is applied.
 
You will find the important arguments for both of them below.  

<hr>

## HotSpot JVM arguments:
- ## Memory

    ``` -Xms<int> -Xmx<int> ```

    Replace int with a value. For example: -Xmx<2G>, -Xms<512M>
    Append the letter k or K to indicate kilobytes, m or M to indicate megabytes, g or G to indicate gigabytes

    - ### Xms
        Sets the minimum and the initial size of the heap. It is best to set Xms equal to Xmx (the maximum heap size) to minimize potentially costly heap reallocations.

    - ### Xmx
        Sets the maximum size of the heap. Setting it to higher amounts reduces the frequency of garbage collections but causes larger lag spikes when the garbage collector runs. It is best to set this value to about half of the memory available on your system. Allocating any more memory than half will probably slow down your system significantly and may even result in your system crashing.


- ## Garbage Collectors

    - ### Serial Garbage Collector
        The serial collector uses a single thread to perform all garbage collection work, which makes it relatively efficient because there is no communication overhead between threads. It is best-suited to single processor machines, because it cannot take advantage of multiprocessor hardware, although it can be useful on multiprocessors for applications with small data sets (up to approximately 100 MB). 
        <br> The serial collector can be enabled with the option ```-XX:+UseSerialGC```.

    - ### Parallel Garbage Collector
        The parallel collector (also known as the throughput collector) performs minor collections in parallel, which can significantly reduce garbage collection overhead. It is intended for applications with medium-sized to large-sized data sets that are run on multiprocessor or multithreaded hardware. 
        <br> The parallel collector can be enabled with the option ```-XX:+UseParallelGC```.

    ### Mostly Concurrent Garbage Collectors
    The mostly concurrent collectors perform most of their work concurrently (for example, while the application is still running) to keep garbage collection pauses short.

    - #### Concurrent Mark Sweep Collector
        The Concurrent Mark Sweep (CMS) collector is designed for applications that prefer shorter garbage collection pauses and that can afford to share processor resources with the garbage collector while the application is running. Typically applications that have a relatively large set of long-lived data and run on machines with two or more processors tend to benefit from the use of this collector. However, this collector should be considered for any application with a low pause time requirement. 
        <br> The CMS collector is enabled with the command-line option ```-XX:+UseConcMarkSweepGC```.

    - #### Garbage-First Garbage Collector
        The Garbage-First (G1) garbage collector is a server-style garbage collector, targeted for multiprocessor machines with large memories. It attempts to meet garbage collection (GC) pause time goals with high probability while achieving high throughput.
        <br> The Garbage-First (G1) garbage collector is enabled using the command-line option ```-XX:+UseG1GC```. It is used by default in most launchers including the official one.

    - #### Z Garbage Collector
        The Z Garbage Collector, also known as ZGC, is a scalable low latency garbage collector designed to meet sub-millisecond max pause times, pause times that do not increase with the heap size and to handle heaps ranging from 8MB to 16TB in size.
        <br> The Z Garbage Collector is enabled using the command-line option ```-XX:+UseZGC```. It isn’t supported in Java 8, so only use it for Minecraft versions 1.17 and above.

    - #### Shenandoah Garbage Collector
        Shenandoah is the low pause time garbage collector that reduces GC pause times by performing more garbage collection work concurrently with the running Java program. Shenandoah does the bulk of GC work concurrently, including the concurrent compaction, which means its pause times are no longer directly proportional to the size of the heap. Garbage collecting a 200 GB heap, or a 2 GB heap should have the similar low pause behaviour. 
        <br> The Shenandoah GC is enabled using the command-line option ```-XX:+UseShenandoahGC```. It does not ship in Oracle JDK builds, so you will have to use other vendors for your JDK builds like AdoptOpenJDK and Azul.

<br> For me the Shenandoah GC works best but I would recommend that you try all of them and see which works best on your system. Ideally, the ZGC should work best as it offers the highest throughput and the smallest pauses.

<hr>

## OpenJ9 JVM arguments:
- WIP

<hr>

These are probably the only JVM arguments you will ever need to change. Be careful when messing around with JVM arguments as making some changes could cause Minecraft to crash on start-up.

Sources:
<br> [Oracle docs](https://docs.oracle.com/en/)
<br> [OpenJDK Wiki](https://wiki.openjdk.java.net/)
<br> [Eclipse OpenJ9](https://www.eclipse.org/openj9/docs/)

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)
