# Operating-System-Bytes


### Operating System
Its a system software which works as a interface between user and hardware.
Hardware - I/O Devices, CPU

### Why Operating System?
If no Operating System, the user needs to write program to access every hardware, ex - To Print a Doc, the user need to invoke the printer by writing program.

### Major Goals of Operating System
1. Convinience - Easiest Access (Windows accquired 95% market, once beacuse of convinnece)
2. Throughput - No of task executed per unit time (Linux) it gave us most efficiency.

### Functionality of Operting System
1. Resource Manger - When multiple user access, what to allocated to who is managed by Resource Manager.
2. Process Management - How to execute multiple process, (CPU Schedulling).
3. Storage Management - Harddisk (FileSystem - NFS, CIFS - How we store data in hardware, how its stored in disk architecture)
4. Memory Management - (RAM) Limitation of Size, Whenever a process executes it comes first to RAM, (Alloc & DeAlloc) occurs here. 
5. Security and Privacy - Authenticated Person can only access windows. (If any process trys to interfare other process, it gets blocked).

### Types of Operating System
1. Batch - Similar type of jobs batched - 1960 - NASA - used Punchcards to load jobs offline - They go to company - Operator - Operator Makes B1 B2 B3 - B1 will be added to CPU for execution, when CPU need to perform I/O, It goes to IDLE, then after finishin the current job, Then its goes to B2 (next job). No fix date for result. IBM made Monitor System which replaced Operators - IBSYS709X 1960 (User can directly go and execute the job)
2. Multiprogrammed - Non Preemptive - When a program is to be executed, CPU will executed it completely untill the program itself says it wants to access I/O or other operation, when the program goes to perform I/O, CPU will jump to next program execution. Less IDLENESS
3. Multitasking - Preemptive - It will be executed in a certian amount to time, if its completes well and good, if it doesn't, it will be scheduled later. So it will touch every program (Responsiveness)
4. RealTime OS - The output should be almost with minimum time difference, NO DELAYS
      * Hard - Missile System, Flight System
      * Soft - Computer Games, Youtube Live Streaming
5. Distributed - Systems are distributed (Geographically Distributed) losly copuled, If one system fails other system can executed the work.
6. Clustered - Same work as distributed, but connected thorugh LAN (kind of super computer) increased computation power. Advantages - Load Balancing, Power.
7. Embedded - It can perform only a specific task which was set once it was made. Eg - AC, Washing Machine

### Process States
Figure - New - Ready - (Wait/Block)- Running - Terminared
1. New - Process Created not runned only stored.
2. Ready - Ready Queue, now its in Ram. Only few process can be in ready state, Long Term Schedular bring the processes in RAM (Multiprogramming) 
    * Few process dispatched to Running State (No. of dispatched depends on power of CPU). after completed - Terminated- then DeAllocate.
    * When RAM throws a priority task to CPU, then CPU will send the previous incomplete task to READY again (Priority), Time Quantum is one other factor which send the task to ready state, (Time Quantum - Specific amount of time allocated to perform the task, if its complete then terminates, if not sends back to ready and reschedule) It is done by STS (Short Term Schedular - has resonsibilty to schedule).
    

