# 📘 Operating System Concepts Summary

---

## 🧠 1. Process and Process Table
- A **process** is a program in execution.
- The **process table** holds information about each process like state and resources used.

---

## 🚦 2. Process States
- **Running**: Actively using the CPU.
- **Ready**: Ready to use CPU.
- **Waiting**: Waiting for an event.

---

## 🧵 3. Thread
- A lightweight process that shares memory with other threads in the same process.

---

## 🔁 4. Process vs Thread

| Feature       | Process              | Thread               |
|---------------|----------------------|-----------------------|
| Entity        | Independent          | Sub-part of a process |
| Memory        | Isolated             | Shared                |
| Communication | Slower               | Faster                |
| Control Block | PCB                  | TCB                   |

---

## ⚡ 5. Benefits of Multithreading
- Improved responsiveness
- Efficient resource sharing
- Less overhead

---

## 🌀 6. Thrashing
- Excessive paging causes system slowdown.

---

## 📦 7. Buffer
- Temporary memory storing data in transfer.

---

## 💾 8. Virtual Memory
- Uses disk to simulate extra RAM.

---

## 🖥️ 9. Purpose of OS
- Interface between user and hardware.
- Ensures efficient execution of programs.

---

## 📥 10. Demand Paging
- Load pages into memory only when needed.

---

## 🔧 11. Kernel
- Core of OS managing memory, CPU, and I/O.

---

## 🗓️ 12. Scheduling Algorithms
- FCFS, SJN, Priority, SRT, RR, Multi-Level Queues.

---

## 🧮 13. Objective of Multiprogramming
- Increase CPU utilization by keeping multiple jobs in memory.

---

## 🕓 14. Time-Sharing System
- Allows multiple users to interact with programs concurrently.

---

## ❌ 15. Without OS
- No UI, resource management, file system, etc.

---

## 🧩 16. Multithreading (Again)
- Allows parallel execution within a process.

---

## 🗂️ 17. FCFS Scheduling
- Non-preemptive, job that arrives first is served first.

---

## 🔄 18. Round Robin Scheduling
- Fair, cyclic CPU allocation using time slices.

---

## 💽 19. RAID Levels
- RAID 0 to RAID 6: Different redundancy and performance.

---

## 🏦 20. Banker’s Algorithm
- Avoids deadlock by simulating safe resource allocation.

---

## 🧭 21. Logical vs Physical Address

| Type     | Logical Address           | Physical Address            |
|----------|---------------------------|------------------------------|
| Generated | By CPU                   | By MMU                       |
| User View | Visible                  | Hidden from user             |
| Usage    | Access virtual memory     | Access actual memory         |

---

## 🔌 22. Dynamic Loading
- Load routines only when called, saving memory.

---

## 🔄 23. Overlays
- Only required part of program is loaded into memory.

---

## 📉 24. Fragmentation
- Small unusable memory gaps due to dynamic allocation.

---

## 📚 25. Paging
- Fixed-size partitions of memory used to store processes.

---

## 🔁 26. Swapping
- Moves processes between main and secondary memory to manage load.

---

## 🔐 27. Classic Synchronization Problems
- Bounded-buffer, Readers-writers, Dining philosophers, Sleeping barber.

---

## 📡 28. Direct Access Method
- Access blocks directly on disk or memory using DMA.

---

## 🔁 29. Thrashing Cause
- High page fault rate causes system overload.

---

## 📏 30. Best Page Size
- Depends on system; balance between overhead and efficiency.

---

## 🖥️ 31. Multitasking
- Multiple tasks executed concurrently by sharing CPU.

---

## 🧠 32. Caching
- Small, fast memory for frequently used data.

---

## 📃 33. Spooling
- Buffering jobs for slow devices like printers.

---

## 🧱 34. Assembler
- Converts assembly language to machine code.

---

## ⚠️ 35. Interrupts
- Signals to CPU to attend high-priority events.

---

## 🖼️ 36. GUI
- Graphical User Interface with icons and windows.

---

## 🔁 37. Preemptive Multitasking
- OS switches between processes by force.

---

## 🧵 38. Pipe
- One-way inter-process communication.

---

## 📊 39. Semaphore Advantages
- Prevents busy waiting, machine-independent, easy correctness checking.

---

## 🚀 40. Bootstrap Program
- Initializes OS during system startup.

---

## 🔗 41. IPC (Inter-Process Communication)
- Synchronization and data sharing between processes.

---

## 🔄 42. IPC Mechanisms
- Pipes, Named Pipes, Message Queues, Semaphores, Shared Memory, Sockets.

---

## ⏸️ 43. Preemptive vs Non-Preemptive

| Aspect       | Preemptive           | Non-Preemptive             |
|--------------|----------------------|-----------------------------|
| Interruption | Allowed              | Not allowed                 |
| Flexibility  | High                 | Rigid                       |
| Starvation   | Possible             | Possible                    |

---

## ☠️ 44. Zombie Process
- Terminated but not removed from process table.

---

## 👻 45. Orphan Process
- Parent terminated before child.

---

## ⏳ 46. Starvation vs Aging
- Starvation: Long wait for resources.\n- Aging: Increases priority over time.

---

## 🧠 47. Monolithic Kernel
- All OS services in one address space for faster execution.

---

## 🔁 48. Context Switching
- Switches CPU from one process to another by saving and restoring states.

---

## 💻 49. OS vs Kernel

| Feature       | Operating System       | Kernel                    |
|---------------|------------------------|----------------------------|
| Role          | Full system software   | Core system manager        |
| Interface     | User-hardware bridge   | Application-hardware bridge |

---

## 🧵 50. Process vs Thread (Again)

| Feature        | Process                | Thread                   |
|----------------|------------------------|---------------------------|
| Memory Space   | Separate               | Shared                    |
| Communication  | Slower                 | Faster                    |

---

## 📘 51. PCB (Process Control Block)
- Stores process metadata like registers, priority, and state.

---

## ✅ 52. Safe State
- All processes can complete without deadlock.

---

## 🕳️ 53. Cycle Stealing
- Access memory without disturbing the CPU.

---

## 🔐 54. Trap vs Trapdoor

| Term       | Meaning                                   |
|------------|-------------------------------------------|
| Trap       | Software interrupt (e.g., errors)         |
| Trapdoor   | Hidden backdoor for unauthorized access   |

---

## 📑 55. Program vs Process

| Type      | Program                         | Process                       |
|-----------|----------------------------------|-------------------------------|
| Nature    | Static code                     | Dynamic execution             |
| Lifespan  | Persistent                      | Temporary                     |
| Entity    | Passive                         | Active                        |
| Resources | Only code memory                | CPU, memory, I/O              |

---



## 🚀 CPU Scheduling & Dispatcher (Q56–Q58)

- **56. Dispatcher**  
  Transfers control of the CPU to the process selected by the scheduler. Tasks:
  - Context switching
  - Switching to user mode
  - Jumping to the correct instruction

- **57. Dispatch Latency**  
  Time taken by the system to switch from one process to another after scheduling.

- **58. Goals of CPU Scheduling**  
  - Maximize CPU utilization & throughput  
  - Minimize waiting, turnaround & response time  
  - Fair CPU allocation

---

## 🔐 Critical Section & Synchronization (Q59–Q67)

- **59. Critical Section**  
  Code segment where shared resources are accessed; requires synchronization.

- **60. Synchronization Techniques**  
  - Mutexes  
  - Semaphores  
  - Condition variables  
  - File locks

- **61. User vs Kernel Threads**  
  | Feature | User-Level Thread | Kernel-Level Thread |
  |--------|-------------------|----------------------|
  | Implementation | User space | OS space |
  | Context Switch | Fast | Slow |
  | Blocking | Entire process blocks | Only the thread blocks |

- **62. Advantages of Multithreading**  
  - Increased responsiveness  
  - Efficient CPU usage  
  - Better performance & structure

- **63. Multithreading vs Multitasking**  
  - Threads share a process; tasks are independent processes  
  - Multithreading is lighter and faster

- **64. Drawbacks of Semaphores**  
  - Risk of deadlock  
  - Priority inversion  
  - Programmer-dependent

- **65. Peterson’s Algorithm**  
  Synchronizes two processes using a flag array and a `turn` variable to ensure mutual exclusion.

- **66. Bounded Waiting**  
  Guarantees that a process entering a critical section will do so within finite time.

- **67. Critical Section Solutions**  
  - Software methods  
  - Hardware instructions  
  - Semaphores

---

## 💀 Deadlock & Concurrency (Q68–Q75)

- **68. Banker’s Algorithm**  
  Deadlock-avoidance algorithm that simulates resource allocation safely.

- **69. Concurrency**  
  Multiple processes progressing at the same time (not necessarily in parallel).

- **70. Drawbacks of Concurrency**  
  - Performance overhead  
  - Deadlocks, starvation, race conditions

- **71. Deadlock Conditions**  
  - Mutual exclusion  
  - Hold and wait  
  - No preemption  
  - Circular wait

- **72. Issues in Concurrency**  
  - Race conditions  
  - Starvation  
  - Blocking  
  - Deadlock

- **73. Precedence Graph**  
  DAG showing execution order of statements or processes.

- **74. Resource Allocation Graph (RAG)**  
  Shows process-resource relationships and helps detect deadlocks visually.

- **75. What is Deadlock?**  
  When processes wait indefinitely for each other’s resources.

---

## 💾 Memory Management (Q76–Q88)

- **76. Goals of Memory Management**  
  - Relocation, Protection, Sharing  
  - Logical & physical memory organization

- **77. Logical vs Physical Address**  
  Logical = virtual address from CPU  
  Physical = actual address in memory

- **78. Address Binding**  
  Mapping of instructions/data to physical memory.

- **79. Types of Binding**  
  - Compile-time  
  - Load-time  
  - Execution-time

- **80. Dynamic Allocation Advantages**  
  - Efficient memory use  
  - Required for dynamic structures (lists, trees)

- **81. Internal vs External Fragmentation**  
  | Feature | Internal | External |
  |---------|----------|----------|
  | Memory Type | Fixed-size | Variable-size |
  | Cause | Unused space within allocation | Gaps between allocations |
  | Solution | Best-fit | Compaction, Paging

- **82. Compaction**  
  Rearranges memory contents to create large free blocks.

- **83. Hashed Page Table (HPT)**  
  - 🟢 Faster access for sparse pages  
  - 🔴 Collisions reduce performance

- **84. Paging vs Segmentation**  
  - Paging: Fixed-size pages, internal fragmentation  
  - Segmentation: Variable-size segments, external fragmentation

- **85. Associative vs Cache Memory**  
  - Associative: Access by content  
  - Cache: High-speed access by address

- **86. Locality of Reference**  
  Tendency to access the same or nearby memory addresses repeatedly.

- **87. Virtual Memory Advantages**  
  - Large program support  
  - Eliminates external fragmentation  
  - Improves multitasking
