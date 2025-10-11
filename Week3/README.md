BabySoC Week 3 - Post-Synthesis GLS & STA Fundamentals

This week focuses on validating synthesized designs through Gate-Level Simulation (GLS) and understanding Static Timing Analysis (STA) fundamentals using OpenSTA.

Part 1 - Post-Synthesis 
Steps Performed

1. Synthesis of BabySoC Design
```
# yosys
read_verilog src/module/vsdbabysoc.v
read_verilog -I src/include src/module/rvmyth.v
read_verilog -I src/include src/module/clk_gate.v


```
<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/a84071f6-e823-470f-8080-05c33e829b42" />


<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/a0895e9c-56ef-440c-a37a-9b22d4856f15" />


<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/34618963-c09e-4c2a-9788-f8723deac071" />

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/e78fca64-8eed-43dd-8c45-dea156d65242" />

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/c53a44ea-66a8-457c-84a2-3cc043fbddcb" />


<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/2ee8b6b8-09e9-444e-8a3e-acc814a6cf7f" />



Caption: Post-synthesis GLS waveform showing correct functionality



VSD HDP GLS Reference

STA Fundamentals Course

OpenSTA GitHub

OpenSTA Documentation
