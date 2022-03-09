# Low-Power_SRAM
# 1.1 Introduction
SRAM is intended to contribute to agility and low power consumption[1]through a direct alliance with the Central Processing Unit (CPU), in order to reduce battery life owing to increasing development in portable devices. The speed and power parameters play a significant role in improving the capacity of electronic equipment used in research and commercial centres. SRAM is a semiconductor memory that utilises flip flop to store each sample as a set of latches. SRAM is quicker than DRAM and utilised as the CPU cache.While DRAM offers a high packing density, cheap cost, lower power consumption, it has to be constantly updated over a period of time. The SRAM cell may overcome this.The SRAM is symmetrical; reading time is equal to specifying the time it has endurance.
![1](https://user-images.githubusercontent.com/100713556/156221114-265d09a6-d933-4753-928b-4ff821dd230a.png)

# 1.	Problem statements
The emerging and growing market for portable electronic devices has led the electronics designers to be more conscious of power and energy constraints in their circuit designs. Designers are forced to design more energy-aware circuits and started to develop methods and design rules to increase energy savings. In the sub-threshold region of operation, the power supply voltage of the circuit is lowered below to transistor’s threshold voltage. As a consequence, its active and leakage power is reduced dramatically. However, this advance comes at the cost of circuit switching speed. One of the central areas of micro electronic design that is affected by such design methodology is memory design. 
![2](https://user-images.githubusercontent.com/100713556/156221150-a997229d-10d1-4b19-b26b-b09b10a563cd.png)

# 2.	Objective of the Project
3.	SRAM Difficulties in maintaining an appropriate noise margin and managing critical instabilities and soft error rate with scaling [are the most difficult problems for the CMOS process's future generations].”
The purpose of this research is to evaluate different low-power SRAM cells and to suggest a cell with a smaller footprint.
With increasing demand for low-power SRAMs, low-power design methods are focusing on several causes of power consumption. Increased leakage current in scaled technology necessitates low-power methods that decrease the SRAM cell's leakage current. Additionally, the SRAM unit's dynamic power consumption is considerable due to the high capacitance of the lengthy interconnecting cables. Because of the high voltage swing nature of the bitlines, the write operation consumes a substantial portion of the total power. As a result, methods for reducing dynamic power consumption, especially write power usage, have gotten a lot of attention. 
# 3.	works Literature survey/Existing related
The need for SRAM power reduction forced several researchers into new low-power circuits. Six transistors for low-power applications have been well known. Figure 1.7 shows a 6-transistor normal SRAM cell that contains one bit of data in an SRAM unit. It usually includes a loop of two transistors and two inverters. The M3 and M4 transistors of the NMOS are termed drive transistors and are responsible for unloading the bitline during reading. The M2 and M1 transistors are known as access transistors. Once enabled, the internal cell nodes(i.e., nodes A and B) may interact using bitlines. The transistor gate is termed word line (WL). The M5 and M6 PMOS transistors are known as load transistors. One internal cell node is at VDD and the other at VSS according to the logical value recorded in the cell. The cell leakage current is displayed in the image when it is not accessible.
![3](https://user-images.githubusercontent.com/100713556/156221617-6fdf421a-9710-4995-a0b6-540270bb4105.png)

The leakage current is caused mainly by subthreshold current and, to a lesser extent, by Gate Induced Drain Leakage (GIDL). The next chapters will demonstrate that the leakage current is inversely proportional to the threshold voltage of the transistors.
# 6T SRAM: 
The CMOS standard 6T SRAM cell has two PMOSs, two NMOSs, and two NMOSs as access transistors. Two data-storage inverters are manufactured and cross-coupled in such a manner that positive feedback is generated. The two inverters are designated as P1, N1, and P2, N2. Additionally, it features a horizontally oriented Word Line (WL) and vertically aligned Bit Lines (BL and BLB). SRAM operates in three distinct modes: standby, read, and write. During standby mode, Vdd is supplied to BL, and WL is turned off, forcing the transistors linked to it to turn off as well. Due to the fact that BL=VDD, the two cross-coupled inverters give positive feedback, which enables data storage while power is supplied. The WL line, which controls the state of the access transistors, is enabled only during read and write operations.
![4](https://user-images.githubusercontent.com/100713556/156221632-3ef88c14-9f40-48b3-b98f-05108e70e9dd.png)
# A sense amplifier
A sense amplifier is required for memory circuits to attain high performance, endurance, and usefulness. It is a part of the read circuitry that is responsible for reading data from memory. Its purpose is to monitor low-power signals from a bit line and convert the tiny voltage difference to full logic voltage, which represents the data bit stored in a memory cell, thus reducing read time significantly. It includes voltage sensing, low-voltage amplification, delay reduction, power consumption reduction, and signal restoration capabilities. They are mainly used to amplify the differential voltage across complimentary bit lines during read operations without flipping the stored cell data, enabling the data to be handled properly by the memory's output circuitry.
![6](https://user-images.githubusercontent.com/100713556/156223368-012f97ed-8b72-4cb9-80ca-0f8a21bed00b.png)

# Pre-Charge Circuit
Pre-charge circuits are used to quickly and painlessly charge both bit-lines voltages to VDD before to each read and write operation. The pre-charge circuit is shown. It comprises of two pull-up PMOS transistors and an equalisation that balances the voltages on both bit lines. The pull-up transistors are controlled by the PR signal, which controls the transistor M3, an equalisation signal that balances the voltage on both bit lines. The term "Vdd pre-charge" refers to the pre-charge. In the pre-charge circuit, PMOS transistors are utilised because they are the most efficient at transmitting the Vdd level voltage to the bit lines.
![7](https://user-images.githubusercontent.com/100713556/156222409-b64a93ab-929c-4542-a8eb-c652a443cab4.png)
# 3.	Concluding Remarks
In this project, a low-power and less area SRAM cell is presented using gpdk 28nm technology.

![6T_SRAM](https://user-images.githubusercontent.com/100713556/157513011-140710b0-6b9f-40ea-83e9-168c3c901c07.PNG)





