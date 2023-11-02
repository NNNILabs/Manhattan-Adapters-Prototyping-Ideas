# Manhattan Adapters & Prototyping Ideas
## Introduction
Prototyping precision and high-speed analog circuits on breadboards, perfboard or stripboard is impractical and performance falls victim to parasitics. The Manhattan prototyping style is a possible solution, and involves "dead-bugging" components on copper-clad board and making connections using component leads and tinned or enamelled wire. Nodes are connected mid-air through component leads, on isolated parts of the copper-clad board, or using "tiles" consisting of square-shaped FR4 pieces with exposed copper. Since the circuit is constructed on top of a layer of copper, a low-impedance return path is automatically present.
## Project Motivation
While there are a wide range of prototyping aids available, they are not always designed with regard to this method of prototyping. For example, various DIP adapters are available, which break out SMD IC packages like SOIC, MSOP and QFN to pin headers with standard 100mil spacing. The adapters in this repository, while follwing a similar idea, are designed differently with decoupling and placement on a base copper-clad board in mind. The foundations of this project are based on [Mark's Manhattan Toolkit](https://github.com/macaba/TheManhattanToolkit).
## Usage
Copper-clad board forms the base upon which the circuit is built. A board of suitable size is to be selected, and power strips cut out of spare board and fixed to the board in such a way that the adapter boards fit between them with space for making connections to ground. The adapters themselves are placed in between the power strips. Connections are to be made preferrably using enamelled copper wire, since accidental contact won't lead to unwanted connections. Having the power rails on the sides of the components is similar to the arrangement of connections on a solderless breadboard. 

<p align="center">
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/Usage.png" height=500>
</p>

(After writing this readme, I happened to come across [this](https://entertaininghacks.files.wordpress.com/2020/07/ps-manhattan04-1.jpg) picture from the Entertaining Hacks blog (link below), which shows a very similar setup. Looks like this idea is not so original after all!)
## List of Files
- SOIC/MSOP-8 adapter: Contains space for a SOIC-8 package on one side, and an MSOP-8 on the other. Decoupling on each supply pin is also possible, and it is particularly easy for pins 1, 4, 5 and 8, since they have direct access to the center region. This applies to both SOIC and MSOP. The center region is intended to be soldered as directly as possible to the base board. (Passive size in image: 0603)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOIC%2BMSOP.png" height=250>
</p>

- 4x Passive adapter: Traces are arranged in such a way as to fit passive components of size 1206 and below, series/parallel connections are possible. (Passive sizes in image: 0402, 0603, 0805, 1206.)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/Passive.png" height=250>
</p>

- SOT-23 adapter: Fits four SOT-23 packages. Since the top-center pin is usually used to dissipate power, its trace is larger than the other two pins. With some creativity in orientation and placement, other packages like SOT-89 and SOT-223 can be soldered (second picture). (Passive size in image: 0603)

<p align="center"> 
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOT23.png" height=250>
</p>

<p align="center">   
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOT23%20Creative.png" height=250>
</p>

- SOIC/MSOP-20 adapter: For use with most common SOIC/MSOP footprints up to SOIC-16/MSOP-20. (Passive size in image: 0603)

<p align="center">
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOIC20%2BMSOP20.png" height=250>
</p>

- LFCSP-8 adapter: I made this because the [ADA4528](https://github.com/macaba/Nuts#nsd) samples I got were in this weird package. (Passive size in image: 0603)

<p align = "center">
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/LFCSP-8.png" height=250>
</p>

- DIP-8 adapter: The LT1193s I have are in DIP.

<p align = "center">
<img src="https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/DIP-8.PNG" height=250>
</p>

- Power strip: 7cm x 10cm FR4 copper-clad board turned out to be more expensive than I thought, so ordering cheap(er) power strips seemed like a resonable idea. Can be broken in half if needed.

<p align = "center">
<img src="https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/Power%20Strip.PNG" height=250>
</p>

- SOT-23-6: The existing SOT-23 adapter cannot handle SOT-23-6 and SOT-23-5 packages easily. 

<p align = "center">
<img src="https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/SOT23-6.PNG" height=250>
</p>

- WSON-20:

<p align = "center">
<img src="https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/WSON20.PNG" height=250>
</p>

## Application Examples
- TL431 Shunt regulator

<p align="center">
<img src="https://github.com/NNNIIndia/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/Application%201.png" height=500>
</p>

- REAL application examples from REAL people:
  - GhostDog: (unknown circuit)
  ![](https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/ghostdog.png)
  - Me: (LM317 regulator, 555 oscillator, 74AC04/source follower current pulser)
  ![](https://github.com/NNNILabs/Manhattan-Adapters-Prototyping-Ideas/blob/main/Resources/20230331_200238.jpg)
## Notes
- These adapters were made specifically for use with 0603 passives, although passives up to 1206 will fit.
- Clearance between traces is 10 mils.
## Links
- https://github.com/macaba/TheManhattanToolkit
- https://www.youtube.com/watch?v=vq968AFgPhg
- https://www.analog.com/media/en/training-seminars/tutorials/MT-100.pdf
- https://hackaday.com/2016/05/04/getting-ugly-dead-bugs-and-going-to-manhattan/
- https://entertaininghacks.wordpress.com/2020/07/22/prototyping-circuits-easy-cheap-fast-reliable-techniques/
  - http://hyse.org/pdf/www.aoc.nrao.edu/~pharden/hobby/HG-MANHAT2.pdf
  - https://www.analog.com/media/en/technical-documentation/application-notes/an120f.pdf
  - https://www.analog.com/media/en/technical-documentation/application-notes/an47fa.pdf
