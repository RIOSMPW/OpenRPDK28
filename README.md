# OpenXPDK28

**Process design kit** (**PDK**) is a set of files or models used within
the semiconductor industry to model a fabrication process characteristic for the
design tools and its users used to design an integrated circuit. An accurate PDK
will increase the chances of first-pass successful silicon and provide good
yield for chip.

The **OpenXPDK28** is created by the RIOS Lab. This PDK is open-source and could
be used for a preliminary template for the industrial level PDK.

OpenXPDK28 defines a certain technology variation and characteristic for the
28nm open-source academic processes. Designers may enhance this PDK, tailoring
it to their specific design styles and markets.

Designers could use the OpenXPDK28 to design, simulate, draw and verify the
integrated circuit design before puting the design back to the foundry to
manufacture chips.

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

    -   SPICE model and Device parameters

    -   Parameterized Cells

-   Rule check files

    -   Design rule checking

    -   Layout versus schematic

    -   Antenna and electrical rule check

    -   Physical parameters extraction

    -   Litho friendly check

    -   Other DFM check

-   Design Rule Manual

    -   A user friendly documents of the process
