# Usermode and Kernel mode

* **Mode Bit** - In user mode, the mode bit is set to 1. In kernel mode, the mode bit is set to 0.

* **User mode** - All application programs runs in user mode. In this mode, the application can not access the hardware functionalities.

* **Kernel Mode** - When an application wants to access the hardware functionality, it mades a system call. The system call is the API provided by kernel to ask the OS for hardware access. The mode is switched and the request is served.

## Workflow of system call

**Steps**
1. The application runs in user mode. The mode bit is set to 1.
2. The application encouters a system call and invokes it.
3. The mode bit is set to 1 and mode switc happens.
4. A trap interrupt is generated for the system call.
5. The trap handler searches the kernel subrouting address that needs to execute from the interrupt table.
6. The handler is executed in kernel mode.
7. The mode bit is set to 1.
8. The control returns to the application.