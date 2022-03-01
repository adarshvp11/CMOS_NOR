# CMOS_NOR
This repository presents the design of NOR gate implemented using Synopsis Custom Compiler on 28nm CMOS Technology.

### Table of Contents
 - [Introduction](#introduction)
 - [Reference Circuit Diagram](#reference-circuit-diagram)
 - [Reference Circuit Waveform](#reference-circuit-waveform)
 - [Tools Used](#tools-used)
 - [Schematics and Simulations:](#schematics-and-simulations)
 - [Netlist of the Circuit:](#netlist-of-the-circuit)
 - [Author:](#author)
 - [Acknowledgements:](#acknowledgements)
 - [References:](#references)
 
## Introduction
The NOR gate is a digital logic gate that implements
logical NOR. NOR is the result of the negation of the OR
operator. If both the inputs to the gate are LOW (0), a HIGH
output (1) is obained as result; if one or both input is HIGH (1),
a LOW output (0) is obtained as result. It can also in some senses
be seen as the inverse of an AND gate. NOR is a functionally
complete operation. NOR gates can be combined to generate any
other logical function. It shares this property with the NAND
gate. NOR gates can be combined to generate any other logical
function. Hence, NOR gate is called Universal logic Gate along
with NAND gate.In this we have carried out the modeling
of NOR gate at 28 nm CMOS technology





![ss](https://user-images.githubusercontent.com/100693635/156202769-4d721926-b2d2-4b1a-a7a9-92afdaea4c26.PNG)



Fig. 1: Block Diagram of NOR gate and Logic Diagram of NOR gate

![ss2](https://user-images.githubusercontent.com/100693635/156202795-d2979822-6327-497c-b632-8c850dab5d06.PNG)


Table 1: Truth Table of NOR gate. Procedure for Paper Submission
## Reference Circuit Diagram
Complementary Metal Oxide Semiconductor (CMOS) logic[1] deploys symmetric number of both types of MOSFETs, i.e., pMOS and nMOS. This leads to better performance of any logic circuit since nMOS is strong ‘0’ device and pMOS is strong ‘1’device. Thus, CMOS provides complete ‘1’ and complete ‘0’ logics at the output without any distortion. NOR gate using CMOS modeled using four  transistors as shown in Figure 3.


![CamScanner 02-19-2022 15 21_1](https://user-images.githubusercontent.com/100693635/156201945-805124fd-0d43-47e1-9d56-374a7dfa1f35.jpg)

 
Figure 3. NOR gate Using CMOS Logic.

## Reference Circuit Waveform

 ![CamScanner 02-19-2022 15 29_1](https://user-images.githubusercontent.com/100693635/156201974-a94b4bba-600d-4b75-96c6-539357b6dd13.jpg)



## Tools Used:
• Synopsys Custom Compiler:
 The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

• Synopsys Primewave:
 PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

• Synopsys 28nm PDK:
 The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.
 
 ## Schematics and Simulations:
 ### Schematics:
 ### CMOS NOR
 Initially Schematic of the NOR gate cell was implemented and converted into a symbol so that it could be used directly as delay cell from the library.
 
 
 
 ![ss3](https://user-images.githubusercontent.com/100693635/156211611-8ec48aff-e217-480f-9882-9640d8ee7c0f.PNG)

 
 Fig. 4: NOR gate Cell Schematic
 
 
 ![ss7](https://user-images.githubusercontent.com/100693635/156211669-56033f33-ddd8-45ba-9e18-b93eb390cc0e.PNG)

 Fig. 5: NOR gate Cell Symbol
 
 ### Parameters set for Voltage Source for Input A
 ![ss4](https://user-images.githubusercontent.com/100693635/156211630-b0fd5864-71b2-4863-86c3-9e0daa2eac82.PNG)








 
 
 
 ### Parameters set for Voltage Source for Input B
 
 
 ![ss5](https://user-images.githubusercontent.com/100693635/156211644-6b7fd639-fdb8-43d6-ab13-688526d6fcac.PNG)

 

 
 
 ![ss6](https://user-images.githubusercontent.com/100693635/156211664-eefa923b-d987-4dd6-b162-ffc7e5b18bd7.PNG)

 Fig. 6: NOR gate Test Circuit 
 
  ### Transient Settings
 
 ### Simulations:
 ### Transient Analysis:
After creating and saving the schematic go to 'Tools' and open 'Primewave' to start the simulation. In the Primewave select the 'model file' i.e the '28nm PDK's .lib file presentin the HSPICE folder.Then add the outputs which needs to be plotted by selecting the nets on the schematic.

![transient](https://user-images.githubusercontent.com/100190726/155507012-b7369b24-be78-401d-aae3-884e000e7ce0.JPG)


Then go to 'Simulations -> Netlist and Run' to generate a netlist and run the simulation to get the below output.

!![hackathon](https://user-images.githubusercontent.com/100693635/156202057-3d5e7c57-ebe3-42fb-b4ed-74fb58fb7ab2.PNG)

Fig. 7: NOR gate output simulation


## Netlist of the Circuit:
Refer to the netlist of the circuit here:[netlist.txt](https://github.com/swati-sgm/Half_Adder_analog_design/files/8129767/netlist.txt)



## Author:
Adarsh V Parekkattil, MTECH 1st year, NIT Meghalaya

## Acknowledgements:
- [Cloud Based Analog IC Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- [Synopsys India](https://www.synopsys.com/)
- [VLSI System Design (VSD) Corp. Pvt. Ltd India](https://www.vlsisystemdesign.com/)
- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Chinmay panda, IIT Hyderabad
## References:
- Balraj Singh, Mukesh Kumar, and J. S. Ubhi, “Analysis of CMOS based
NAND and NOR Gates at 45 nm Technology”, International Journal of
Electronics, Electrical and Computational System , IJEECS ,ISSN 2348-
117X,, Volume 6, Issue 4, April 2017
- V. soni and nitin naiyar. Evaluation of logic families using nor and
nand logic gates. https://studylib.net/doc/18649909/evaluation-oflogicfamilies-using-nor-and-nand-logic-gate.
 
