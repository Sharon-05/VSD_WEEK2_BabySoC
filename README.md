# VSD_WEEK2_BabySoC
# BabySoC Week 2: Fundamentals & Functional Modelling

**Topics Covered:**

* System-on-Chip (SoC) fundamentals
* Components of typical SoCs: CPU, memory, peripherals, interconnect
* BabySoC as a simplified educational model
* Role of functional modelling in SoC design flow

## Part 2: Labs (Hands-on Functional Modelling)

### Lab Steps

Steps: 
1.Clone the BabySoC project repo. 
2.Compile the BabySoC Verilog modules using iverilog. 
3.Simulate and generate .vcd waveform files. 
   Open .vcd files in GTKWave and analyze: 
         Reset operation 
         Clocking 
         Dataflow between modules 
### Simulation Results

<img width="1271" height="799" alt="image" src="https://github.com/user-attachments/assets/bcc8cb78-fcb3-45ad-bf99-d3bc8f4a8638" />


<img width="1275" height="798" alt="image" src="https://github.com/user-attachments/assets/59daa5f2-5ac7-4e93-b5bd-d50459a75bef" />


<img width="1284" height="794" alt="image" src="https://github.com/user-attachments/assets/353a6a31-33dd-404f-b457-3e430a615cf1" />


<img width="1276" height="798" alt="image" src="https://github.com/user-attachments/assets/629f591e-4e22-4677-b587-1259165e8507" />



* **Reset Operation:** Shows reset signal initializing BabySoC components
* **Clock Generation:** PLL generates stable clock signals
* **Data Flow:** Digital output from RISC-V core converted to analog by DAC
* **Dump Waveform:** `dump.vcd` waveform demonstrating full simulation

### Generated Files

* `babysoc.out.out` – Compiled simulation executable
* `dump.vcd` – Waveform data
* Simulation logs and verification reports


**Compile Design**

```bash
iverilog -o output/simulation_results/babysoc.out -I src/include -I src/module src/module/testbench.v src/module/*.v
```

**Run Simulation**

```bash
cd output/simulation_results ./babysoc.out
```

**Waveforms**

```bash
gtkwave dump.vcd
```

### Conclusion

* Demonstrates understanding of SoC architecture
* Functional modelling of digital systems
* Simulation and verification with standard tools
* Integration of processor, clock, and analog interfaces

**BabySoC** is an educational platform for learning embedded systems design and digital-analog interfacing concepts.
