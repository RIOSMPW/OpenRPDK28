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


# Reference

https://xschem.sourceforge.io/stefan/xschem_man/xschem_elements.html

