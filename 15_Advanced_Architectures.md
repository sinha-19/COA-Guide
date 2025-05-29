# 15. Advanced Architectures (Superscalar, VLIW, DSP, GPU)

---

## Superscalar Architecture

- **Definition:** Processor that can issue multiple instructions per clock cycle.
- **Multiple execution units:** ALU, FPU, load/store.
- **Instruction dispatch and reservation stations** enable parallel execution.
- **Out-of-order execution:** Instructions may complete out of order to maximize utilization.

---

## VLIW (Very Long Instruction Word)

- **Definition:** Multiple operations encoded in a single, long instruction.
- **Relies on compiler:** Compiler schedules instructions to avoid hazards.
- **Used in embedded/DSP processors** (e.g., Intel Itanium, TI DSPs).

---

## SIMD (Single Instruction, Multiple Data)

- **Definition:** One instruction operates on multiple data elements (vectors).
- **Applications:** Multimedia, scientific computing.
- **Examples:** SSE, AVX (x86), NEON (ARM).

---

## MIMD (Multiple Instruction, Multiple Data)

- **Definition:** Multiple instruction streams, each on different data (multicore, clusters).

---

## Digital Signal Processors (DSP)

- Specialized for real-time signal processing (audio, video, radar).
- Features: Multiply-accumulate (MAC) units, circular buffers, zero-overhead loops.

---

## Graphics Processing Units (GPU)

- Highly parallel SIMD processors for graphics and general-purpose compute (GPGPU).
- Thousands of cores, optimized for throughput.
- Programming models: CUDA, OpenCL.

---

## Reconfigurable Architectures

- **FPGA (Field Programmable Gate Array):** Hardware logic can be reprogrammed.
- Used in prototyping, custom accelerators.

---

## Network-on-Chip (NoC)

- Multiple cores/processors interconnected via on-chip network.
- Improves scalability, bandwidth.

---

## Heterogeneous Computing

- Systems with CPUs, GPUs, DSPs, FPGAs working together.
- Workload assigned to best-suited processor.

---

## Quantum and Neuromorphic Architectures (Intro)

- **Quantum computers:** Qubits, superposition, entanglement; not mainstream yet.
- **Neuromorphic:** Brain-inspired, implements neural networks in hardware.

---

## Interview Patterns

- Explain superscalar and VLIW differences.
- Discuss SIMD and its applications.
- Compare CPU and GPU architectures.
- Describe use cases for FPGAs.

---

## Common Pitfalls

- Assuming all instruction-level parallelism is exploited automatically.
- Overlooking compiler role in VLIW.
- Underestimating memory bottlenecks in highly parallel systems.

---

## Exercises

1. Draw a superscalar datapath showing multiple pipelines.
2. Write a simple SIMD code example.
3. Explain out-of-order execution in modern CPUs.
4. Compare DSP and general-purpose CPU features.
5. Research a modern GPU and summarize its architecture.

---

## Key Interview Questions

- What is a superscalar processor?
- How does VLIW differ from superscalar?
- Why are GPUs better for parallel workloads?
- What is the role of FPGAs in modern systems?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 17](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Advanced Architectures](https://www.geeksforgeeks.org/advanced-computer-architecture/)
- [Wikipedia: Superscalar processor](https://en.wikipedia.org/wiki/Superscalar_processor)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 7](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
