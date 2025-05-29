# 06. Addressing Modes and Instruction Cycle

---

## What are Addressing Modes?

Addressing modes define how operands are specified in instructions. They are essential for flexible data access and efficient instruction execution.

---

## Common Addressing Modes

1. **Immediate Addressing**  
   Operand is part of the instruction.  
   Example: `MOV R1, #10` (move 10 to R1)

2. **Register Addressing**  
   Operand is in a register.  
   Example: `MOV R1, R2` (copy R2 to R1)

3. **Direct Addressing**  
   Memory address is specified directly in the instruction.  
   Example: `MOV R1, [1000]`

4. **Indirect Addressing**  
   Instruction specifies a register/memory location that contains the address.  
   Example: `MOV R1, [R2]`

5. **Indexed Addressing**  
   Address = base register + offset.  
   Example: `MOV R1, [R2 + 5]`

6. **Relative Addressing**  
   Used in branches; PC + offset.  
   Example: `JMP +4`

7. **Base Register Addressing**  
   Similar to indexed, but base is often frame pointer (used in stack frames).

---

## Importance of Addressing Modes

- Allow compact and flexible code.
- Enable efficient access to arrays, structures, and pointers.
- Affect instruction complexity and CPU design.

---

## Instruction Cycle

The sequence of operations CPU performs to execute an instruction.

### Phases of the Instruction Cycle

1. **Fetch**: Get the instruction from memory (using PC).
2. **Decode**: Interpret the opcode and addressing mode.
3. **Fetch Operands**: Get the required data (register or memory).
4. **Execute**: Perform the operation (ALU, memory, I/O).
5. **Write Back**: Store result in destination register/memory.
6. **Update PC**: Point to the next instruction.

---

## Micro-operations in the Cycle

- **MAR ← PC**: Memory Address Register gets address from PC.
- **MDR ← Memory[MAR]**: Memory Data Register fetches instruction.
- **IR ← MDR**: Instruction Register gets instruction.
- **Decode IR**: Control unit decodes instruction and addressing mode.
- **ALU ← Operands**: ALU executes arithmetic/logical operation.
- **Result → Destination**: Result written back.

---

## Interrupts in the Cycle

- **Interrupt Check**: After each instruction, CPU checks for interrupts.
- **Interrupt Service Routine (ISR)**: Special handling routine if interrupt is pending.

---

## Pipelining and the Instruction Cycle

- Stages of the cycle are overlapped for higher throughput.
- Leads to potential hazards (structural, data, control).

---

## Interview Patterns

- Identify addressing mode for given instructions.
- Draw the sequence of steps in the instruction cycle.
- Explain the role of PC, MAR, MDR, IR.
- Discuss the impact of addressing modes on instruction length and execution.

---

## Common Pitfalls

- Confusing register and direct modes.
- Not handling indirect and indexed addressing correctly.
- Overlooking the importance of updating PC.

---

## Exercises

1. List and explain all addressing modes with an instruction example.
2. Trace the instruction cycle for `ADD R1, [R2+4]`.
3. Explain how indexed addressing is used in array operations.
4. What happens if an interrupt occurs during instruction execution?
5. Draw a timing diagram for the instruction cycle.

---

## Key Interview Questions

- What is the purpose of different addressing modes?
- Describe the steps in the instruction cycle.
- How does the CPU fetch and execute instructions?
- How does indexed addressing help in array processing?
- What role does the program counter play?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 7](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Addressing Modes](https://www.geeksforgeeks.org/addressing-modes-in-computer-architecture/)
- [Wikipedia: Addressing Mode](https://en.wikipedia.org/wiki/Addressing_mode)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 4](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
