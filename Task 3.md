-understand the R, I, S, B, U, and J instruction types.
-For those 15 instructions, determine the exact 32-bit instruction code in their respective instruction type formats.
<img width="960" alt="T1 - Copy" src="https://github.com/user-attachments/assets/a1b9692a-8e45-4bb8-9dfb-2279e171ee62" />
**1) Instruction: lui a0, 0x21**
Opcode: 0110111 (7 bits)
Immediate: 0x21 (20 bits)
Destination Register (rd): a0 (x10, 5 bits)
Breakdown:
Immediate (20 bits): 0000 0000 0000 0010 0001
rd (a0 = x10): 01010
Opcode: 0110111
Machine Code:
Binary: 0000 0000 0000 0010 0001 0101 0011 0111
Hex: 00021537
<img width="960" alt="T2" src="https://github.com/user-attachments/assets/ba3f20ff-03e7-4a52-9358-fc1930075bd1" />
**2) Instruction: li a2, 210**
Opcode: 0010011 (7 bits)
Immediate: 210 (12 bits)
Source Register (rs1): (00000 5 bits)
Destination Register (rd): a2 (x12, 5 bits)
Function (funct3): 000 (3 bits)
**Breakdown:**
Immediate (12 bits): 0000 1101 0010
rs1: 00000
funct3: 000
rd (a2 = x12): 01100
Opcode: 0010011
Machine Code:
Binary: 0000 1101 0010 0000 0000 0110 0001 0011
Hex: 0d200613
