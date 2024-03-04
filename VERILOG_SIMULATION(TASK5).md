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
![1](https://![Screenshot 2024-03-04 194441](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/eb0dadd3-966f-40d7-81f2-0476b920aec6)


## 3. INSTRUCTION SET OF RISC-V RV32I
![2](https://![Screenshot 2024-03-04 194958](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/f3863dfc-86ec-4a9e-a485-012108349ef0)



![3](https://![ss3](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/4b5a4508-7c08-445e-b0f9-56fde7fffa7d)


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
$ iverilog -o hello hello.v hello_tb.v

$ ./hello
```

![running verilog code using iverilog](https://![hello](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/19f3bc3e-59f7-4528-b937-a09a56387145)



- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd'

![w1](https://![gtkwave](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/7f6fc16e-92d0-4283-a482-1f605668dec2)



### 4.3 The output waveform


 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 <img width="1282" alt="1" src="https://![pic1](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/59b3e5ec-9c27-464a-8981-d3513ffce04d)


 Instruction 2:sub r7,r1,r2
 <img width="1280" alt="2" src="https://![pic12](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/7f237bc2-bedd-4984-8f12-8e8bfd6d5bde)

Instruction 4:or r9,r2,r5
<img width="1294" alt="4" src="https://![pic13](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/0ed56971-a107-461b-bdfd-344725bea112)


 Instruction 5:xor r10,r1,r4
 <img width="1293" alt="5" src="https://![pic14](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/77b7594f-7028-40bd-a9a1-3bc066ee3b68)


  

![w6](https://![pic16](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/7a64e0d2-b2f1-4262-b146-ca2edc553813)


![RISCV_folder](https://![pic0](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/733965a9-3bbb-4c15-b411-5c4d8ad29825)


