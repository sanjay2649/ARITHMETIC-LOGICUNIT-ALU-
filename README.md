# ARITHMETIC-LOGICUNIT-ALU-

COMPANY :CODTECH IT SOLUTIONS

NAME :SANJAY RAJ C

INTERN ID :CT04DH982

DOMAIN: VLSI

DURATION: 4 WEEKS

MENTOR : NEELA SANTOSH


This Verilog module, simple_alu, implements a tiny 4‑bit Arithmetic Logic Unit that operates purely combinationally. It accepts two 4‑bit unsigned inputs (A and B) and a 3‑bit opcode that selects the operation. The result is a 4‑bit reg, assigned inside an always @(*) block, which tells the synthesizer/simulator that the logic is combinational (i.e., it should re‑evaluate whenever any input changes). The ALU supports five operations: addition (opcode = 3'b000), subtraction (001), bitwise AND (010), bitwise OR (011), and bitwise NOT of A only (100). Any other opcode defaults the output to zero. Because all datapaths are only 4 bits wide, arithmetic naturally wraps around modulo 16; overflow/underflow flags are not produced, and high-order carries are silently discarded. Subtraction is two’s‑complement by construction (as in standard Verilog arithmetic), so A - B will also wrap modulo 16. The use of reg for result is just a Verilog storage type requirement for signals assigned in procedural blocks; it does not imply sequential logic, since there is no clock and no non‑blocking (<=) edge‑triggered assignment. The priority chain is written as an if/else if ladder; functionally this is equivalent to a case statement for mutually exclusive opcodes, but the given form is perfectly synthesizable. The NOT operation ignores B, which is typical for unary operations. In practice, you might later extend this ALU with XOR, arithmetic shifts, set‑on‑less‑than, or with status flags (carry, zero, negative, overflow).


code1.v it is a verilog verified by modelsim
code2_tb.v it is a verilog verified by modelsim

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/5d9c554e-9a5c-4ef5-b09a-5274ae9ab932" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4b338aca-aca6-4cc4-9504-32b2ead18ef6" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0322cadf-7873-4300-b4c2-e1d86b118b1f" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2da473a2-140b-4815-ac69-f0233500c33d" />
