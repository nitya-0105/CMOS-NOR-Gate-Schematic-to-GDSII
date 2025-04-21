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

For a 3-input NOR gate → 3 PMOS (series) + 3 NMOS (parallel)

The schematic is built using Cadence Virtuoso in 90nm CMOS technology, ensuring accurate transistor-level design and simulation.

This repository includes:

📐 Schematic design of a 2-input CMOS NOR gate

⚡ Transient analysis and DC sweep simulations

📈 Output waveform results and performance evaluation
The images shown below represents the circuit diagram and a logic symbol of a CMOS NOR gate.

!(Schematic of NOR gate )[https://media.licdn.com/dms/image/v2/D4D22AQG0PTkhwd9_rA/feedshare-shrink_2048_1536/B4DZZNVF1aHAAk-/0/1745054098166?e=1747872000&v=beta&t=Hem_bT8Emimt-OexJKCFi6DgK6LaOWg70MS11pbJDLg]
