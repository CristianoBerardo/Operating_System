# Operating System 

This repository contains materials for the **Operating Systems** course, a third-year offering within the **BSc in Computer, Communication and Electronic Engineering** program at **UNITN**. It covers fundamental concepts, advanced topics, and practical examples related to how operating systems function and manage computer resources.


## Contents Summary

### 1. What is an Operating System?
* Explores the core definition of an operating system.
* Details the components of a **computer system** and their interactions.
* Discusses **memory** organization and the performance hierarchy of different storage levels.
* Examines **modern system architectures**, including the **processor** and **high-performance computing (HPC)**.
* Covers the **startup process**, methods to **improve performance**, **switching mechanisms**, **security and OS protection**, **program counters**, and **storage management**.

### 2. Operating-System Structures
* Outlines various **Operating System Services**, including **(G)UI**.
* Explains **System Calls**, how parameters are passed, and different types of system calls, with examples like **MS-DOS** and **FreeBSD**.
* Discusses **Operating System Design and Implementation**.
* Compares different **kernel implementations**: **Monolithic Kernel (UNIX)**, **Layered Approach**, **MicroKernel System Structure**, **Solaris Modular Approach**, and **Hybrid Systems**.

### 3. Process
* Introduces the **Process Concept**, including **process states** and the **Process Control Block (PCB)**.
* Explains **Context Switching**.
* Covers **Threads** and **multitasking in mobile systems**.
* Details **Process Scheduling**, **Process Creation**, and **Process Termination**, including Android's process termination hierarchy.
* Explores **Inter-process Communication (IPC)**, including the **producer-consumer problem**, **message passing** (direct and indirect communication), and **synchronization**.
* Discusses **Pipes** (ordinary and named) and **Communication in Client-Server Systems** using **sockets** and **Remote Procedure Calls (RPC)**.

### 4. Threads & Concurrency
* Revisits the **Process Concept** with a focus on **motivation** for threads.
* Explains **Multi-Threading**, including the difference between `fork` and threads, and **Linux Threads**.
* Highlights the **benefits of multi-threading**.
* Covers **Multicore Programming** and **Amdahl's Law**.
* Examines various **Multi-thread models**: **Many-to-One**, **One-to-One**, **Many-to-Many**, and **Two-level Model**.
* Discusses **Thread libraries** like **Java Threads** and **OpenMP**.
* Explores **Implicit threading**, **Thread Pools**, and **Fork-Join Parallelism**.
* Delves into **CPU scheduling** with **basic concepts**, **CPU Scheduler**, **preemptive and nonpreemptive scheduling**, **dispatcher**, and **scheduling criteria**.
* Analyzes different **Scheduling Algorithms**: **FCFS**, **SJF**, **SRT**, and **Round Robin**.
* Explains **Priority Scheduling** and **Scheduling using multiple queues** (multilevel queue, multiprocessor systems, multi-core processors).
* Covers **Real-time CPU scheduling**, **latencies**, and **priority-based scheduling**.
* Provides **OS scheduling examples** from **Linux**, **Windows**, and **Solaris**.
* Discusses **Scheduling evaluation** using **queueing models** and **simulations**.

---

### 5. Synchronization Tools
* Introduces **Critical section** and **race conditions**, and the **critical section problem**.
* Presents **Software solutions** like **Peterson's Solution**, considering **reordering** and comparison with multi-threading.
* Explains **Memory Barrier** and **Hardware instructions** for synchronization.
* Covers **Atomic Variables** and **Mutex Locks**.
* Detailed explanation of **Semaphores**, including `wait` and `signal` operations, implementation without busy waiting, and common problems.
* Discusses **Monitors**, their implementation using semaphores, **condition variables**, and resuming processes within a monitor.
* Addresses **Single Resource allocation**.
* Examines **Liveness** issues, **Deadlock**, **Starvation**, and **Priority Inversion**.

### 6. Synchronization Examples
* Provides practical examples of synchronization mechanisms.
* Covers **POSIX Synchronization**, including **POSIX Mutex Locks**, **POSIX Semaphores** (named and unnamed), and **POSIX Condition Variables**.
* Discusses **Java Synchronization** and **Java Semaphores**.
* Explains **OpenMP Synchronization**.
* Illustrates solutions to classic synchronization problems: **Bounded buffer**, **Readers-Writers Problem**, and **Dining-Philosophers Problem** (including a monitor solution).

### 7. Deadlocks
* Analyzes **Resource-Allocation Graphs**.
* Discusses various **Methods for Handling Deadlocks**: **Deadlock Prevention** (e.g., avoiding circular wait) and **Deadlock Avoidance**.
* Explains the concept of a **(Thread-)Safe State**.
* Provides a **recap** of deadlock concepts.

---

### 8. Main Memory
* Introduces concepts of **Spatial Locality and Temporal Locality**.
* Covers **Protection** mechanisms, including **Hardware Address Protection** and **Address Binding**.
* Explains the **Memory Management Unit (MMU)**, **Logical vs. Physical Address Space**, and how the MMU handles situations with large programs and limited memory.
* Discusses **LINKING AND LOADING**, including **Dynamic loading** and **Static vs Dynamic Linking**.
* Examines **Program allocation**, including **Contiguous Allocation**, **Variable Partition**, the **Dynamic Storage-Allocation Problem**, **Fragmentation**, and **Compaction**.
* Details **Paging**, the **Address Translation Scheme**, and **Paging Hardware**.
* Calculates the number of pages, discusses **Implementation of Page Table**, **Translation Look-Aside Buffer (TLB)**, and **Effective Access Time**.
* Relates **C code and page faults**.
* Explains **Page Faults**, how they are detected, steps in handling them, and the cost of a page fault.
* Covers **Page replacement strategy**, what happens when there's no free frame, and **Basic Page Replacement**.
* Analyzes various **Page and Frame Replacement Algorithms**: **FIFO**, **Optimal (?) Algorithm**, **Least Recently Used (LRU) Algorithm**, **LRU Approximation Algorithms**, and **Counting Algorithms**.
* Discusses **Allocation of frames to processes** (Fixed, Proportional, Global vs. Local), **Reclaiming Pages**, **Thrashing**, and **Page-Fault Frequency**.

### 9. More on Virtual Memory
* Explores **Page swapping**, including context switch time with swapping and swapping on mobile systems.
* Details the **Structure of the Page Table**: **Hierarchical Page Tables**, **Hashed Page Tables**, and **Inverted Page Table**.
* Introduces **Segmentation** and compares **Paging vs Segmentation**.

---

### 10. Mass-Storage Systems
* Discusses **Nonvolatile Memory Devices**.
* Covers **HD Scheduling** algorithms: **FCFS**, **SCAN (elevator algorithm)**, **C-SCAN**, and criteria for choosing a disk-scheduling algorithm.
* Examines **NVM Scheduling**.
* Explains **Device management**, including **Storage Device Management** and **Swap-Space Management**.
* Covers **Host Storage Attachment** and **Cloud Storage**.
* Introduces **Redundant Array of Independent Disks (RAID)**.

### 11. File-System Interface
* Defines **What's a File?**, including **File Attributes** and **File Structure**.
* Covers **File access and operation**, including **File Locking** and **Access Methods**.
* Explains **Memory-Mapped Files**.
* Discusses **Disk and File Systems** and **Types of File Systems**.
* Details **Directory Structure**: **Directory Organization**, **Single-Level Directory**, **Two-Level Directory**, **Tree-Structured Directories**, **Acyclic-Graph Directories**, and **General Graph Directory**.
* Addresses **Protection** within file systems.

---

### 12. File System Implementation
* Explores **File-System Structure** and the **Layered File System** (Device drivers, Basic file system, File organization module, Logical file system).
* Discusses **File System Types**.
* Traces the path **From API to implementation**, covering **File-System Operations**, **File Control Block (FCB)**, and the **Linux iNode**.
* Details **In-Memory File System Structures**.
* Explains **Directory Implementation** using **Linear** and **HashTable** methods.
* Covers **Allocation Method**s: **Contiguous Allocation Method**, **Linked Allocation**, **FAT Allocation Method**, and **Indexed Allocation Method**, along with their **performance**.
* Discusses **Free-Space Management** (Linked Free Space List on Disk and in Memory).
* Provides insights into **FS in other OS** like **Window's File Systems** and **The Apple File System**.

### 13. Other File Systems
* Examines **File Sharing**.
* Discusses **Remote File Systems** and the **Client-Server Model**.
* Introduces **Distributed Information Systems (DIS)**.
* Covers **Consistency Semantics**.
* Explores **Virtual File Systems** and their implementation.

---

### 14. Virtualization and Virtual Machines
* Defines **Virtualization** and **Virtual machines**.
* Discusses the **Implementation of VMMs** (Virtual Machine Monitors).
* Highlights **Benefits and Features** of virtual machines.
* Explains **Running modes** and **Trap-and-Emulate** virtualization.
* Compares virtual machines with **Containers**.
* Categorizes **Types of VMs and implementations**: **Type 0 Hypervisor**, **Type 1 Hypervisor**, and **Type 2 Hypervisor**.
* Covers **Programming Environment Virtualization**.
* Addresses **Virtualization Issues**.
* Discusses **CPU scheduling**, **I/O**, and **Storage Management** in virtualized environments.

### 15. Security & Protection
* Defines **What's security?** and the **security problem**.
* Identifies **Security Violation Categories**.
* Provides **Examples of attacks**.
* Outlines **Security Measure Levels**.
* Discusses **Program Threats** and the concept of **The Threat Continues**.
* Covers **System and Network Threats** like **Port scanning**, **Denial of Service (DoS)**, and **Man-in-the-middle attacks**.
* Explains **Security mechanisms** using **Cryptography as a Security Tool**.
* Delves into **Cryptography implementation**, **Authentication (MAC)**, and an **Encryption Example (TLS)**.
* Discusses **Passwords** and **Firewalls**.
* Explores **Principles of Protection**, including **Protection Rings**, **Sandboxing**, **System integrity protection (SIP)**, and **Code signing**.

### 16. I/O Hardware
* Introduces **SCSI – Daisy Chain**.
* Examines **I/O strategies**: **Polling** and **Interrupts**, and associated **Latency**.
* Covers **Direct Memory Access (DMA)**.
* Discusses the **Application I/O Interface** and **Characteristics of I/O Devices**.
* Further explores **I/O strategies** such as **Nonblocking and Asynchronous I/O**.
