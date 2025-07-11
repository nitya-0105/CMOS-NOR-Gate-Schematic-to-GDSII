# CMOS-NOR-Gate-Schematic-to-GDSII
Introduction of Nor Gate -
In CMOS (Complementary Metal-Oxide-Semiconductor) technology, a NOR gate is a fundamental combinational logic gate that outputs logic ‘0’ when any of its inputs are logic ‘1’, and only outputs logic ‘1’ when all inputs are ‘0’.
 
Table of Content :

1.Schamtic Circuit Design

2.Symbol and Analysis 

3.Layout and Optimization Technique

4.Verification 

5.Calculation

This repository focuses on the design and simulation of a 2-input CMOS NOR gate.

A NOR gate (NOT + OR) is a digital logic gate that outputs logic HIGH (‘1’) only when all inputs are LOW (‘0’). If any input is HIGH, the output will be LOW.

The CMOS implementation of a NOR gate consists of:

A Pull-Up Network (PUN) using PMOS transistors in series

A Pull-Down Network (PDN) using NMOS transistors in parallel

📌 The number of PMOS and NMOS transistors required depends on the number of inputs:
For a 2-input NOR gate → 2 PMOS + 2 NMOS
![CMOS NOR Gate Circuit](https://user-images.githubusercontent.com/99066843/152633848-0b85bb7c-ab51-4721-87bb-5e0b6086fbcf.png)

![CMOS NOR Gate Symbol](https://user-images.githubusercontent.com/99066843/152634113-20813373-ca72-41a1-9ff2-96fba86acb30.png)

The schematic is built using Cadence Virtuoso in 90nm CMOS technology, ensuring accurate transistor-level design and simulation.
The images shown below represents the circuit diagram and a logic symbol of a CMOS NOR gate.

**Schematic of NOR Gate** 
![Schematic of NOR gate ](https://github.com/nitya-0105/CMOS-NOR-Gate-Schematic-to-GDSII/blob/main/NOR%20Gate%20Schematic.jpg)
2.Simulation 
The CMOS NOR gate was simulated using Cadence Virtuoso with GPDK 90nm technology, focusing on analyzing transient response, waveform behavior, and the effect of PMOS sizing on output timing characteristics.

Transient Analysis Observations:
The output waveform was analyzed for rise time (LOW to HIGH) and fall time (HIGH to LOW).

Since PMOS transistors are in series, they dominate the rise time, while the NMOS in parallel dominate the fall time.


PMOS Width	Rise Time

120nm        	~42 ps

280nm	        ~31.5 ps

560nm        	~28 ps

**Transient Analysis**
![Transient Analysis](https://github.com/nitya-0105/CMOS-NOR-Gate-Schematic-to-GDSII/blob/main/NOR%20gate%20Transient%20Analysis.jpg)

As PMOS width increases, the rise time improves due to reduced pull-up resistance.
Fall time remained nearly constant since NMOS sizing was unchanged

![Calculation of Rise and Fall Time](https://github.com/nitya-0105/CMOS-NOR-Gate-Schematic-to-GDSII/blob/main/NOR%20ate%20Calculation.jpg)

he observed results align with the theoretical relationship:

𝑡
𝑟
𝑖
𝑠
𝑒
∝
𝑅
𝑝
⋅
𝐶
𝐿
and
𝑅
𝑝
∝
1/
𝑊
𝑝

​
 
Hence, increasing PMOS width (W<sub>p</sub>) reduces resistance and improves rise time — until parasitic effects start to dominate.

