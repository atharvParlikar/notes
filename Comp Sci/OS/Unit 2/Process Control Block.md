Process Control Block is a datastructure to store information about a process such as
- Stack pointer
- Process State
- Process Number
- Registers
- Memory Limits
- Open File Lists
- Misc. Accounting and state data

### here's a detailed overview of each
-   **Pointer –** It is a stack pointer which is required to be saved when the process is switched from one state to another to retain the current position of the process.
-   **Process state –** It stores the respective state of the process.
-   **Process number –** Every process is assigned with a unique id known as process ID or PID which stores the process identifier.
-   **Program counter –** It stores the counter which contains the address of the next instruction that is to be executed for the process.
-   **Register –** These are the CPU registers which includes: accumulator, base, registers and general purpose registers.
-   **Memory limits –** This field contains the information about memory management system used by operating system. This may include the page tables, segment tables etc.
-   **Open files list –** This information includes the list of files opened for a process.


To identify each process OS assigns a process identification number (PID) to each process.
And as the OS is multi-programming it needs to keep track of all the processes, PCB is also useful during context switching as it stores the necessart info about the process to restart later.
There is also something known as Process table...
![[Pasted image 20230126145844.png]]