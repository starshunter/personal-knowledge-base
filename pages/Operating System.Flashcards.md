deck:: OS

- What is an operating system? #card
  id:: 6207cedd-3f01-41ad-bf8e-80309901f939
	- From users' point of view, it is a program that allows them to interact with computer hardware. From user programs' view, it is a resource allocator and a control program that prevent other programs from damaging the computer
- How does different device connect to computer? #card
  id:: 6207cedd-0349-4f82-9da9-1e3e32579389
	- Devices connect to computer through device driver and device controller, and device controllers are connected through a common bus, which also connect to a shared memory
- How does operating system be loaded into main memory? #card
  id:: 6207cedd-b33a-45b6-bd5f-8d7a14343c86
	- A program called bootstrap program inside ROM will be loaded first after booting up, and then it will load the OS into memory
- What is an interrupt? #card
  id:: 6207cedd-5f2b-4aa8-8766-7fdbe622704a
	- A mechanism to inform CPU that certain task from hardware or software need to be handle
- Why do we need interrupt? #card
  id:: 6207cedd-d05c-474d-a7b5-3953b8f8d86a
	- Without interrupt, CPU has to busy-waiting an operation to finish, which will hamper CPU utilization
- What is the procedure of interrupt? #card
  id:: 6207cedd-e771-4482-88ee-6a9dff871357
	- CPU will save current process's address and state
	- OS use interrupt ID to call interrupt service routine in the interrupt vector
	- CPU runs interrupt service routine
	- resume to previous process
- What happen when an interrupt occur while CPU is handling an interrupt? #card
  id:: 6207cedd-43d9-4fe3-836f-4ed020a7b178
	- The interrupt will be ignored by CPU temporary, and once current interrupt is finished, the interrupt will be handled
- What type of storage can CPU access directly? #card
  id:: 6207cedd-cccc-436c-be24-1ead149c6b23
	- main memory
	- register
- Why do we need secondary storage outside of main memory? #card
  id:: 6207cedd-9209-43fa-9df3-162c2f166f9b
	- Because main memory is too small to store all the data. And also main memory is volatile, once the power is cut off, every thing will be wiped out
- What is the purpose of device driver? #card
  id:: 6207cedd-f873-4278-bbf9-89d075524585
	- It offers an uniform interface for OS to interact with different kind of device
- What is the procedure of a I/O operation? #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-last-reviewed:: 2022-02-12T13:26:54.291Z
  card-next-schedule:: 2022-02-12T16:00:00.000Z
  card-last-score:: 1
  id:: 6207cedd-0888-4b53-99c6-73f36e86572b
	- device driver loads the registers within the device controller
	- device controller than decide what action to take base on the registers
	- controller transfer data from device to its buffer
	- controller informs driver through interrupt once the transfer is completed
- What are the advantages of multiprocessor systems over single processor system? #card
  id:: 6207cedd-23b5-4e2d-8407-ea41d5477444
	- increased throughput
	- economy of scale
	- increased reliability
- What is multiprogramming? #card
  id:: 6207cedd-81f8-49b0-a9c8-afa2a8dbb789
	- It's a OS design that allows CPU to execute other jobs when current process is doing I/O or other works. It increases CPU utilization
- What is multitasking? #card
  id:: 6207cedd-e9a0-4a19-a426-b08b80f97590
	- It's a OS design that divides CPU usage into time slices, which allows CPU to switch jobs frequently and makes user think the whole system is dedicated to his use
- What is job pool? #card
  id:: 6207cedd-a147-465b-b371-eab5e8c92afa
	- Job pool consists of programs that are ready to be loaded to main memory by job scheduling
- Why does OS need dual-mode operation? #card
  id:: 6207cedd-e9b4-47d6-9f97-4f7d7293030b
	- Prevent system being damaged by malicious user
- What is system call? #card
  id:: 6207cedd-51ae-4c76-b819-2e1b341ca80c
	- It's a mechanism that allow user to use services that provided by the OS, normally about managing computation resources
- What is the procedure of system call? #card
  id:: 6207cedd-46cc-49e9-8cde-a82ce53b8262
	- system call is treated by hardware as trap
	- mode bit set to 0
	- OS examine the trap and use interrupt vector to determine which interrupt service routine to execute
	- return control to the instruction following the system call
- What kind of service does OS provide? #card
  id:: 6207cedd-6e83-4033-80c5-90777b46a91f
	- UI
	- program execution
	- I/O
	- file system manipulation
	- communication
	- error detection
	- resource allocation
	- accounting
	- protection and security
- What is the benefit of implementing command through system programs? #card
  id:: 6207cedd-7b91-4217-b395-2b41fb607288
	- Reduce command interpreter's size
	- Easy to add new command
	-
- What is the advantage of using API instead of using system call? #card
  id:: 6207cedd-9dce-4185-8fcd-457f071ddd5e
	- Increase portability and reduce development complexity
- What are ways to pass parameters with system call? #card
  id:: 6207cedd-09b7-4d96-b884-ab718dd99423
	- Pass in register
	- Store in a block, and pass block's address
	- Push parameters onto a stack
- What types does system call consist of? #card
  id:: 6207cedd-779b-4b2f-993e-9e46c69668da
	- process control
	- file management
	- device management
	- communication
- What is the advantage of using message passing for process communication? #card
  id:: 6207cedd-f940-44d5-b7a5-17bff9bc9c68
	- Easy to implement
- What is the advantage of using shared memory for process communication? #card
  id:: 6207cedd-44f2-4892-86c9-e00ce2604b40
	- Faster read and write speed
- What is a system program? #card
  id:: 6207cedd-5f63-4eca-b9b4-7ce141a24be3
	- It is mostly consist of system calls, and OS can view as a collection of system programs
- What is the disadvantage of simple structure OS? #card
  id:: 6207cedd-fd9e-4fa7-a837-c4f137797130
	- Complex structure for more functionality, hard to maintain
- What is the disadvantage of layered OS? #card
  id:: 6207cedd-833b-4ea4-a3a5-fb04f9219eb7
	- Hard to divide services into layers and inefficient
- What is the disadvantage of microkernels OS? #card
  id:: 6207cedd-7b58-45ae-ba3d-e17d0f8e1086
	- Communication between services is inefficient
- Why is modules OS better than layered OS and microkernels OS? #card
  id:: 6207cedd-dee4-4d56-b278-6f6f0805e2e1
	- Different modules can talk to each other, and since both modules and kernel are in kernel space, communication is more efficient
- What is the functionality of SYSGEN? #card
  id:: 6207cedd-adc8-4e73-9b20-16496e6cf648
	- It collects hardware information for OS generation
- What is the functionality of bootstrap program? #card
  id:: 6207cedd-32e9-41f8-87f7-11eb1628379a
	- It is responsible for locating and loading the OS into memory, as well as executing it
- What is the structure of a process in memory? #card
  id:: 6207cedd-2d61-40a2-bb82-4343c9a0d0f6
	- text
	- stack
	- data
	- heap
	- program counter
	- register status
- What kind of state can a process be in? #card
  id:: 6207cedd-5c75-4eae-a075-cb5e317b946c
	- new
	- running
	- waiting
	- ready
	- terminated
- What is a process control block? #card
  id:: 6207cedd-cbb2-42d7-b2a4-b72750482116
	- It's a representation of a process in OS. It contains information such as process state, program counter, CPU register and I/O status
- Why does OS need process scheduler? #card
  id:: 6207cedd-a38e-4a57-811b-5d553625d49a
	- We need a scheduler to decide what process should be execute by CPU, and in what order do other processes get executed
- What is job queue? #card
  id:: 6207cedd-592a-4cbe-886f-9e639f4ae988
	- Processes in this queue reside on disk, and need job scheduler to select them into memory
- What is ready queue? #card
  id:: 6207cedd-db7e-4251-9c13-ac1d8a9c16ff
	- Processes in this queue are in memory and waiting for CPU execution
- What is device queue? #card
  id:: 6207cedd-6262-4508-ac30-d62f8962fd29
	- A device queue contains processes that are waiting for a certain device
- What is job scheduler? #card
  id:: 6207cedd-a7c0-4415-84df-3fa645934d2b
	- It's a long term scheduler that selects which process should be brought into ready queue, and it also controls the degree of multiprogramming
- What is CPU scheduler? #card
  id:: 6207cedd-2af2-4bd9-ae9d-a8dac1e67732
	- It's a short term scheduler that selects which process should be executed by CPU
- What is medium term scheduler? #card
  id:: 6207cedd-e8da-4ecb-a64a-b080b5ee1cd7
	- It's a scheduler that swap processes into or out of memory, to maintain the balance of I/O-bound process and CPU-bound process
- What is context switch? #card
  id:: 6207cedd-7533-495c-add7-283aba0da381
	- It's the process of CPU saving the context of one process, and load another process's context for execution
- What is context of a process? #card
  id:: 6207cedd-c2a6-4e06-b8ce-914d725f0722
	- Context is represented as PCB in the OS
- Why does OS need interprocess communication? #card
  id:: 6207cedd-fd14-46ea-a9b5-80bf72cf775e
	- It allows cooperating processes to exchange data and information, which in turn increase computation speed and system modularity
- How does shared memory work? #card
  id:: 6207cedd-535f-4804-9ba6-fffc14a37650
	- A process first creates a shared memory in its address space, then any other process that wish to use this shared memory has to attach it to its address space, then these processes can read and write into this space
- Why is message passing communication slow? #card
  id:: 6207cedd-437a-4587-86d9-8dbcdd1b9d5c
	- It's slow because it's accomplish through system call
- What is the advantage of indirect communication over direct communication? #card
  id:: 6207cedd-839a-4264-82ce-dbd8c44cfa24
	- Indirect communication is easier to maintain because the messages are sent to and received from mailboxes
- What are some of the mechanism that allow client-server system communication? #card
  id:: 6207cedd-7d53-435c-861b-8b383feda815
	- sockets
	- pipes
	- RPC
- What is the difference between ordinary pipe and named pipe? #card
  id:: 6207cedd-f1e0-496b-9c31-4904b68860dd
	- Ordinary pipe can only be used by processes with parent-child relation, but named pip can be used by processes with no such relation
- What is remote procedure call? #card
  id:: 6207cedd-70c0-46ab-a50a-7a79fe28d280
	- It's a message-based communication that allows a client to invoke a procedure on a remote host
- Why does the system need parameter marshalling in RPC? #card
  id:: 6207cedd-6fa0-4f7d-b2a9-51a16f9ed353
	- Because data representation on different machine are different, and parameter marshalling allows receiving host to unmarshal parameters into its format
- How does client side stubs know the port corresponding to a procedure on the server? #card
  id:: 6207cedd-0e5f-416b-a4a9-8394b3996207
	- Client first sends a message to matchamker to find out the correct port, than send the message to that port
- What is thread? #card
  id:: 6207cedd-f6e3-48f6-bbc6-79e7eeec4534
	- Thread is a basic unit that can be scheduled by scheduler, and be executed by CPU. It consists of a thread ID, program counter, registers set and a set
- What do threads in the same process share? #card
  id:: 6207cedd-8b35-4468-878d-2f1b28e801fa
	- code
	- data (global variable)
	- OS resources (I/O devices, files)
- What is the benefits of using threads instead of processes? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207cedd-49f8-433d-8adf-f023a753f820
	- responsiveness
		- an application can keep running even a thread is blocked
	- resource sharing
	- economy
		- resource allocation and context switch for process are slow
	- utilization of multiprocessor architecture
- What is user thread? #card
  id:: 6207cedd-9ca6-4b84-8121-8be4d37b1650
	- User threads are threads support and manage in user space, OS doesn't know their existence
- What is kernel thread? #card
  id:: 6207cedd-ff02-427c-a4ac-9848bd3756f7
	- Kernel threads run in kernel space, are managed by OS, and can be scheduled to CPU
- Why does user thread has to map onto kernel thread? #card
  id:: 6207cedd-131f-4dc9-a1e9-fc91260f89d4
	- Because only kernel threads can be schedule and executed, OS doesn't know the existence of user threads, so for user threads to execute, it must map onto a kernel thread
- What is the disadvantage of many-to-one model? #card
  id:: 6207cedd-0f6c-4226-95b5-bea67b287d0d
	- A blocking system call may block the entire process, and a kernel thread can not utilize multiprocessor architecture
- What is the disadvantage of one-to-one model? #card
  id:: 6207cedd-ebcd-4843-a14d-c45bc3c6d692
	- A kernel thread has to be created for a user thread, the creation process is an overhead that will lower system performance
- What is a lightweight process? #card
  id:: 6207cedd-a955-489f-8434-9a985c598108
	- It's an intermediate data structure provided by kernel to application, it can be viewed as virtual processor and used to schedule a user thread onto it
- Why does OS need scheduler activation? #card
  id:: 6207cedd-9882-460c-b162-fd2175f370e6
	- A user thread may make a blocking system call and blocks a thread, so a mechanism is needed to allow other user threads to execute
- What is the procedure of scheduler activation? #card
  id:: 6207cedd-605c-48af-91d5-0d10874bb925
	- a user thread may block LWP and kernel thread if it makes a blocking system call
	- kernel informs application through upcall
	- kernel allocate another LWP for application, and application runs upcall handler to handle upcall on that LWP
	- upcall handler saves the state of the blocking thread and release the blocking LWP
	- upcall handler assign an user thread to new LWP
	- kernel inform application through upcall when the blocked thread can run again
- What is a preemptive CPU scheduling algorithm? #card
  id:: 6207cedd-bc9e-423d-a3e3-d98aa4894ac5
	- A process may be selected to be executed when it switches from waiting state to ready state or another process switches from running state to ready state
- What is the downside of preemptive CPU scheduling? #card
  id:: 6207cedd-8ccc-46a2-9c47-3059712530cd
	- Shared data between processes may be in inconsistent state, and if a process is preempted during a system call, chaos could occur
	-
- What is the responsibility of a dispatcher? #card
  id:: 6207cedd-96f8-42d7-9c8a-e47f55354306
	- It is responsible for transferring CPU control to the process selected by CPU scheduler, including switching context, switching to user mode and jumping to proper location of the program
- What is throughput? #card
  id:: 6207cedd-3120-42ec-ad5b-c5fa6b769abf
	- The number of processes that complete execution in the given time
- What is turnaround time? #card
  id:: 6207cedd-bd35-4fa6-bf7f-428596cfead8
	- Total amount of time to execute a process, including the time waiting in the ready queue, executing on CPU and waiting for I/O...
- What is response time? #card
  id:: 6207cedd-3902-407c-80b0-6c9d2285058f
	- The time between a process being submitted and the first response is produced
- What is the disadvantage of using FCFS algorithm? #card
  id:: 6207cedd-07cd-49ca-92be-4ea76da4eaf3
	- The performance depends a lot on the order of the processes
- Why is it unrealistic to use shortest-job-first scheduling? #card
  id:: 6207cedd-0ca0-49c6-84a1-ee53aa480da9
	- It's hard to predict CPU burst length accurately
- What is the disadvantage of priority scheduling? #card
  id:: 6207cedd-fbef-4be1-993e-1bbe108bfeb0
	- Low priority processes may wait a long time before executing
- What is the difference between multilevel queue scheduling and multilevel feedback-queue scheduling? #card
  id:: 6207cedd-7001-4e41-bf00-4c2ccf65b222
	- They all divide processes into different queue, and define which scheduling to use on different queues, but multilevel feedback-queue also define how a process should move between queues
- What is processor affinity? #card
  id:: 6207cedd-2a98-4e0d-8a83-d5cbbdd27750
	- If a process originally run at a processor, the cache of that processor has data related to that processor, than next time this process is scheduled to be executed, OS tends to schedule it to the original processor
- How do user threads get executed? #card
  id:: 6207cedd-e341-4928-9618-b5c481b93f6e
	- First, user threads get scheduled onto LWP, the scheduling is handled by thread library, and then kernel threads get scheduled onto CPU, the scheduling is handled by CPU scheduler
- What is race condition? #card
  id:: 6207cedd-09ab-4fd6-8387-0491d55644fa
	- Several processes can modify the same data at the same time, and the result depends on the order in which the modification takes place
- What is critical section? #card
  id:: 6207cedd-2e6c-4750-9c59-931be851856f
	- Critical section is a segment of code where processes may modify some shared resources, and without caution, this may result in race condition
- What properties should a solution to critical section problem have? #card
  id:: 6207cedd-3323-4712-9236-d161c6e047b1
	- mutual exclusive
	- progress
	- bounded waiting
- What is Peterson's solution? #card
  id:: 6207cedd-7305-4fd5-87b6-c0f1e1225e2e
	- It's a solution for critical section problem with only two processes, and it uses two flags to indicate request, one variable to indicate which process could enter
- How can hardware help solving the critical section problem? #card
  id:: 6207cedd-d396-401e-b1a5-18da40b80c02
	- Hardware can implement atomic `TestAndSet()` or `Swap()`, which can be used to construct a solution
- What is semaphore? #card
  card-last-interval:: 4
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-02-16T13:26:29.271Z
  card-last-reviewed:: 2022-02-12T13:26:29.273Z
  card-last-score:: 3
  id:: 6207cedd-bf65-481a-9cdb-44ac24540de8
	- It's a software solution to critical-section problem
- How to avoid busy waiting in semaphore implementation? #card
  id:: 6207cedd-4ca5-46d6-80f6-5df0384ea8fc
	- Block the waiting process and place it in a waiting queue, and processes in waiting queue can move back to ready queue only when another process execute `signal()`
- What is monitor? #card
  id:: 6207cedd-5701-47c0-86e9-e4034d90c489
	- It's a high level programming language construct that help solving the critical section problem, which also make programming easier
- What is deadlock? #card
  id:: 6207cedd-d5e1-4c11-a8b9-2066a4c990d5
	- It's a state that a set of processes is waiting for some events to occur, and those events can only be caused by another process in the set
- What conditions need to be satisfied for a deadlock to occur? #card
  id:: 6207cedd-ac69-4f9d-9133-91154eef03fc
	- mutual exclusion
		- only one process at a time can use a resource
	- circular wait
		- $P_0$ wait for $P_1$, $P_1$ wait for $P_2$, and $P_n$ wait for $P_0$
	- hold and wait
		- a process is holding at least one resource, and is waiting for resources hold by others
	- no preemption
		- a resource can only be released voluntarily by the process that allocate it
- What is deadlock prevention? #card
  id:: 6207cedd-31c3-4716-8a5c-4ed3df1bacd0
	- It's the method that can prevent system from entering deadlock state by ensuring one of the deadlock conditions never hold
- What is deadlock avoidance? #card
  id:: 6207cedd-618d-4560-980e-ade5b96c33c7
	- It's an algorithm that ensure the system will not enter a deadlock state
- What is a safe state in deadlock avoidance? #card
  card-last-interval:: 4
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-02-16T13:27:14.957Z
  card-last-reviewed:: 2022-02-12T13:27:14.958Z
  card-last-score:: 3
  id:: 6207cedd-00a2-4eda-9057-89227fac8fbb
	- It's a state that system can allocate resources in some order that will not result in a deadlock state
- How does OS define a memory space for user program? #card
  id:: 6207cedd-ca82-4e8f-9b74-719f1f18d51d
	- It uses base register and limit register
- What is address binding? #card
  id:: 6207cedd-f061-42e5-8012-343761fe2574
	- To move a process from disk to memory, we need to map every logical addresses in the program onto a physical address, so that it can exist in the memory
- How does the timing of address binding affect program's execution? #card
  id:: 6207cedd-447a-4054-b7c0-6bab8600c175
	- compile time
		- if starting location change, then recompile is needed
	- load time
		- if starting location change, then reload is needed
	- execution time
		- mostly use when the process can be moved during its execution
- What is dynamic loading? #card
  id:: 6207cedd-a0bd-449a-aa71-808dc29a8ef7
	- It's a mechanism that a program is not loaded into memory until it is called
- What is dynamic linking? #card
  id:: 6207cedd-1cc5-4165-8dad-c4ff5564697d
	- It's a method to postpone linking of some libraries to execution time, which can increase memory utilization efficiency because only one copy of the library need to be in the memory
- What is swapping? #card
  id:: 6207cedd-1d36-4455-bcbc-bff280b8bea7
	- A process may reside on the disk, and to execute it, we need to swap out a process to make space for swapping it in
- When does swapping happen? #card
  id:: 6207cedd-5f52-4a4d-b7a0-cb8c14b02f3d
	- It happens after CPU scheduler making the decision and OS calls the dispatcher
- What is contiguous memory allocation? #card
  id:: 6207cedd-3c20-44d6-bf7c-9c1d7e4c5ddf
	- Process is located in a contiguous space inside the memory
- What is external fragmentation? #card
  id:: 6207cedd-5926-4c00-916a-93880d11176b
	- Total space left in the memory is enough for a process, but those spaces are contiguous
- What is internal fragmentation? #card
  id:: 6207cedd-5333-4669-8f46-8b94914b6d97
	- In fixed sized partition, each partition is slightly larger than the process that it allocates to
- What is compaction? #card
  id:: 6207cedd-fd85-4af1-9a3c-ae5147ee5995
	- It's a method to merge all free memory spaces into a large block
- What is paging? #card
  id:: 6207cedd-c56b-4835-af25-9c977a1e86e8
	- It's a memory management scheme that allows the physical address space of a process to be noncontiguous, to be specific, process's logical memory is divided into page, and physical memory is divided into frame
- How is paging implemented? #card
  id:: 6207cedd-5a56-4c4f-8a79-074872159132
	- OS need a page table for each process, can be implemented as registers or directly placed in memory
- What is the benefit of shared page? #card
  id:: 6207cedd-59ad-4c47-8c44-1404f07159f2
	- Processes can share common section that code to reduce memory usage
- Why do we need hierarchical paging? #card
  id:: 6207cedd-be71-4237-85c1-58de1de9b1f9
	- A single page table may be too large to store it in memory contiguously
- What is the disadvantage of using inverted page table? #card
  id:: 6207cedd-591b-4431-85d6-19a27299ee95
	- Searching is time consuming, also it's hard to implement shared page
- What is segmentation? #card
  id:: 6207cedd-74b0-455f-94a5-4ac772397dde
	- It's a mechanism to map programmer's view of program onto physical address space
- What is virtual memory? #card
  id:: 6207cedd-3139-4cbf-ae27-b12e16b6dc5f
	- It's a technique that allows a program to execute without being entirely loaded into the memory
- What is the benefit of virtual memory? #card
  id:: 6207cedd-9f23-4a75-8ae0-ed3b49f58a70
	- system libraries can be shared by several processes
	- enable process to share memory
	- speeding up process creation
- What is demand paging? #card
  id:: 6207cedd-8a2e-4398-bee5-13e070100160
	- It's a technique that pages are loaded into memory only when they are demanded
	-
- What is copy-on-write? #card
  id:: 6207cedd-7b06-40e5-9789-a32b40ccb1c1
	- It's a technique that allow parent process to share pages with child process initially, and when one of the process try to modify a shared page, a copy of that page will be created
- What is the purpose of modify bit? #card
  id:: 6207cedd-4bd4-4557-be49-eb9e131b2641
	- If we need to swap out a page whose modify bit is set, it means that page has been modified since it get brought into memory, so it's necessary to write it back to disk
- What is page buffering algorithm? #card
  id:: 6207cedd-e188-4eda-8d72-7bfec484184b
	- It's a mechanism that OS maintains a list of free frames, so we can execute swap in and swap out concurrently
- How do frames allocate to each process? #card
  id:: 6207cedd-300f-485a-bdd2-96a29c654b78
	- equal allocation scheme
		- split frames equally
	- proportional allocation scheme
		- allocate frames according to process size
- What is thrashing? #card
  id:: 6207cedd-2686-4771-9fc8-aeff1a985c78
	- It's a situation where a process spends more time on paging than on executing
- How do we avoid thrashing? #card
  id:: 6207cedd-7083-43c9-b60f-6ca449844f04
	- Allocate enough frames to each process by one of these method
		- working-set model
		- page-fault frequency
- What is memory-mapped files? #card
  id:: 6207cedd-29fe-4ff5-8a07-fea5440c8b71
	- It's a mechanism that allows a part of the virtual address space to be logically associated with a file