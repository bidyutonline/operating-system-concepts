* **Batch Processing** - Put tasks in punch card and create a batch of job. The operator will put the batch of jobs together. This is a non-premptive method. Once the process starts execution, processor will remain allocated to it until it is finished. Even if the current process is blocked for I/O the processor will not shift to next process.

* **Multiprogramming** - A set of processes will be loaded in primary memory. CPU will pick up processes one after another and execute. This is non-premptive process. Once the process starts execution, processor will remain allocated to it until it is finished. In this case, if the process is blocked for I/O, the CPU will pick up next process.

* **Multitasking/Time Sharing** - Time quantaum, a slice of time, is decided. The CPU picks up every process and executes it upto the time quantum. Once the time quantum is expired, the processor picks up next process and continues. Round robin is one of the example of multitasking system.

* **Multiprocessor** - The system has multiple processor and jobs are scheduled over them.

* **Realtime** - Operating system which are time sensitive. 
    * **Soft Realtime System** - Time critical, but not that fatal if time is missed. Like youtube live streaming service.
    * **Hard Realtime System** - Time critical and is fatal for any missed time. Like missile launch.
    
* **Embedded** - Specific to a system to perform a set of fixed tasks. Like Microwave oven.