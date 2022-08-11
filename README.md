# RTL-Design-Workshop

## Introduction
RTL Design using Verilog with SKY130 Technology Workshop by VLSI System Design-IAT was a 5 day workshop in RTL design and synthesis. This workshop covered RTL design and synhtesis using Verilog with the help of open source tools such as iverilog, gtkwave and yosys. The SkyWater Open Source PDK was used to design, simulate and verify the design. 

## Day 1: Introduction to Verilog RTL design and Synthesis

### 2.1 Register Transfer Level
In digital circuit design, register-transfer level (RTL) is a design abstraction which models a synchronous digital circuit in terms of the flow of digital signals (data) between hardware registers, and the logical operations performed on those signals.

Register-transfer-level abstraction is used in hardware description languages (HDLs) like Verilog and VHDL to create high-level representations of a circuit, from which lower-level representations and ultimately actual wiring can be derived. Design at the RTL level is typical practice in modern digital design.

### 2.2 Verilog
Verilog, standardized as IEEE 1364, is a hardware description language (HDL) used to model electronic systems. It is most commonly used in the design and verification of digital circuits at the register-transfer level of abstraction.

### 2.3 Verilog Modules
A module is the basic building block in Verilog. It is a block of Verilog code that implements certain functionality. Modules can be embedded within other modules, and a higher level module can communicate with its lower-level modules using their input and output ports.

### 2.4 Testbench
The functionality of the design block can be tested by applying stimulus and checking results. We call such a block the stimulus block or testbench.We create a test bench using Verilog which applies stimuli to the RTL design and validate the design's outcomes. As a project evolves, up-front verification becomes increasingly crucial as design size and complexity grow with each stage.

### 2.5 Simulation
RTL design is checked for adherence to its design specification using simulation. Simulation is the process of appplying stimulus to the design to verify the functionality of the design.

### 2.6 Icarus Verilog
Icarus Verilog is a Verilog simulation and synthesis tool. It operates as a compiler, compiling source code written in Verilog (IEEE-1364) into some target format. For batch simulation, the compiler can generate an intermediate form called vvp assembly. This intermediate form is executed by the `vvp` command. For synthesis, the compiler generates netlists in the desired format.

### 2.7 GTKWave
GTKWave is a fully featured GTK+ based wave viewer for Unix, Win32, and Mac OSX which reads LXT, LXT2, VZT, FST, and GHW files as well as standard Verilog VCD/EVCD files and allows their viewing. 
