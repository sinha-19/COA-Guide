# 02. Number Systems and Data Representation

---

## Why Number Systems Matter

Understanding number systems and their representations is crucial for hardware design, programming, networking, and error detection.

---

## Types of Number Systems

- **Binary (Base 2):** Digits 0, 1 – used internally by all computers.
- **Octal (Base 8):** Digits 0–7 – sometimes used as shorthand for binary.
- **Decimal (Base 10):** Digits 0–9 – standard human system.
- **Hexadecimal (Base 16):** Digits 0–9, A–F – compact representation for binary.

---

## Conversion Techniques

- **Binary ↔ Decimal**: Use positional weights (e.g., 1101₂ = 1×8 + 1×4 + 0×2 + 1×1 = 13₁₀)
- **Decimal ↔ Binary**: Repeated division/remainder.
- **Binary ↔ Hexadecimal**: Group binary digits into 4s.

---

## Data Representation in Computers

### 1. Integer Representation

- **Unsigned Integers**: All bits represent the value.
- **Signed Integers**: 
    - **Sign-Magnitude**: Most significant bit (MSB) is the sign.
    - **1’s Complement**: Invert all bits for negative numbers.
    - **2’s Complement**: Invert all bits and add 1. Most common in computers.

### 2. Fixed-Point Representation

- Used to represent numbers with fractional parts when floating point is not required.

### 3. Floating-Point Representation (IEEE 754)

- **Single Precision (32 bits)**: 1 (sign) + 8 (exponent) + 23 (mantissa)
- **Double Precision (64 bits)**: 1 + 11 + 52
- Allows for a large range of real numbers.

### 4. Character Representation

- **ASCII**: 7/8 bits per character.
- **Unicode**: 16/32 bits, supports worldwide scripts.

### 5. Other Codes

- **BCD (Binary Coded Decimal):** Each decimal digit is represented by 4 bits.
- **Gray Code:** Only one bit changes between consecutive numbers. Used in encoders.

---

## Arithmetic Operations

- **Binary Addition/Subtraction**: Similar to decimal operations, with carrying/borrowing.
- **Overflow Detection**: In 2’s complement, overflow occurs if carry into MSB ≠ carry out.
- **Multiplication/Division**: Performed using add/shift algorithms.

---

## Error Detection and Correction

- **Parity Bit**: Adds an extra bit for error checking.
- **Hamming Code**: Allows detection and correction of single-bit errors.

---

## Data Storage

- **Little Endian vs. Big Endian**: Byte order in multibyte data – important for networking and file formats.

---

## Applications

- Embedded systems, networking (IP addresses), error detection, digital signal processing.

---

## Interview Patterns

- Convert decimal to binary/hex and vice versa.
- Represent a negative integer in 2’s complement.
- Detect overflow in binary addition.
- Explain the significance of Gray code.
- Design a Hamming code for a given data word.

---

## Common Pitfalls

- Forgetting to invert and add 1 for 2’s complement.
- Confusing endian-ness in storage.
- Not distinguishing between 1's and 2's complement.

---

## Exercises

1. Convert 45 (decimal) to binary, octal, and hexadecimal.
2. Represent -25 in 8-bit 2’s complement.
3. Add 10110101 and 01101101 in binary and check for overflow.
4. Encode the word “COA” in ASCII and binary.
5. Show the Gray code sequence for 4 bits.

---

## Key Interview Questions

- What is the difference between 1’s and 2’s complement?
- How is floating-point data represented in memory?
- Why is Gray code used in hardware design?
- How does a parity bit detect errors?

---

## References

- [Stallings, Computer Organization and Architecture, Ch. 2](https://www.pearson.com/en-us/subject-catalog/p/computer-organization-and-architecture/P200000001275/9780134101613)
- [GeeksforGeeks - Number Systems in COA](https://www.geeksforgeeks.org/number-system-in-computer-organization/)
- [Wikipedia: Binary Number](https://en.wikipedia.org/wiki/Binary_number)
- [IEEE 754 Standard](https://en.wikipedia.org/wiki/IEEE_754)

---
