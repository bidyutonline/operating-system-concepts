# What is process

The process is program in execution. Once we run a program, it turns into process.

It has following memory map -

* **Code Segment** - The code of the process resides here.
* **Data Segment** - The initialized static variables are allocated here.
* **Extra Segment (BSS)** - Unintialized static variables are allocated here.
* **Heap Segment** - Dynamic memory allocation happends from here. It grows from bottom to upwards.
* **Stack Segment** - Local variables are stored here. It grows from top to downwards.


## The process memory map

+---------------------------+
|                           |
|      Stack Segment        |
|                           |
+---------------------------+
|                           |
|      Heap Segment         |
|                           |
+---------------------------+
|                           |
|      BSS (uninitialized)  |
|                           |
+---------------------------+
|                           |
|      Data Segment         |
|                           |
+---------------------------+
|                           |
|      Code Segment         |
|                           |
+---------------------------+