# OpenRPDK28

![rios-ip](https://github.com/riosmpw/OpenXPDK28/assets/100336131/9f3d5cb0-e9f8-48c8-b4e6-38c896d54da8)

**Process Design Kit** (**PDK**) is a set of files or models used within the semiconductor industry to model a fabrication process characteristic for the design tools and its users used to design an integrated circuit. An accurate PDK will increase the chances of first-pass successful silicon and provide good yield for chip.

The **OpenRPDK28** is Open RIOS PDK, created by the [RIOS Lab](https://www.rioslab.org/). This PDK is open-source and could be used for a preliminary template for the industrial level PDK.

![image](https://github.com/riosmpw/OpenRPDK28/assets/100336131/0f9578f7-6952-4f26-ba7d-d6dfec5fbe3b)

28nm OpenRPDK Content

**OpenRPDK28 is under constrcuction now**


OpenRPDK28 defines a certain technology variation and characteristic for the 28nm open-source academic processes. Designers may enhance this PDK, tailoring it to their specific design styles and markets.

OpenRPDK28 offers a library of blocks for re-use, each one the result of years of research and development. It will plays a pivotal role in open source EDA and process breakthrough:

1) Access to a OpenRPDK28 means IC designers don’t have to start from scratch. Designer could choose from open-source building blocks which have already proven their efficacy and functionality, resulting in a shorter time to research or market and at lower development costs. 

2) An OpenRPDK28 is crucial in the design phase. 28nm PDK-based designs follow a series of design rules which makes them compliant with 28nm open-source process. 

Designers could use the OpenRPDK28 to design, simulate, draw and verify the integrated circuit design before puting the design back to the foundry to manufacture chips.

![image](https://github.com/riosmpw/OpenRPDK28/assets/100336131/8b3b951a-5c36-41fb-9bce-23d1072cef08)

Open EDA Ecosystem



# Description

Different tools in the design flow have different input formats for the PDK data.

![image](https://github.com/riosmpw/OpenRPDK28/assets/100336131/61d08cb4-57c1-4a23-8941-614b1bfddb0e)




**OpenRPDK28** PDK contains:

-   Technology data

    -   Layers, layer names, layer/purpose pairs

    -   Colors, fills and display attributes

    -   Process constraints

    -   Electrical rules

-   A primitive device library

    -   Symbols

    -   SPICE or Varilog-A model and device parameters

    -   Parameterized cells

-   Rule check files

    -   Design rule checking

    -   Layout versus schematic

    -   Antenna and electrical rule check

    -   Physical parameters extraction

    -   Litho friendly check

    -   Other DFM check

-   Design Rule Manual

    -   A user friendly documents of the process

![image](https://github.com/riosmpw/OpenXPDK28/assets/100336131/89d5dcd0-6f8f-43c8-8960-570019a38714)

Standard Cell Designed with OpenRPDK

# DTCO (Design-Technology Co-Optimization)

Design Technology Co-Optimization (DTCO) is a methodology that helps semiconductor foundries reduce cost and time-to-market in process development. 

In DTCO flow, design and process technology optimized together to improve performance, power efficiency, transistor density, and cost. DTCO for a new technology node usually involves substantial architectural innovation instead of just delivering the similar structure as the previous process node.

![image](https://github.com/riosmpw/OpenRPDK28/assets/100336131/58bf54e3-be74-4ffb-9f95-a8528c1161de)


DTCO Flow (Source: Synopsys)

# DFM (Design for Manufacturing)

As the IC manufacturing enter sub 40nm tech nodes, DFM become more and more important to make sure more stable yield and lower cost. Manufacturing is facing big challenges in terms of manufacturability, yield ramp-up, and variability.

To addresses these challenges, physical verification and implementation technolgies have been augmented with in-design and signoff DFM checks and automated DFM enhancement, then designers can reduce the impact of variability and improve the manufacturability of IC designs. And foundries also need highly accurate modeling and efficient design analysis, yield enhancements, and mask data preparation in their workflow.

![image](https://github.com/riosmpw/OpenRPDK28/assets/100336131/46f7294c-e84c-42cd-9baa-9ad8eb4723f1)


Typical DFM flow:

1) LFD (Litho Fridenly Design)

LFD is the methodology to address the urgent issue of how to accurate manage lithographic process variability in the early stages of design creation.  Accurately LFD could maintain the lithographic processes on “as-drawn” layout data to determine the actual “as-built” dimensions of fabricated gates and metal interconnects.

2) CMP(Chemical-mechanical polishing)

Chemical mechanical polishing (CMP) or planarization is a process of smoothing surfaces with the combination of chemical and mechanical forces. It can be thought of as a hybrid of chemical etching and free abrasive polishing


# IR-Drop and Multi-physics Analysis


# 28nm Process Node

Under the guidance of Moore's Law, the feature length of integrated circuits is constantly reducing.

The 28nm process is between 32nm and 22nm. 2013 was the year of 28nm process popularization. Between 2015 and 2016, the 28nm process began to be used in cell phone application processors and basebands chip at scale. 

The planar process can be most cost-effective at 28nm, and 28nm maybe the best planar process in foundry both in performance and cost-efficiency . For the subsequent 16/14nm FinFET process, the cost of IC manufacturing increases by at least 50%. Only applications with huge amount such as cell phones or processors can support the cost and market size. In many applications, 28nm planar process offers good value for performance, and cost balance. 

![81d00d417c3e3dc179ee0d73a42d95d9_figure-4-amd215821](https://github.com/riosmpw/OpenXPDK28/assets/100336131/20b596a1-bc7d-44ca-b5dd-f306b69e4cb3)

28nm HP 6T-SRAM Example – Plan View SEM (Source: chipworks)



# Main Reference


| Item                   | Type    | Link             | Comment |
|------------------------|---------|------------------|---------|
| google/skywater-pdk    | PDK     | [https://github.com/google/skywater-pdk](https://github.com/google/skywater-pdk)               |         |
| SkyWater SKY130 PDK    | DOC     | [https://skywater-pdk.readthedocs.io](https://skywater-pdk.readthedocs.io)                |         |
| GlobalFoundries 0.18UM 3.3V/(5V)6V MCU PDK | DOC     |[https://gf180mcu-pdk.readthedocs.io/](https://gf180mcu-pdk.readthedocs.io/)         |         |
| globalfoundries-pdk-libs-gf180mcu_fd_pr | PDK     |[https://github.com/efabless/globalfoundries-pdk-libs-gf180mcu_fd_pr](https://github.com/efabless/globalfoundries-pdk-libs-gf180mcu_fd_pr)    |         |
| The OpenLane Documentation    | DOC     |[https://openlane.readthedocs.io/](https://openlane.readthedocs.io）   |         |
| Gate level static timing analyzer    |      | [https://github.com/The-OpenROAD-Project/OpenSTA ](https://github.com/The-OpenROAD-Project/OpenSTA )               |         |
| Neural Networks for Automated Power Delivery Network (PDN) Synthesis    |       | [https://github.com/The-OpenROAD-Project/OpeNPDN ]( https://github.com/The-OpenROAD-Project/OpeNPDN)               |         |
| IR Solver   |       | [https://github.com/The-OpenROAD-Project/OpenROAD/tree/master/src/psm ](https://github.com/The-OpenROAD-Project/OpenROAD/tree/master/src/psm )               |         |



# About RIOS Lab

![image](https://github.com/riosmpw/OpenRPDK28/assets/109063674/6aae13c6-50a5-40c3-9a4e-ed4c79d41c20)


**Ecosystem Wants to be Free**

By David A. Patterson · Director of RIOS Lab

**RISC-V International Open Source Laboratory** (RIOS Lab) is a Shenzhen-based research facility focused on computer system architecture, supported by the Tsinghua-Berkeley Shenzhen Research Institute. As an Open Source and Nobel Prize Laboratory, RIOS Lab promotes open-source innovation and collaboration. Our philosophy is that the computer architecture ecosystem should be free for all to access and build upon.

In November 2019, RIOS Lab was officially unveiled. Under the leadership of 2017 A.M. Turing Award winner Prof. David A. Patterson and operational support from TBSI,  RIOS Lab will conduct cutting-edge research in RISC-V hardware and software technology. Patterson first proposed the Reduced Instruction Set Computer (RISC), an open and free instruction set architecture enabling a new era of processor innovation through open standard collaboration. Released in 2010, the latest Fifth Generation RISC has gained worldwide attention.

The name for the lab RIOS is also inspired by the Spanish word for “rivers.” It symbolizes the flow of information from many sources, coming together to create a whole that is greater than the sum of its parts.


