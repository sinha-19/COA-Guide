# 07. Memory Hierarchy and Organization

---

## What is Memory Hierarchy?

Memory hierarchy is a layered structure of storage devices with varying speed, size, and cost. It enables fast average access to a large memory space at low cost.

---

## Levels of Memory Hierarchy

1. **Registers**: Fastest, smallest, inside CPU.
2. **Cache Memory**: Small, fast, sits between CPU and main memory.
3. **Main Memory (RAM)**: Medium speed, moderate size (volatile).
4. **Secondary Storage**: Hard Disk Drives (HDD), Solid State Drives (SSD) – large, slow, non-volatile.
5. **Tertiary Storage**: Magnetic tapes, optical disks – archival, very slow.

---

## Principle of Locality

- **Temporal Locality**: Recently accessed data is likely to be accessed again soon.
- **Spatial Locality**: Data near recently accessed locations is likely to be accessed soon.

---

## Cache Memory

- **L1, L2, L3 Cache**: Levels of cache, with L1 closest and fastest to CPU.
- **Cache Line/Block**: Unit of data transfer between cache and memory.
- **Associativity**: Direct-mapped, set-associative, fully associative.

---

## Main Memory Organization

- **RAM**: Volatile, used for primary storage of programs/data.
    - **DRAM**: Dynamic, needs refreshing.
    - **SRAM**: Static, faster, used for cache.
- **ROM**: Non-volatile, stores firmware.

---

## Memory Addressing

- **Byte Addressable**: Each address refers to a byte.
- **Word Addressable**: Each address refers to a word (multiple bytes).
- **Interleaving**: Spreads memory access across modules for speed.

---

## Memory Management

- **Paging**: Fixed-size blocks, simplifies allocation.
- **Segmentation**: Variable-size blocks, reflects program structure.
- **Virtual Memory**: Uses disk as extension of RAM, managed by OS.

---

## Error Detection and Correction

- **Parity Bits**: Simple error detection.
- **ECC (Error Correction Code)**: Corrects single-bit errors.

---

## Memory Access Time & Bandwidth

- **Access Time**: Time to read/write memory.
- **Cycle Time**: Time before next access can begin.
- **Bandwidth**: Rate of data transfer.

---

## Interview Patterns

- Draw a diagram of the memory hierarchy.
- Explain the principle of locality.
- Compare DRAM and SRAM.
- Describe the function of cache memory.
- Explain the difference between paging and segmentation.

---

## Common Pitfalls

- Ignoring the impact of cache and locality on performance.
- Confusing volatile and non-volatile memory types.
- Overlooking memory management techniques in system design.

---

## Exercises

1. Draw and label the memory hierarchy pyramid.
2. Explain how virtual memory works.
3. Compare L1, L2, and L3 caches.
4. Describe the benefits of associativity in cache design.
5. Write short notes on DRAM vs. SRAM.

---

## Key Interview Questions

- What is the principle of locality and why is it important?
- Describe the structure and function of cache memory.
- How does virtual memory enable large address spaces?
- What are the differences between paging and segmentation?
- Why is memory hierarchy used in computer systems?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 8](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Memory Hierarchy](https://www.geeksforgeeks.org/memory-hierarchy-in-computer-architecture/)
- [Wikipedia: Memory Hierarchy](https://en.wikipedia.org/wiki/Memory_hierarchy)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 5](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
