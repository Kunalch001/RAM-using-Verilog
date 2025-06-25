# 4x4 RAM Module in Verilog

This project implements a simple 4x4 Random Access Memory (RAM) module using Verilog. It provides 4 memory locations, each capable of storing 4-bit data. The design supports both read and write operations synchronized with the clock signal.

## 🧠 Features

- 4 memory locations (indexed by 2-bit address)
- 4-bit wide data at each location
- Synchronous read and write operations (on positive clock edge)
- Write enable control

## 🧱 Module Description

### Inputs:
- `clk`: Clock signal (write and read triggered on rising edge)
- `we`: Write Enable (1 = Write, 0 = Read)
- `addr`: 2-bit address to access memory (00 to 11)
- `din`: 4-bit data to be written when `we = 1`

### Output:
- `dout`: 4-bit data output from selected memory address
