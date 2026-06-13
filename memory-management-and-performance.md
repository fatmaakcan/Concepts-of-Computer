## Memory Management & Performance

### 1. Stack vs Heap Architecture
During program execution, system memory (RAM) is logically divided into two primary areas: **Stack** and **Heap**.

**Stack**
- The stack is a very fast memory region that operates on a last-in, first-out (LIFO) principle. 
- Its size is determined at compile time and is static. 
- Because it is automatically managed by the CPU, the memory is automatically cleaned up when a function finishes. 
- Local variables, function calls, and primitive data types are stored here.

**Heap**
- The heap is a distributed, dynamic, and flexible memory structure. 
- Its size grows or shrinks as needed during program runtime. 
- It is slower than the stack because it requires searching for free memory and performing addressing. 
- While its management is done automatically with the Garbage Collector in languages ​​like Java or Python, it is done manually by the programmer in C or C++. Large objects, dynamic arrays, and global data are stored here.

### 2. How Garbage Collection (GC) Works
Garbage Collection is an automated memory management process that clears objects in the Heap memory that are **no longer referenced** by any part of the application.

Main operational algorithms include:
1. **Reference Counting:** Tracks how many pointers point to an object. When the count hits 0, the memory is immediately reclaimed (e.g., Python).
2. **Mark and Sweep:** Starts from GC Roots and traverses the memory tree. Active objects are "marked". Unmarked (unreachable) objects are "swept" away in the next phase (e.g., Java / JVM).



### 3. What is a Memory Leak and How Does It Occur?
A Memory Leak occurs when an application allocates memory from the Heap but **fails to release it back to the operating system** after use. Over time, the accumulated leaked memory degrades system performance and eventually leads to an **Out of Memory (OOM)** crash.

**Common Causes:**
* **In Managed Languages (C/C++):** Forgetting to pair malloc() / new with free() / delete.
* **In Automatic GC Languages (Java/Python):** Unintentional lingering references like unused static fields, unclosed system streams (files, databases), or abandoned event listeners preventing GC from purging the object.
