# OpenXPDK28

![rios-ip](https://github.com/riosmpw/OpenXPDK28/assets/100336131/9f3d5cb0-e9f8-48c8-b4e6-38c896d54da8)

**Process design kit** (**PDK**) is a set of files or models used within the semiconductor industry to model a fabrication process characteristic for the design tools and its users used to design an integrated circuit. An accurate PDK will increase the chances of first-pass successful silicon and provide good yield for chip.

The **OpenXPDK28** is created by the [RIOS Lab](https://www.rioslab.org/). This PDK is open-source and could be used for a preliminary template for the industrial level PDK.

![image](https://github.com/riosmpw/OpenXPDK28/assets/100336131/fdc4ddf9-8764-43c2-9938-640eadb82325)



OpenXPDK28 defines a certain technology variation and characteristic for the 28nm open-source academic processes. Designers may enhance this PDK, tailoring it to their specific design styles and markets.

OpenXPDK28 offers a library of blocks for re-use, each one the result of years of research and development. It will plays a pivotal role in open source EDA and process breakthrough:

1) Access to a OpenXPDK28 means IC designers don’t have to start from scratch. They can choose from open-source building blocks which have already proven their efficacy and functionality, resulting in a shorter time to research or market and at lower development costs. 

2) A OpenXPDK28 is crucial in the design phase. 28nm PDK-based designs follow a series of design rules which makes them compliant with 28nm open-source process. 

Designers could use the OpenXPDK28 to design, simulate, draw and verify the integrated circuit design before puting the design back to the foundry to manufacture chips.

![image](https://github.com/riosmpw/OpenXPDK28/assets/100336131/8b3b951a-5c36-41fb-9bce-23d1072cef08)

Open EDA Ecosystem

# Description

Different tools in the design flow have different input formats for the PDK
data.

**OpenXPDK28** PDK contains:

-   Technology data

    -   Layers, layer names, layer/purpose pairs

    -   Colors, fills and display attributes

    -   Process constraints

    -   Electrical rules

-   A primitive device library

    -   Symbols

    -   SPICE model and device parameters

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

# Reference


| Item                   | Type    | Link             | Comment |
|------------------------|---------|------------------|---------|
| google/skywater-pdk    | PDK     | [https://github.com/google/skywater-pdk/tree/main](https://github.com/google/skywater-pdk/tree/main)               |         |
| SkyWater SKY130 PDK    | DOC     | [https://skywater-pdk.readthedocs.io](https://skywater-pdk.readthedocs.io)                |         |
|       |      |                  |         |




