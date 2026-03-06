# Computer Sciences Concepts

## 1. CPU(Central Processing Unit)
CPU is the brain of the computer. It is the responsible for running  programs, mathematical and logical operations. All commands are processed by the CPU. 

For instance, when we use a for loop, loop control and processes are conducted by the CPU.

## How the CPU works?
1.Fetch->The command is fetched from memory.
2.Decode->The command is decoded.
3.Execute->The command is executed.

This loop occurs billions of times per second.

## Fundamentals of the CPU
-ALU(Arithmetic Logic Unit)= Performs mathematical and logical operations.
-Control Unit= Controls the flow of intructions.
-Registers= Very fast temporary memory.

## Factors that affect the CPU's Performance
-Clock Speed(GHz)
-Number of Cores
-Number of Threads
-Cache memory

For example, an 8-core processor is more effective than a 2-core processor in multitasking.

## 2. RAM (Random Access Memory)
RAM is the temporary memory of the computer. Running programs and active data are held here, and when the computer is powered off, the RAM is cleared.

For example, when VS Code is open and a Java program is running, data are held in RAM.

## How the RAM works?
When the CPU makes a process, data are held in RAM not on the CPU;because RAM is faster than the disk.

Disk-> RAM->CPU (spped order)

## Types of RAM
-DDR3
-DDR4
-DDR5

New generation RAMs present higher speed and bandwidth.

## What happens if RAM is inadequate?
-The computer becomes slow.
-Disk swap is used.
-Applications freeze.

For instance, it gets hard to use a browser with 4GB RAM.

##  3.Disk (Hardware Unit)
Disk is the component where data are permanently stored. The operating system, programs and files are stored here.

## Types of Disk
1. HDD(Hard Disk Drive)
-Mechanical Structure
-Slower
-Cheaper

2. SSD (Solid State Drive)
-No mechanical structure
-Faster
-More expensive

SSD could be 5-10 times faster than HDD.

## Factors that affect disk performance
-Read/Write Speed
-IOPS
-Connection Type(SATA,NVMe)

### The Relation between CPU, RAM and Disk
Disk keeps data.
RAM keeps data temporarily.
CPU processes.

If one of them is weak, system performance decreases.

For example:
-Stronger CPU + low RAM->bottleneck
-HDD instead of SSD-> The system works slowly.

As a conclusion, CPU, RAM and disk are the fundamental components of computer performance. In modern software development, it is important that these components are balanced. Especially, RAM capacity and the use of an SSD make a big difference for software developers.