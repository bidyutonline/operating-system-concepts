# Process States

A process goes through following states in its lifetime.

## State Diagram
<img src="../images/Process States.png"/>

## States

* **New** - When a process is created its in new state. This is the default state of a process.
* **Ready** - When a process is up for execution, it is put into ready queue. This task is done by **long term scheduler**.
* **Running** - Depending on the scheduling algorithm, the processor picks up process and the process enters into running state. The scheduling is done by **short term scheduler**.
* **Terminated** - When the process is either complete or terminated by the user, the process goes into terminated state.
* **Waiting** - If a running process wants to do I/O operation, the operating system, puts the process into the wating state. Once the I/O is done, the process moves to ready state.
* **Suspended Ready** - When ready queue is full, the operating system may move a new process to suspended ready state and swap out it into the secondary memory. This task is done by **medium term scheduler**.
* **Suspended Waiting** - When waiting queue is full, the operating system may move a new process to suspended waiting state and swap out it into the secondary memory. This task is done by **medium term scheduler**.
