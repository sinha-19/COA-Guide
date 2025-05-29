# 08. Cache Memory and Virtual Memory

---

## What is Cache Memory?

**Cache memory** is a small, high-speed memory located close to the CPU. It stores frequently accessed data and instructions to speed up processing by reducing the average time to access memory.

---

## Types and Levels of Cache

- **L1 Cache:** Closest to CPU core, smallest (32KB–128KB), fastest.
- **L2 Cache:** Larger (256KB–2MB), slightly slower, shared by cores or per-core.
- **L3 Cache:** Even larger (2MB–64MB), shared across all CPU cores, slower than L1/L2 but faster than main memory.

---

## Cache Mapping Techniques

- **Direct Mapped Cache:** Each block of main memory maps to exactly one cache line.
    - Simple, fast, but prone to conflicts.
- **Fully Associative Cache:** Any block can go into any cache line.
    - Flexible, reduces conflicts, but costly hardware.
- **Set Associative Cache:** Cache is divided into sets; each block maps to a set, and can go into any line in the set.
    - N-way set associative (common in modern CPUs).

---

## Cache Operations

- **Read Hit:** Data found in cache.
- **Read Miss:** Data not in cache; fetch from lower memory, update cache.
- **Write Hit/Miss:** Write policies determine behavior (write-back, write-through).

---

## Cache Replacement Policies

- **LRU (Least Recently Used)**
- **FIFO (First In, First Out)**
- **Random**
- **LFU (Least Frequently Used)**

---

## Cache Performance Metrics

- **Hit Rate:** % of accesses found in cache.
- **Miss Rate:** % not found (Miss = 1 – Hit).
- **Miss Penalty:** Extra time to fetch from lower memory.

---

## Write Policies

- **Write-Through:** Data written to both cache and main memory (simpler, more traffic).
- **Write-Back:** Data written to cache only, written to memory when block is replaced (faster, more complex).

---

## Virtual Memory

**Virtual memory** allows programs to use more memory than physically available by using disk storage as an extension of RAM.

- **Paging:** Memory is divided into fixed-size pages (commonly 4KB).
- **Page Table:** Maps virtual addresses to physical addresses.
- **TLB (Translation Lookaside Buffer):** Fast cache for page table entries.
- **Page Fault:** Occurs when data is not in physical memory; triggers disk access.

---

## Page Replacement Algorithms

- **FIFO**
- **LRU**
- **Optimal (theoretical, not practical)**
- **Clock (Second Chance)**

---

## Advantages of Virtual Memory

- Enables large address spaces.
- Simplifies memory management and protection.
- Isolates processes for security.

---

## Interview Patterns

- Calculate cache hit/miss rates with given access patterns.
- Explain difference between direct-mapped and set-associative cache.
- Describe virtual to physical address translation.
- Illustrate page replacement with LRU or FIFO.
- Explain TLB and its role.

---

## Common Pitfalls

- Forgetting that write-back caches must track “dirty” blocks.
- Overlooking TLB misses in performance calculations.
- Confusing cache miss with page fault.

---

## Exercises

1. Compute the number of sets in a 32KB 4-way set-associative cache with 64B block size.
2. Simulate LRU page replacement for a sequence of page accesses.
3. Explain how write-back and write-through caches differ.
4. Draw a diagram showing the memory hierarchy including TLB, cache, main memory, and disk.
5. Describe the steps taken when a page fault occurs.

---

## Key Interview Questions

- What is the purpose of cache memory?
- How does a set-associative cache work?
- What is a TLB, and why is it important?
- Explain page replacement and page fault handling.
- What are the trade-offs between write-back and write-through?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 8-9](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 5](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)
- [GeeksforGeeks - Cache Memory](https://www.geeksforgeeks.org/cache-memory-in-computer-organization/)
- [Wikipedia: Virtual Memory](https://en.wikipedia.org/wiki/Virtual_memory)

---
