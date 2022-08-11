# RTL-Design-Workshop

## 1. Introduction
RTL Design using Verilog with SKY130 Technology Workshop by VLSI System Design-IAT was a 5 day workshop in RTL design and synthesis. This workshop covered RTL design and synhtesis using Verilog with the help of open source tools such as iverilog, gtkwave and yosys. The SkyWater Open Source PDK was used to design, simulate and verify the design. 

## 2. Day 1: Introduction to Verilog RTL design and Synthesis

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

### 2.8 Labs on compilation and simulation using iverilog and GTKWave
In this lab, we compiled and simulated verilog files using iverilog and GTKWave. The commands to compile and simulate the verilog design and tesbench using iverilog and to view the simulation waveform in vcd file on GTKWave are as follows:
```
$ iverilog design_file.v testbench.v
$ ./a.out
$ gtkwave vcd_file.vcd
```
### 2.9 Introduction to Yosys open synthesis suite
Yosys is a framework for Verilog RTL synthesis. It currently has extensive Verilog-2005 support and provides a basic set of synthesis algorithms for various application domains. Selected features and typical applications:

 - Process almost any synthesizable Verilog-2005 design
 - Converting Verilog to BLIF / EDIF/ BTOR / SMT-LIB / simple RTL Verilog / etc.
 - Built-in formal methods for checking properties and equivalence
 - Mapping to ASIC standard cell libraries (in Liberty File Format)
 - Mapping to Xilinx 7-Series and Lattice iCE40 and ECP5 FPGAs

### 2.10  Netlist
In electronic design, a netlist is a description of the connectivity of an electronic circuit. In its simplest form, a netlist consists of a list of the electronic components in a circuit and a list of the nodes they are connected to.
