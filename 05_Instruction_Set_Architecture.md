# 05. Instruction Set Architecture (ISA)

---

## What is an Instruction Set Architecture?

An **Instruction Set Architecture (ISA)** is the interface between the computer’s hardware and its software. It defines the set of instructions that a processor can execute, the data types, addressing modes, registers, and hardware support for software.

---

## Components of ISA

- **Instruction Set:** List of all operations the processor can perform (e.g., ADD, SUB, MOV).
- **Register Set:** Number and type of registers available.
- **Data Types:** Supported types (integer, float, char, etc.).
- **Addressing Modes:** Ways to specify operands for instructions.
- **Instruction Formats:** Layout of bits in an instruction.
- **Memory Model:** How memory is accessed and organized.

---

## Types of Instructions

- **Data Movement:** MOV, LOAD, STORE, PUSH, POP
- **Arithmetic:** ADD, SUB, MUL, DIV
- **Logical:** AND, OR, XOR, NOT
- **Control Flow:** JMP, CALL, RET, JZ, JNZ
- **Input/Output:** IN, OUT

---

## Addressing Modes

- **Immediate:** Operand is part of instruction (e.g., MOV R1, #5)
- **Register:** Operand is in a register (e.g., MOV R1, R2)
- **Direct:** Address is specified directly (e.g., MOV R1, 1000)
- **Indirect:** Address is in a register (e.g., MOV R1, [R2])
- **Indexed:** Base address plus offset (e.g., MOV R1, [R2 + 4])
- **Relative:** Used in branching (e.g., JMP +4)

---

## Instruction Format

- **Opcode:** Operation code specifying the operation.
- **Operands:** Registers or memory locations involved.
- **Mode bits:** Indicate addressing mode.

Example (32-bit instruction):  
| Opcode | Dest | Src1 | Src2 |  
|--------|------|------|------|  
|  8 bits|  8   |  8   |  8   |

---

## Types of ISAs

- **CISC (Complex Instruction Set Computer):** Many instructions, complex addressing modes (e.g., x86).
- **RISC (Reduced Instruction Set Computer):** Fewer, simpler instructions, fixed length (e.g., ARM, MIPS).

---

## Examples of Popular ISAs

- **x86:** CISC, variable-length instructions, used in most PCs.
- **ARM:** RISC, fixed-length, widely used in mobile.
- **MIPS:** RISC, educational and embedded systems.
- **SPARC, PowerPC:** Other RISC architectures.

---

## Role of ISA in Software Development

- Compilers generate machine code based on ISA.
- OS and system software depend on ISA for context switching, interrupt handling.

---

## Compatibility and Evolution

- **Backward Compatibility:** New CPUs often support old ISAs.
- **Extensions:** SSE, AVX in x86 for multimedia, vector processing.

---

## Micro-operations and Micro-instructions

- Complex instructions may be decomposed into simpler micro-operations internally.

---

## Interview Patterns

- Decode and execute a given instruction (e.g., MOV R1, [R2]).
- List and explain addressing modes with examples.
- Compare RISC and CISC ISAs.
- Design a simple instruction format for a hypothetical CPU.
- Map assembly instructions to micro-operations.

---

## Common Pitfalls

- Confusing addressing modes.
- Overlooking instruction size and alignment issues.
- Not understanding the implications of fixed vs. variable-length instructions.

---

## Exercises

1. List all addressing modes and give an example of each.
2. Convert a simple C statement to pseudo-assembly (ISA-specific).
3. Explain how a compiler uses the ISA.
4. Given a binary instruction, decode its fields.
5. Contrast RISC and CISC with real-world architectures.

---

## Key Interview Questions

- What is an ISA? Why is it important?
- Describe the addressing modes used by x86/ARM.
- What advantages do RISC architectures offer?
- How does the ISA affect compiler design?
- What is the difference between instruction format and instruction set?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 5](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 2](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)
- [GeeksforGeeks - Instruction Set Architecture](https://www.geeksforgeeks.org/instruction-set-architecture/)
- [Wikipedia: Instruction set architecture](https://en.wikipedia.org/wiki/Instruction_set_architecture)

---
