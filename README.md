## Overview

This README provides a detailed description of the Verilog modules implemented in this project. The modules included are:
1. **4-Bit Adder**
2. **Arithmetic Logic Unit (ALU)**
3. **Multiplexer (MUX) with CASE Statement**
4. **3-Bit Up/Down Counter**

Each module's purpose and functionality are explained below.

## 1. 4-Bit Adder

### Description
The 4-Bit Adder module performs binary addition of two 4-bit numbers, producing a 4-bit sum and a carry-out bit.

### Functionality
- **Inputs:** Two 4-bit numbers `A` and `B`, and a carry-in bit `Cin`.
- **Outputs:** A 4-bit sum `Sum` and a carry-out bit `Cout`.

## 2. Arithmetic Logic Unit (ALU)

### Description
The ALU module performs various arithmetic and logical operations on two 4-bit inputs based on a 3-bit control signal.

### Functionality
- **Inputs:** Two 4-bit numbers `A` and `B`, and a 3-bit control signal `ALU_Sel`.
- **Outputs:** A 4-bit result `ALU_Out` and a carry-out bit `CarryOut`.

## 3. Multiplexer (MUX) with CASE Statement

### Description
The MUX module selects one of several input signals and forwards the selected input to a single output line using a CASE statement for selection.

### Functionality
- **Inputs:** Two 4-bit numbers `A` and `B`, and a selection bit `Sel`.
- **Output:** A 4-bit output `Out`.

### Selection Logic
- If `Sel` is `0`, `Out` is `A`.
- If `Sel` is `1`, `Out` is `B`.

## 4. 3-Bit Up/Down Counter

### Description
The 3-Bit Up/Down Counter module counts up or down based on a control signal.

### Functionality
- **Inputs:** Clock `Clk`, reset `Reset`, and control signal `UpDown`.
- **Output:** A 3-bit counter output `Count`.

### Counting Logic
- On each clock cycle, if `Reset` is `1`, the counter resets to `0`.
- If `UpDown` is `1`, the counter increments.
- If `UpDown` is `0`, the counter decrements.

## Conclusion

These Verilog modules provide essential digital logic functionalities and can be integrated into larger systems. Each module is designed with clear inputs and outputs, making them easy to use and integrate. For further customization and functionality, you can modify the Verilog code as needed.
