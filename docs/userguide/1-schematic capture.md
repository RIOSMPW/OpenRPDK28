# XSCHEM ELEMENTS

## SYMBOLS
Symbols are graphical elements that represent electrical components. A symbol represents an electronic device, like for example a resistor, a bipolar transistor, an amplifier etc. As you can see graphically symbols are built with lines, rectangles, polygons and texts, the graphical primitives shown before. In the picture below some components are placed in a schematic window. Components are instances of symbols. For example you see three placements of the 'npn' bipolar transistor symbol. Like in C++, where objects are instances of classes, here components are instances of symbols.

![492ce4fae41d7153a3cad57ae1df84df_xschem_symbols](https://github.com/riosmpw/OpenRPDK28/assets/100336131/ff877469-51b1-4ee6-b859-2b42515ea8c1)


## WIRES

Wires in XSCHEM are the equivalent of copper traces in printed circuit boards or electrical conductors. Wires are drawn as lines but the electrical connectivity graph is built by XSCHEM. To draw a wire segment point the mouse somewhere in the drawing window and press the 'w' key. A rubber wire is shown with one end following the mouse. Clicking the left mouse button finishes the placement. The following picture shows a set of connected wires. There are many wire segments but only 3 electrical nodes. XSCHEM recognizes connection of wires and uses this information to build up the circuit connectivity. All wires are drawn on the 'wire' layer. One electrical node in the picture below has been highlighted in red (this is a XSCHEM function we will cover later on).

![7984efe9c3daa6e90b3735dd7e6253b1_xschem_wires](https://github.com/riosmpw/OpenRPDK28/assets/100336131/31228215-8381-4da5-8a92-cd942ded4198)

## LINES

Lines are just segments that are used for drawing. Lines do not have any electrical meaning, in fact when building the circuit netlist, lines are completely ignored. XSCHEM uses different layers to draw lines. Each layer has its own color, allowing to draw with different colors. Lines are placed like wires, but using the 'l' key. The 'Layers' menu allows to select various different layers (colors) for the line.

![3783d4b934e54dc1841895a81f77d01b_xschem_lines](https://github.com/riosmpw/OpenRPDK28/assets/100336131/3170a6b8-5bbd-441a-8ff6-baf8fff30dcd)

## TEXT

Text can be placed with the 't' bindkey. A dialog box appears where the user inputs the text and text size.

![d73159a32450e6fc9dcf0c1bbe1a1c11_xschem_texts](https://github.com/riosmpw/OpenRPDK28/assets/100336131/dd5c31c9-5305-4def-8182-527b9f0289fa)

The layer property can be used to draw text on a different layer, for example, setting layer=6 will draw on cyan color. A font property is defined to change the default font. A hcenter=true attribute may be set to center text in the reading direction, while vcenter=true centers text in the perpendicular (to reading) direction. the 2 attributes may be set both to get full centered text box.
A weight=bold attribute may be given for bold text, while a slant=italic or slant=oblique may specify italic or slanted text.
A hide=true will make the specified text invisible when the symbol is displayed as a component in a schematic.

![a02e8d97dfea608036fd0cd0959e42ac_xschem_elements_02](https://github.com/riosmpw/OpenRPDK28/assets/100336131/95b57255-8216-42be-a097-0290e0511efd)

# CREATING A CIRCUIT SCHEMATIC

To create a new circuit start from an empty window, run xschem and select New Schematic in the File menu. Suppose we want co create a NAND gate, with two inputs, A and B and one output, Z. Lets start placing the input and output schematic pins; use the Insert key and locate the devices/ipin.sym symbol. After placing it change its lab attribute to 'A'

![76e5141b3ea5d6e32d15b88a061d9fb2_creating_schematic1](https://github.com/riosmpw/OpenRPDK28/assets/100336131/b7061b45-db47-4bde-95f2-2df2c04709aa)

Copy another instance of it and set its lab attribute to B. Next place an output pin devices/opin.sym and set its lab to Z. The result will be as follows:

![e0979d37986e50390489378468dea062_creating_schematic2](https://github.com/riosmpw/OpenRPDK28/assets/100336131/45a15821-f89b-451b-874b-d378be25e143)

Now we need to build the actual circuit. Since we plan to do it in CMOS technology we need nmos and pmos transistors. Place one nmos from devices/nmos4.sym and one pmos from devices/pmos4.sym By selecting them with the mouse, moving (m bindkey), copying ('c' bindkey) place 4 transistors in the following way (the upper ones are pmos4, the lower ones nmos4):

![c625c6dbdd08a4a298bb2c9ac0bda127_creating_schematic3](https://github.com/riosmpw/OpenRPDK28/assets/100336131/e5273dc2-da7d-49e7-a63a-368baaf12c39)


now draw wires to connect together the transistor to form a NAND gate; in the picture i have highlighted 2 electrical nodes by selecting one wire segment of each and pressing the 'k' bindkey.


![848ee184998a2c30eb46ed783737d2fb_creating_schematic4](https://github.com/riosmpw/OpenRPDK28/assets/100336131/fc05c276-4ebf-49f8-a9d7-b9f902f61f8e)

Next we need to place the supply nodes , VCC and VSS. we decide to use global nodes. Global nodes in SPICE semantics are like global variables in C programs, they are available everywhere, we do not need to propagate global nodes with pins. We could equally well use regular pins , as used for the A and B inputs, I am just showing different design styles. Use the Insert key and place both devices/vdd.sym and devices/gnd.sym Since the default names are respectively VDD and GND use the edit property bindkey 'q' to change these to VCC and VSS.

![266b3c38b645bbe58c4e5eb4b2e22111_creating_schematic5](https://github.com/riosmpw/OpenRPDK28/assets/100336131/0b78f783-658b-431e-bc6c-aa6e6f294e7a)

we still need to connect the body terminals of the mos transistors. One possibility is to hookup the two upper pmos transistor terminals to VCC with wires, and the two bottom nmos terminals to VSS with wires, but just to show different design styles i am planning to use ''by name'' connection with labels. So place a wire label devices/lab_pin.sym and use 4 instances of it to name the 4 body terminals. Remember, while moving (select and press the 'm' key) you can flip/rotate using the R/F keys.


![415ef4e2b0f7324178b701704f89e772_creating_schematic6](https://github.com/riosmpw/OpenRPDK28/assets/100336131/eb625905-8b89-410c-8d5a-548f093b2408)


Finally we must connect the input and output port connectors, and to complete the gate schematic we decide to use W=8u for the pmos transistors. Select both the pmos devices and press the edit proprty 'q' key; modify from 5u (default) to 8u.

![f9f385fb909b695ba5f6eda08bc7ac6a_creating_schematic7](https://github.com/riosmpw/OpenRPDK28/assets/100336131/b0c832f7-831e-44b9-857d-c60b968e90d2)

Now do a Save as operation, save it for example in mylib/nand2.sch.
To make the schematic nicer we also add the title component. This component is not netlisted but is useful, it reports the modification date and the author. Place the devices/title.sym component. The NAND gate is completed! (below picture also with grid, normally disabled in pictures to make image sizes smaller).




# Reference

https://xschem.sourceforge.io/stefan/xschem_man/xschem_elements.html

https://xschem.sourceforge.io/stefan/xschem_man/creating_schematic.html

