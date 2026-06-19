# Concurrency & Parallel Programming

## 1. Concurrency vs. Parallelism
Concurrency is about structure, whereas Parallelism is about execution.

* **Concurrency:** It is about the progression of multiple tasks within the same time frame. It does not strictly mean tasks run at the exact same moment. On a single-core CPU, the operating system switches between tasks incredibly fast (context switching), creating the illusion that they are running simultaneously.
    
* **Parallelism:** It is the physical execution of multiple tasks at the exact same time across multiple cores or processors. Parallelism strictly requires multi-core or multi-processor hardware.
    
---

## 2. What is a Race Condition?
A Race Condition is a synchronization anomaly that occurs when multiple threads attempt to access the same shared resource simultaneously, and at least one of them modifies (writes to) the data. 

In this scenario, the final output of the program becomes dependent on the arbitrary scheduling and execution order of the threads by the CPU. The outcome becomes completely non-deterministic and unpredictable.

---

## 3. Core Concepts: Mutex, Semaphore, and Lock
To prevent race conditions, we must synchronize thread access to shared resources. The primary mechanisms used for this are:

### Lock
The most fundamental synchronization concept. Before entering a critical section of code, a thread acquires the lock. Once the execution is done, it releases (unlocks) it. While locked, no other thread can enter that section; they must wait in line.

### Mutex (Mutual Exclusion)
Essentially a locking mechanism, but it is an object managed at the operating system level. Its most defining feature is ownership.
* The unique thread that locked the Mutex is the only one authorized to unlock it.
* It can only hold binary values: 0 or 1 (Locked or Unlocked).

### Semaphore (Signaling Mechanism)
A counter-based system used to allow a maximum of N threads to access a specific resource simultaneously.
* **Counting Semaphore:** It maintains an internal counter. For instance, if the counter is set to 3, up to 3 threads can use that resource concurrently. A 4th thread must wait until one of the active threads releases its slot.
* **Binary Semaphore:** Its counter can only be 0 or 1. Logically similar to a Mutex, but its key difference is that it lacks ownership. A Binary Semaphore locked by one thread can be unlocked (released) by a signal from a completely different thread.

