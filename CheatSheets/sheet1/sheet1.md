# Operating Systems Cheat Sheet
---

### 1. Basics

- Operating System (OS): Software that manages computer hardware and software resources,      providing common services for computer programs.
- Kernel: Core part of the OS, managing system resources and communication between hardware and software.

---

### 2. Types of Operating Systems
- Batch OS: Processes batches of jobs without user interaction.
- Time-Sharing OS: Multiple users can access the system simultaneously.
- Distributed OS: Manages a group of distinct computers and makes them appear as a single computer.
- Embedded OS: Designed for embedded systems.
- Real-Time OS (RTOS): Processes data as it comes in, typically used in systems that require immediate processing.
- Network OS: Provides services to computers connected in a network.
- Mobile OS: Designed specifically for mobile devices.

---

### 3. Processes and Threads
- Process: A program in execution, with its own address space.
- Thread: The smallest unit of processing, sharing the process’s resources.
- Process States: New, Ready, Running, Waiting, Terminated.
- Multithreading: Running multiple threads within a single process.

---

### 4. Process Scheduling

`Scheduling Algorithms:`

- FCFS (First-Come, First-Served): Processes are attended in the order they arrive.
- SJF (Shortest Job First): Processes with the shortest burst time are scheduled first.
- Priority Scheduling: Processes are scheduled based on priority.
- Round Robin (RR): Each process gets a small unit of CPU time in a cyclic order.
- Multilevel Queue: Processes are divided into queues based on priority.


---

### 5. Memory Management
- RAM (Random Access Memory): Volatile memory used by processes.
- Virtual Memory: Extends physical memory onto the disk.
- Paging: Divides memory into fixed-size pages.
- Segmentation: Divides memory into segments of varying sizes.
- Page Replacement Algorithms:
- FIFO (First-In, First-Out): Replaces the oldest page.
- LRU (Least Recently Used): Replaces the least recently used page.
- Optimal Page Replacement: Replaces the page that will not be used for the longest time.


---

### 6. File Systems
- File: A collection of data stored in a storage device.
- Directory: A container that holds files and other directories.
- File System Types: NTFS, FAT32, ext3, ext4, HFS+, APFS.
- File Operations: Create, Open, Read, Write, Delete, Close.
- File Attributes: Metadata about the file, such as name, size, type, permissions.

---

### 7. I/O Management

- I/O Devices: Hardware used for input and output operations.
- Device Drivers: Software that controls a hardware device.
- I/O Scheduling: Manages the order in which I/O requests are processed.
- Buffering: Storing data temporarily while it is being moved from one place to another.

---

### 8. Concurrency
- Concurrency: Multiple processes or threads executing simultaneously.
- Race Condition: When multiple processes or threads access shared data concurrently, leading to unpredictable results.
- Mutex (Mutual Exclusion): Prevents multiple processes from accessing a critical section simultaneously.
- Semaphore: A signaling mechanism to control access to shared resources.
- Deadlock: A situation where two or more processes are unable to proceed because each is waiting for the other to release resources.
- Deadlock Prevention: Ensuring at least one of the necessary conditions for deadlock cannot occur.
- Deadlock Avoidance: Using algorithms like Banker's algorithm to avoid unsafe states.
- Deadlock Detection and Recovery: Allowing deadlock to occur, then detecting and recovering from it.

---

### 9. Security and Protection
- Authentication: Verifying the identity of a user or process.
- Authorization: Granting or denying access to resources based on permissions.
- Encryption: Protecting data by transforming it into an unreadable format.
- Firewall: Controls incoming and outgoing network traffic.
- Antivirus: Software that detects and removes malware.
- User and Group Management: Managing permissions and access rights for users and groups.

---

### 10. System Calls
- Definition: Interface between user programs and the OS.
`Types:`
- Process Control: fork(), exit(), wait()
- File Management: open(), read(), write(), close()
- Device Management: ioctl(), read(), write()
- Information Maintenance: getpid(), alarm(), sleep()
- Communication: pipe(), shmget(), mmap()


---

### 11. Common Commands (Unix/Linux)
`File Operations:`
- ls: List directory contents.
- cd: Change directory.
- cp: Copy files.
- mv: Move or rename files.
- rm: Remove files.
- cat: Concatenate and display files.
`Process Management:`
- ps: Report a snapshot of current processes.
- top: Display and update sorted information about processes.
- kill: Terminate processes.
- bg: Resume suspended jobs in the background.
- fg: Resume suspended jobs in the foreground.
`System Information:`
- uname: Print system information.
- df: Report filesystem disk space usage.
- du: Estimate file space usage.
- uptime: Tell how long the system has been running.
- free: Display amount of free and used memory.

----

### 12. Virtualization
- Virtual Machine (VM): Emulates a physical computer system.
- Hypervisor: Software that creates and manages VMs.
- Type 1: Runs directly on hardware (e.g., VMware ESXi).
- Type 2: Runs on a host operating system (e.g., VirtualBox, VMware Workstation).
- Containerization: Lightweight virtualization using containers (e.g., Docker).

---

### 13. Backup and Recovery
- Backup: Copying data to protect against data loss.
- Full Backup: Complete copy of all data.
- Incremental Backup: Copies only data that has changed since the last backup.
  Differential Backup: Copies all data changed since the last full backup.
- Recovery: Restoring data from a backup after data loss.


---

### 14. Common OS Examples
- Windows: Microsoft's OS with a graphical user interface.
- Linux: Open-source Unix-like OS, commonly used for servers.
- macOS: Apple's Unix-based OS for Mac computers.
- Unix: Multiuser, multitasking OS, known for stability and security.

