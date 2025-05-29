# 10. Pipelining and Hazards

---

## What is Pipelining?

**Pipelining** is a technique that breaks instruction execution into discrete stages, allowing multiple instructions to be processed simultaneously and increasing CPU throughput.

---

## Pipeline Stages (Classic 5-Stage RISC Pipeline)

1. **IF (Instruction Fetch):** Get instruction from memory.
2. **ID (Instruction Decode):** Decode instruction, read registers.
3. **EX (Execute):** Perform ALU operation or calculate address.
4. **MEM (Memory Access):** Access data memory (load/store).
5. **WB (Write Back):** Write result to register.

---

## Pipelining Example

- While instruction 1 is in EX, instruction 2 can be in ID, instruction 3 in IF, etc.
- Increases instruction throughput (instructions per cycle), but not latency of a single instruction.

---

## Pipeline Performance

- **Throughput:** Number of instructions completed per unit time.
- **Speedup:** Ideal speedup = number of stages (rare in practice due to hazards).
- **Pipeline Fill and Drain:** Pipeline must fill before max throughput is reached.

---

## Hazards in Pipelining

### 1. Structural Hazards

- Caused by hardware resource conflicts (e.g., single memory for instructions and data).

### 2. Data Hazards

- **RAW (Read After Write):** Instruction needs a value before previous instruction writes it.
- **WAR (Write After Read):** Rare in simple pipelines.
- **WAW (Write After Write):** Rare in simple pipelines.

**Solution:** Forwarding (bypassing), pipeline stalls (bubbles).

### 3. Control Hazards

- Due to branches and jumps; pipeline may fetch wrong instruction.

**Solution:** Branch prediction, delayed branching, pipeline flushing.

---

## Pipeline Stalls and Bubbles

- **Stall:** CPU waits for hazard to clear.
- **Bubble:** No operation is inserted to delay pipeline progression.

---

## Advanced Pipelining Concepts

- **Superpipelining:** More stages, higher clock rate.
- **Superscalar Execution:** Multiple pipelines, issue multiple instructions per cycle.
- **Dynamic Scheduling:** Out-of-order execution to reduce stalls.

---

## Interview Patterns

- Draw the pipeline diagram for a sequence of instructions.
- Identify and resolve data hazards in instruction streams.
- Explain branch prediction and its importance.
- Calculate pipeline speedup with and without stalls.

---

## Common Pitfalls

- Assuming pipelining always gives linear speedup.
- Not recognizing hazards in code.
- Ignoring the impact of pipeline flushes after branches.

---

## Exercises

1. Given instruction sequence, highlight all hazards and show pipeline execution.
2. Explain how forwarding reduces data hazards.
3. Describe the impact of branch prediction accuracy on pipeline performance.
4. Calculate the throughput of a 5-stage pipeline with a 20% stall rate.
5. Compare superscalar and superpipelined architectures.

---

## Key Interview Questions

- What are the three types of pipeline hazards?
- How do you resolve data hazards in a pipeline?
- Why does pipelining improve throughput but not latency?
- Describe branch prediction techniques.

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 14](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Pipelining in Computer Architecture](https://www.geeksforgeeks.org/pipelining-in-computer-architecture/)
- [Wikipedia: Instruction Pipelining](https://en.wikipedia.org/wiki/Instruction_pipelining)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 4-6](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
