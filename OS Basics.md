## OPERATING SYSTEM BASICS

# What is kernel?

Kernel (core) is the fundamental component of the operating system. It is like a bridge between hardware and software. Basic processes such as  managing memory, managing processes and device control are handled by the kernel.

For example when a program is run, the kernel decides how this program will use the CPU and RAM.


# Difference between process and thread

A process is a running program. Every process has its own memory and system resources.

For instance, when a browser is run the operating system creates a new process.

Thread is the smallest unit in a process. A process can include more than one thread and these threads share the same memory.

For instance, in a browser playing a video,loading a page and user interaction could happen simultaneously by different threads.

So,basically:
-Processes have separate memory space, threads share the memory.
-Processes are heavier than threads.
-Communication between processes is slower.


# Memory Management

Memory management is the mechanism that ensures the operating system's effective use of memory. Enough space is reserved for every program and prevents them from affecting each other. 
 
How is memory managed?
-Operating system allocates memory to processes.
-It tracks memory usage.
-IT releases unused memory.

Virtual Memory

When RAM is insufficient, virtual memory allows the system to use disk space as an extension of RAM.

When RAM is full:
RAM -> Disk (Swap)

It prevents the system from crashing but could decrease the system performance.

# CPU Scheduling

CPU scheduling is the algorithm that decides which process will use the CPU and for how long.

-It allows the effective use of the CPU.
-Increases system performance.
-Provides fairness between processes.

Scheduling Algorithms

1. FCFS (First Come First Serve)
- The first process runs first.
- Easy but waiting time can be longer. 

2. SJF (Shortest Job First)
- The shortest job is run first.
- More efficient but it is hard to predict.

3. Round Robin (RR)
- Every process has its own time slice.
- It is a fair and common way. 

