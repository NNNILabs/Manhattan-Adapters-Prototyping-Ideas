# Manhattan Adapters & Prototyping Ideas
## Introduction
Prototyping precision and high-speed analog circuits on breadboards, perfboard or stripboard is impractical and performance falls victim to parasitics. The Manhattan prototyping style is a possible solution, and involves "dead-bugging" components on copper-clad board and making connections using component leads and tinned or enamelled wire. Nodes are connected mid-air through component leads, on isolated parts of the copper-clad board, or using "tiles" consisting of square-shaped FR4 pieces with exposed copper. Since the circuit is constructed on top of a layer of copper, a low-impedance return path is automatically present.
## Project motivation
While there are a wide range of prototyping aids available, they are not always designed with regard to this method of prototyping. For example, various DIP adapters are available, which break out SMD IC packages like SOIC, MSOP and QFN to pin headers with standard 100mil spacing. The adapters in this repository, while follwing a similar idea, are designed differently with decoupling and placement on a base copper-clad board in mind. 
## List of boards:
- SOIC/MSOP-8 adapter: Contains space for a SOIC-8 package on one side, and an MSOP-8 on the other. The trace patterns are optimised for supply decoupling either on pin 7 or 8. In the case of dual-supply op-amps, decoupling on each supply pin is also possible. This applies to both SOIC and MSOP. (Passive sizes in image: 0402, 0602.)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOIC%2BMSOP.png" height=250>
</p>

- 4x Passive adapter: Traces are arranged in such a way as to fit passive components of size 1206 and below, series/parallel connections are possible. (Passive sizes in image: 0402, 0603, 0805, 1206.)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/Passive.png" height=250>
</p>

- SOT-23 adapter: Fits four SOT-23 packages. Since the top-center pin is usually used to dissipate power, its trace is larger than the other two pins. With some creativity in orientation and placement, other packages like SOT-89 and SOT-223 can be soldered (second picture). (Passive sizes in image: 0603, 0805.)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOT23.png" height=250>
</p>

<p align="center">   
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOT23%20Creative.png" height=250>
</p>

- SOIC/MSOP-20 adapter: For use with most common SOIC/MSOP footprints up to SOIC/MSOP-20.
