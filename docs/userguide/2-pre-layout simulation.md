# ngspice

ngspice is a circuit simulator that numerically solves equations describing (electronic) circuits: These are made of passive and active devices. Time varying currents and voltages are simulated as well as noise and small signal behavior. ngspice is the Open Source successor of the venerable spice3f5 from UC at Berkeley.

![9b71e463bd51a9206bc8178207623268_intro1](https://github.com/riosmpw/OpenRPDK28/assets/100336131/70f7b48a-7f3b-4d5e-bcd7-552957776eb4)


Fig. 1

As shown in Fig. 1, you start with a circuit (here: an inverter). You have to create a netlist describing this circuit. The netlist is the input to ngspice, telling it about the circuit to be simulated. Together with some simulation commands this input cares for reading and parsing the netlist, starting the simulation and plotting the output. The output voltage (plotted in red) is the inverse of the (green) input. Both voltages are plotted versus time.

The input to ngspice is read from a file, and it may be enhanced by commands given on the command line. The simulated output may be written to a file, or be plotted as a y-x graph or a smith chart. There is no graphical user interface with schematic capture of circuit diagrams and automatic netlist generation, however there are third party tools available to draw the circuit and generate a ngspice netlist.


# Reference

https://ngspice.sourceforge.io/ngspice-tutorial.html
