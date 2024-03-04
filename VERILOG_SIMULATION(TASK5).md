# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![1](https://github.com/Abdulbitm/Abdul/assets/160620896/ba781b31-81bb-4003-9b93-cff8f7825d9a)

## 3. INSTRUCTION SET OF RISC-V RV32I
![2](https://github.com/Abdulbitm/Abdul/assets/160620896/9b986703-34be-4527-8558-1e2cea21f4f9)


![3](https://github.com/Abdulbitm/Abdul/assets/160620896/0b2e2308-186c-4f70-9081-54ff8b3190ca)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```

![install_i_verilog_gtkwave](https://![task51](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/87d56ca8-a77c-48d1-9ba3-8ecad5ce9e05)


- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://![task52](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/8c9c6022-4fdc-4148-814e-c1c103910448)

 
```
(https://![task52](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/324dbc01-a554-4be4-995a-bc606744b970)


- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v 
$ ./hello
```

![running verilog code using iverilog](https://![task53](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/50b92277-ad59-4317-a3d7-86eb15300ae7)

- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello_tb.v`

![w1](https://![task54](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/c02a6ab0-ce77-4c8b-ad47-19c259f0a4e9)


### 4.3 The output waveform


 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 <img width="1282" alt="1" src="https://![pic1](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/59b3e5ec-9c27-464a-8981-d3513ffce04d)


 Instruction 2:sub r7,r1,r2
 <img width="1280" alt="2" src="https://![pic12](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/7f237bc2-bedd-4984-8f12-8e8bfd6d5bde)


Instruction 3:and r8,r1,r3
<img width="1282" alt="3" src="https://github.com/Abdulbitm/Abdul/assets/160620896/18bfdf76-1173-4984-b50b-83443ab48596">

Instruction 4:or r9,r2,r5
<img width="1294" alt="4" src="https://github.com/Abdulbitm/Abdul/assets/160620896/4f214bb2-c934-4778-bf46-841efe877fb8">

 Instruction 5:xor r10,r1,r4
 <img width="1293" alt="5" src="https://github.com/Abdulbitm/Abdul/assets/160620896/6fa91f49-5e73-4133-8bf6-84ec4aca64da">

 Instruction 6:slt r11,r2,r4
<img width="1290" alt="6" src="https://github.com/Abdulbitm/Abdul/assets/160620896/c9c32048-62ed-4f55-8e11-9763816b1bd1">

 Instruction 7:addi r12,r4,5
 <img width="1285" alt="7" src="https://github.com/Abdulbitm/Abdul/assets/160620896/308b8a9d-46c8-4a0e-8824-90e11d9a6a1e">

 Instruction 8:sw r3,r1,2
 <img width="1280" alt="8" src="https://github.com/Abdulbitm/Abdul/assets/160620896/84f16d7f-9d16-4236-b64d-615e187a00ff">

 Instruction 9:lw r13,r1,2
<img width="1295" alt="9" src="https://github.com/Abdulbitm/Abdul/assets/160620896/c7bc7d9a-6745-4eeb-903d-fa723dca1394">

 Instruction 10:beq r0,r0,15
 <img width="1287" alt="10" src="https://github.com/Abdulbitm/Abdul/assets/160620896/a1c6781f-c301-45d9-a502-fb32e6204e4c">

 After branching, performing
 Instruction 11:add r14,r2,r2
 <img width="1287" alt="11" src="https://github.com/Abdulbitm/Abdul/assets/160620896/56b50ce0-60aa-41fe-8f53-0b4583b39665">

  Full 5-stage instruction pipeline and pc-increment description Waveform
  
<img width="1325" alt="12" src="https://github.com/Abdulbitm/Abdul/assets/160620896/e5ebc923-ad2c-44fc-a577-3ce7b8419bce">

![w6](https://github.com/Abdulbitm/Abdul/assets/160620896/d39e08b3-38e9-43bd-a814-c53faebf0607)

![RISCV_folder](https://github.com/Abdulbitm/Abdul/assets/160620896/669887ed-9ab6-48f1-8cf8-83e5f3eec2bd)

