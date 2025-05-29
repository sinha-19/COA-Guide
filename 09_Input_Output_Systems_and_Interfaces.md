# 09. Input/Output Systems and Interfaces

---

## What are Input/Output Systems?

**Input/Output (I/O) systems** connect the CPU and memory to external devices (disks, keyboards, displays, networks, etc.), facilitating data exchange between the computer and the outside world.

---

## Types of I/O Devices

- **Input Devices:** Keyboard, mouse, scanner, microphone
- **Output Devices:** Monitor, printer, speakers
- **Storage Devices:** Hard drives, SSDs, USB drives
- **Communication Devices:** Network cards, Bluetooth, Wi-Fi

---

## I/O Techniques

1. **Programmed I/O**
   - CPU controls all I/O operations.
   - Polling: CPU repeatedly checks I/O status.
   - Simple but wastes CPU time.

2. **Interrupt-Driven I/O**
   - Device interrupts CPU when it’s ready.
   - CPU can execute other tasks while waiting.
   - Reduces CPU idle time.

3. **Direct Memory Access (DMA)**
   - DMA controller transfers data directly between memory and device.
   - CPU sets up transfer but is free during the data movement.
   - Essential for high-speed data transfer (disk, network).

---

## I/O Interface and Ports

- **I/O Interface:** Hardware that connects CPU and device, handles handshaking, buffering, error detection.
- **Ports:** Physical or logical connections (USB, serial, parallel).

---

## Bus Structure

- **Data Bus:** Carries data.
- **Address Bus:** Specifies memory/device locations.
- **Control Bus:** Carries control signals (read/write, interrupt, etc.).

---

## Synchronous vs. Asynchronous I/O

- **Synchronous:** Data transfer is clocked; both sides operate at same rate.
- **Asynchronous:** Uses handshaking; accommodates devices of different speeds.

---

## Memory-Mapped vs. Isolated I/O

- **Memory-Mapped I/O:** Devices use the same address space as memory; CPU uses standard instructions.
- **Isolated I/O:** Separate address space and instructions for I/O.

---

## I/O Scheduling and Buffering

- **Buffering:** Temporary storage to smooth speed mismatch between CPU and devices.
- **Spooling:** Buffering for slow devices (e.g., print queues).
- **I/O Scheduling:** Determines order of requests (e.g., disk scheduling algorithms: FCFS, SSTF, SCAN).

---

## Error Detection

- Parity, CRC, checksums for reliable data transfer.

---

## Plug and Play

- Automatic detection and configuration of devices (PCI, USB).

---

## Interview Patterns

- Explain DMA and its advantages.
- Describe interrupt-driven I/O and handling.
- Compare memory-mapped and isolated I/O.
- Discuss bus arbitration and priorities.
- Draw the block diagram of an I/O system.

---

## Common Pitfalls

- Ignoring CPU overhead in programmed I/O.
- Confusing synchronous and asynchronous transfer.
- Overlooking buffering in performance analysis.

---

## Exercises

1. Draw the block diagram of a DMA-based I/O system.
2. Explain the steps involved in handling an I/O interrupt.
3. Compare programmed, interrupt-driven, and DMA I/O.
4. List types of buses and their functions.
5. Design a simple I/O handshake protocol.

---

## Key Interview Questions

- What is the advantage of DMA over interrupt-driven I/O?
- How does memory-mapped I/O work?
- What are the main components of an I/O interface?
- Explain the role of buffering in I/O systems.

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 11](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Input/Output Organization](https://www.geeksforgeeks.org/input-output-organization-in-computer-architecture/)
- [Wikipedia: Input/Output](https://en.wikipedia.org/wiki/Input/output)
- [Patterson & Hennessy, Computer Organization and Design, Ch. 6](https://www.elsevier.com/books/computer-organization-and-design-arm-edition/patterson/978-0-12-801733-3)

---
