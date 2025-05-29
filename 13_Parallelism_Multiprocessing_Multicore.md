# 13. Parallelism, Multiprocessing, and Multicore

---

## What is Parallelism?

**Parallelism** is the simultaneous execution of multiple computations to increase performance and resource utilization.

---

## Types of Parallelism

- **Bit-level Parallelism:** Processing multiple bits in one instruction.
- **Instruction-level Parallelism (ILP):** Overlapping execution of instructions (pipelining, superscalar).
- **Thread-level Parallelism (TLP):** Multiple threads run in parallel (multithreading).
- **Process-level Parallelism:** Multiple independent processes execute simultaneously.

---

## Multiprocessing Systems

- **Symmetric Multiprocessing (SMP):** All CPUs share a single memory and OS (common in servers, desktops).
- **Asymmetric Multiprocessing (AMP):** CPUs assigned specific tasks or master/slave roles.
- **Massively Parallel Processing (MPP):** Many processors with their own memory, often in clusters.

---

## Multicore Processors

- **Multicore:** Single chip with multiple CPU cores.
    - Each core can execute separate threads/processes.
    - Shared L2/L3 cache, shared or private L1.
    - Improves throughput and energy efficiency.

---

## Shared vs. Distributed Memory

- **Shared Memory:** All processors access a common memory space.
- **Distributed Memory:** Each processor has its own memory, communication via messages.

---

## Interconnection Networks

- **Bus:** Simple, shared communication line.
- **Crossbar Switch:** Direct connection, high speed, expensive.
- **Multistage Networks:** Scalable, used in large systems (e.g., hypercube, mesh).

---

## Parallel Programming Models

- **Shared Memory:** Threads, OpenMP, Pthreads.
- **Distributed Memory:** MPI, message passing.
- **SIMD:** GPUs, vector processors.

---

## Synchronization and Consistency

- **Locks, Semaphores, Barriers:** Prevent race conditions.
- **Cache Coherence:** Ensures all CPUs see consistent memory values (MESI protocol).

---

## Flynn’s Taxonomy (Review)

- **SISD, SIMD, MISD, MIMD** – categorizes parallel architectures.

---

## Amdahl’s Law

- **Speedup = 1 / (S + (1–S)/N)**
    - S = Serial fraction, N = number of processors
    - Limits speedup due to non-parallelizable portions.

---

## Interview Patterns

- Compare multiprocessor and multicore systems.
- Explain cache coherence protocols.
- Discuss Amdahl’s Law and its implications.
- Draw diagrams of interconnection networks.

---

## Common Pitfalls

- Ignoring synchronization overhead.
- Assuming linear speedup from adding processors.
- Overlooking memory bandwidth limitations.

---

## Exercises

1. Derive speedup for various serial/parallel fractions using Amdahl’s Law.
2. Explain MESI cache coherence protocol.
3. Compare SMP and MPP architectures.
4. List advantages of multicore processors in mobile devices.
5. Write a parallel program using OpenMP or Pthreads.

---

## Key Interview Questions

- What are the advantages of multicore over multiprocessor systems?
- How does cache coherence work?
- Why is synchronization necessary in parallel systems?
- What limits the speedup in parallel computing?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 16](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Multiprocessing and Multicore](https://www.geeksforgeeks.org/multiprocessing-and-multicore-in-computer-architecture/)
- [Wikipedia: Multicore Processor](https://en.wikipedia.org/wiki/Multi-core_processor)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 7](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
