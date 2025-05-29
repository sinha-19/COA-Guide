# 11. RISC vs. CISC Architecture

---

## What is RISC?

**RISC (Reduced Instruction Set Computer)** is a CPU design philosophy that uses a small set of simple, general instructions, typically of fixed length, to achieve high performance through pipelining and parallelism.

---

## What is CISC?

**CISC (Complex Instruction Set Computer)** uses a larger set of more complex instructions, often variable in length, which can execute multi-step operations in a single instruction.

---

## Features of RISC

- Fewer instructions (typically 32–64)
- Simple, fixed-length instruction formats
- Single-cycle execution for most instructions
- Large number of general-purpose registers
- Load/store architecture (memory accessed only by load/store)
- Emphasizes compiler optimization

**Examples:** ARM, MIPS, SPARC, PowerPC

---

## Features of CISC

- Large instruction set (100+)
- Variable-length instructions
- Instructions can perform complex tasks (e.g., string copy)
- Fewer registers, more use of memory
- Emphasizes microprogramming for complex instructions

**Examples:** x86, VAX, 68000

---

## RISC vs. CISC: A Comparison

| Feature             | RISC                        | CISC                    |
|---------------------|-----------------------------|-------------------------|
| Instruction Set     | Small, simple               | Large, complex          |
| Instruction Length  | Fixed                       | Variable                |
| Execution Time      | Usually single-cycle        | Multi-cycle possible    |
| Registers           | Many                        | Few                     |
| Memory Access       | Load/store only             | Memory access in many   |
| Pipelining          | Easy                        | Harder                  |
| Code Size           | Larger                      | Smaller                 |
| Hardware Complexity | Lower                       | Higher                  |

---

## Modern Trends

- **x86 (CISC) CPUs internally use RISC-like micro-operations.**
- RISC-V: Open-source RISC ISA gaining popularity.
- ARM dominates mobile and embedded, x86 leads desktops/servers.

---

## Advantages and Disadvantages

**RISC Advantages:**
- Easier pipelining
- Lower power consumption
- Predictable performance

**CISC Advantages:**
- Compact code (smaller binaries)
- Fewer instructions per program

**Disadvantages:**  
- RISC: Larger programs, increased memory traffic  
- CISC: Complex hardware, harder pipelining

---

## Interview Patterns

- Compare RISC vs. CISC by features and examples.
- Explain why pipelining is easier in RISC.
- Discuss the evolution of x86 towards RISC-like internals.
- Map assembly code between RISC and CISC.

---

## Common Pitfalls

- Believing all modern CPUs are purely RISC or CISC (most are hybrids).
- Ignoring the role of compilers in RISC performance.
- Overlooking micro-operations in CISC implementations.

---

## Exercises

1. List main differences between RISC and CISC.
2. Write equivalent RISC and CISC assembly code for a simple arithmetic operation.
3. Explain how micro-operations bridge RISC and CISC.
4. Draw a block diagram of a RISC datapath.
5. Research and summarize the RISC-V ISA.

---

## Key Interview Questions

- What is the difference between RISC and CISC?
- Why is RISC architecture well-suited for pipelining?
- How do modern x86 CPUs use RISC ideas?
- What are the trade-offs between hardware and software complexity in RISC/CISC?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 10](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - RISC vs CISC](https://www.geeksforgeeks.org/difference-between-risc-and-cisc/)
- [Wikipedia: RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer)
- [Wikipedia: CISC](https://en.wikipedia.org/wiki/Complex_instruction_set_computer)
- [Patterson & Hennessy, Computer Organization and Design](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
