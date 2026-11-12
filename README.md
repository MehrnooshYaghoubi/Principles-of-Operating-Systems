# Principles of Operating Systems — Study Guide

Lecture slides for the course, one folder per lecture. Each folder holds a single PDF:

```
NN-Lecture-Name/NN-Lecture-Name.pdf
```


Work through the folders in numbered order — each lecture assumes the one before it.
Slides are in Persian; every technical term appears with its English equivalent, so the
English textbook chapters listed below line up directly with the slides.

| # | Lecture | Slides | Textbook |
|---|---------|-------:|----------|
| 0 | [Course Overview](00-Course-Overview) | 4 | — |
| 1 | [Introduction](01-Introduction) | 11 | Ch. 1 |
| 2 | [Computer System Architecture](02-Computer-System-Architecture) | 11 | Ch. 1 |
| 3 | [Operating System Structures](03-Operating-System-Structures) | 3 | Ch. 2 |
| 4 | [Operating System Services](04-Operating-System-Services) | 13 | Ch. 2 |
| 5 | [I/O Management](05-IO-Management) | 15 | Ch. 12 |
| 6 | [Processes](06-Processes) | 27 | Ch. 3 |
| 7 | [Scheduling Queues](07-Scheduling-Queues) | 16 | Ch. 3 |
| 8 | [Threads](08-Threads) | 19 | Ch. 4 |
| 9 | [Scheduling Algorithms](09-Scheduling-Algorithms) | 64 | Ch. 5 |
| 10 | [Concurrency Management](10-Concurrency-Management) | 48 | Ch. 6–7 |
| 11 | [Deadlock](11-Deadlock) | 20 | Ch. 8 |
| 12 | [Memory Management](12-Memory-Management) | 28 | Ch. 9 |

Textbook = Silberschatz, Galvin, Gagne, _Operating System Concepts_, 10th edition —
in `Reference-Books/`, along with Stallings, _Operating Systems: Internals and Design
Principles_, 7th edition.

---

## What each lecture covers

### 0 — Course Overview
Course outline, reference list, grading breakdown.

### 1 — Introduction
What an operating system is. The families you will meet throughout the course: Unix,
Linux, Windows, macOS. The role of the OS in a computer system, built up in layers —
user, application software, operating system, hardware. Registers and the shared bus.

### 2 — Computer System Architecture
The classifications a system can fall into: single-user and multi-user; single-processor
and multiprocessor; single-tasking and multi-tasking; single-programming and
multiprogramming; time-sharing; standalone, clustered, real-time, and peer-to-peer
systems.

### 3 — Operating System Structures
How an operating system is organised internally.

### 4 — Operating System Services
The services the OS provides, one per slide: I/O device management, memory management
(RAM), CPU scheduling, process management, concurrency management, file management,
communication management, error detection, protection and security, and accounting.
This lecture is the map of the rest of the course — lectures 5 through 12 each expand
one of these services.

### 5 — I/O Management
Input/output device management in depth.

### 6 — Processes
What a process is. Process creation and termination. Special process states. The Process
Control Block (PCB) and what it stores. Process states, then the five-state model.

### 7 — Scheduling Queues
The scheduling queues, including the waiting/blocked queue. Context switching and its
cost. Where scheduling algorithms fit. The dispatcher. Swapping, and the seven-state
process model it leads to.

### 8 — Threads
Why threads exist and where a thread sits inside a process. Kinds of threads. The
multi-threading models: many-to-one, one-to-one, many-to-many, two-level. Communication
between threads, and the programming challenges multithreading introduces.

### 9 — Scheduling Algorithms
The longest lecture, and the most exercise-heavy. Preemptive versus non-preemptive
scheduling, and the CPU scheduling criteria used to compare algorithms. Job scheduling
algorithms, then CPU scheduling algorithms — non-preemptive first, then preemptive.
Roughly half the slides are worked problems: 21 questions, 14 exercise slides, and 2
past national-exam (کنکور) questions.

### 10 — Concurrency Management
Why concurrency causes problems, shown through a worked example. Race conditions. The
critical section, with software solutions developed step by step. Hardware support for
concurrency: memory barriers, hardware instructions, atomic variables. Then the
synchronisation tools — mutex locks, semaphores, monitors. Includes 5 past national-exam
questions and 5 exercise slides.

### 11 — Deadlock
The characteristics of deadlock. Resource-allocation graphs, with a worked example.
Deadlock prevention. Deadlock avoidance: safe states, and the Banker's Algorithm over
six slides.

### 12 — Memory Management
The role of main memory and the memory-stall problem. Memory protection, the base-and-
limit scheme, hardware protection and address translation, and how a trap works. Address
binding: the kinds of addresses at each stage, binding times, logical versus physical
addresses. The MMU. Dynamic loading. Contiguous memory allocation, allocation
strategies, and fragmentation. Finally, paging and its basic method.

---

## How to use the practice slides

Lectures 6 through 10 interleave worked problems with the material. Three kinds appear:

- **سوال** — a question on the material just presented; try it before reading on
- **تمرین / تمرینات** — exercises, usually several per slide
- **سوال کنکور** — a question from the Iranian national graduate entrance exam

Lectures 9 and 10 carry almost all of them. If you are revising for an exam, those two
folders are where the practice is.
