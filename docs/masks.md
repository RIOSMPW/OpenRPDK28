This file provide the mask layer information of current OpenXPDK 28nm process.

The following layers are drawn directly on the layout system.

| Layer Type | Layer Name           | Purpose                                                         | GDS \# | Data type |
|------------|----------------------|-----------------------------------------------------------------|--------|-----------|
| Drawn      | COMP (1)             | Diffusion for device and interconnect                           | 22     | 0         |
| Drawn      | DNWELL               | Deep Nwell                                                      | 12     | 0         |
| Drawn      | Nwell                | Nwell implant                                                   | 21     | 0         |
| Drawn      | LVPWELL              | Pwell implant                                                   | 204    | 0         |
| Drawn      | Dualgate             | 6V Gate Oxide                                                   | 55     | 0         |
| Drawn      | Poly2                | POLY2 gate & interconnect                                       | 30     | 0         |
| Drawn      | Nplus                | Nplus Implant                                                   | 32     | 0         |
| Drawn      | Pplus                | Pplus Implant                                                   | 31     | 0         |
| Drawn      | SAB                  | Unsalicided poly & active regions                               | 49     | 0         |
| Drawn      | ESD (2)              | ESD Implant (Optional)                                          | 24     | 0         |
| Drawn      | Contact              | Metal1 to Active or Poly2 contact                               | 33     | 0         |
| Drawn      | Metal1               | Metal1 interconnect                                             | 34     | 0         |
| Drawn      | Via1                 | Metal2 to Metal1 contact                                        | 35     | 0         |
| Drawn      | Metal2               | Metal2 interconnect                                             | 36     | 0         |
| Drawn      | Via2                 | Metal3 to Metal2 contact                                        | 38     | 0         |
| Drawn      | Metal3               | Metal3 interconnect                                             | 42     | 0         |
| Drawn      | Via3                 | Metal4 to Metal3 contact                                        | 40     | 0         |
| Drawn      | Metal4               | Metal4 interconnect                                             | 46     | 0         |
| Drawn      | Via4                 | Metal5 to Metal4 contact                                        | 41     | 0         |
| Drawn      | Metal5               | Metal5 interconnect                                             | 81     | 0         |
| Drawn      | Via5                 | Metal 6 to Metal5 contact                                       | 82     | 0         |
| Drawn      | MetalTop             | MetalTop interconnect                                           | 53     | 0         |
| Drawn      | Pad (1)              | Bond pad opening                                                | 37     | 0         |
| Drawn      | Resistor (3)         | High sheet rho P-poly resistor (Optional)                       | 62     | 0         |
| Drawn      | FHRES (3)            | Free high sheet rho P-POLY2 resistor                            | 227    | 0         |
| Drawn      | FuseTop (3)          | Top plate of MIM capacitors (Optional)                          | 75     | 0         |
| Drawn      | FuseWindow\_D        | Metal Fuse window (Optional)                                    | 96     | 1         |
| Drawn      | POLYFUSE             | POLY FUSE window (Optional)                                     | 220    | 0         |
| Drawn      | MVSD                 | Define LDNMOS Drain                                             | 210    | 0         |
| Drawn      | MVPSD                | Define LDPMOS Drain                                             | 11     | 39        |
| Drawn      | NAT                  | N-channel native VT mark layer                                  | 5      | 0         |
| Drawn      | COMP\_Dummy          | COMP Dummy fill                                                 | 22     | 4         |
| Drawn      | Poly2\_Dummy         | Poly2 Dummy Fill                                                | 30     | 4         |
| Drawn      | Metal1\_Dummy (4)    | Metal1 Dummy Fill                                               | 34     | 4         |
| Drawn      | Metal2\_Dummy (4)    | Metal2 Dummy Fill                                               | 36     | 4         |
| Drawn      | Metal3\_Dummy (5)    | Metal3 Dummy Fill                                               | 42     | 4         |
| Drawn      | Metal4\_Dummy (5)    | Metal4 Dummy Fill                                               | 46     | 4         |
| Drawn      | Metal5\_Dummy (5)    | Metal5 Dummy Fill                                               | 81     | 4         |
| Drawn      | MetalTop\_Dummy (5)  | MetalTop Dummy Fill                                             | 53     | 4         |
| Drawn      | COMP\_Label (6)      | LABEL drawn at active layer                                     | 22     | 10        |
| Drawn      | Poly2\_Label (6)     | LABEL drawn at poly2 layer                                      | 30     | 10        |
| Drawn      | Metal1\_Label (6)    | LABEL drawn at Metal1 layer                                     | 34     | 10        |
| Drawn      | Metal2\_Label (6)    | LABEL drawn at Metal2 layer                                     | 36     | 10        |
| Drawn      | Metal3\_Label(6)     | LABEL drawn at Metal3 layer                                     | 42     | 10        |
| Drawn      | Metal4\_Label (6)    | LABEL drawn at Metal4 layer                                     | 46     | 10        |
| Drawn      | Metal5\_Label (6)    | LABEL drawn at Metal5 layer                                     | 81     | 10        |
| Drawn      | MetalTop\_Label (6)  | LABEL drawn at MetalTop layer                                   | 53     | 10        |
| Drawn      | Metal1\_Slot         | Metal1 Slot (used to create slots in metal1)                    | 34     | 3         |
| Drawn      | Metal2\_Slot         | Metal2 Slot (used to create slots in metal2)                    | 36     | 3         |
| Drawn      | Metal3\_Slot         | Metal3 Slot (used to create slots in metal3)                    | 42     | 3         |
| Drawn      | Metal4\_Slot         | Metal4 Slot (used to create slots in metal4)                    | 46     | 3         |
| Drawn      | Metal5\_Slot         | Metal5 Slot (used to create slots in metal5)                    | 81     | 3         |
| Drawn      | MetalTop\_Slot       | MetalTop Slot (used to create slots in metal top)               | 53     | 3         |
| Drawn      | UBMPPeri             | Direct Bumping option using peripheral printing                 | 183    | 0         |
| Drawn      | UBMPArray            | Direct Bumping option using Array printing                      | 184    | 0         |
| Drawn      | UBMEPlate            | Direct Bumping option using Electroplating                      | 185    | 0         |
| Drawn      | Schottky\_diode      | Define Schottky diode area                                      | 241    | 0         |
| Drawn      | ZENER                | ZENER diode implant                                             | 178    | 0         |
| Marking    | RES\_MK (1)          | Resistor Mark                                                   | 110    | 5         |
| Marking    | OPC\_drc             | Marking layer for OPC design rule check.                        | 124    | 5         |
| Marking    | NDMY (1)             | Dummy Active Exclude Mark layer                                 | 111    | 5         |
| Marking    | PMNDMY (1)           | Dummy Poly & Metal Exclude Mark                                 | 152    | 5         |
| Marking    | V5\_XTOR (7)         | Define 5V Transistor Marking Layer                              | 112    | 1         |
| Marking    | CAP\_MK (8)          | MIM Capacitor Marking layer                                     | 117    | 5         |
| Marking    | MOS\_CAP\_MK         | MOS capacitor LVS marking                                       | 166    | 5         |
| Marking    | IND\_MK              | Inductor Mark                                                   | 151    | 5         |
| Marking    | DIODE\_MK            | Diode Mark                                                      | 115    | 5         |
| Marking    | DRC\_BJT (9)         | BJT marking for DRC                                             | 127    | 5         |
| Marking    | LVS\_BJT             | BJT Mark                                                        | 118    | 5         |
| Marking    | MIM\_L\_MK           | Min length marking layer for MIM Capacitor                      | 117    | 10        |
| Marking    | Latchup\_MK          | Marking layer for I/O latch-up rule check                       | 137    | 5         |
| Marking    | GUARD\_RING\_MK      | Marking Layer for Scribe Line Guard Ring                        | 167    | 5         |
| Marking    | OTP\_MK              | To define OTP area with Marking layer                           | 173    | 5         |
| Marking    | MTPMARK              | Multi Time Program Memory cell marking                          | 122    | 5         |
| Marking    | NEO\_EE\_MK          | NeoEE OTP area with Marking layer                               | 88     | 17        |
| Marking    | SramCore (10)        | SRAM Mark                                                       | 108    | 5         |
| Marking    | LVS\_RF              | RF LVS Mark                                                     | 100    | 5         |
| Marking    | LVS\_Drain           | RF Drain LVS Mark                                               | 100    | 7         |
| Marking    | IND\_MK1             | Inductor Mark                                                   | 151    | 5         |
| Marking    | HVPOLYRS             | High Voltage Poly2 Resistor in HV area Marking layer            | 123    | 5         |
| Marking    | LVS\_IO              | IO LVS Mark                                                     | 119    | 5         |
| Marking    | PROBE\_MK            | Marking layer for probe pad                                     | 13     | 17        |
| Marking    | ESD\_MK              | Marking layer on ESD protection device                          | 24     | 5         |
| Marking    | LVS\_Source          | Source LVS/DRC marking Layer                                    | 100    | 8         |
| Marking    | WELL\_DIODE\_MK      | Marking layer for Nwell/Psub, LVPwell/Dnwell, DNwell/Psub diode | 153    | 51        |
| Marking    | LDMOS\_XTOR          | LDMOS device mark layer                                         | 226    | 0         |
| Marking    | PLFUSE               | Marking layer for eFUSE Link                                    | 125    | 5         |
| Marking    | EFUSE\_MK            | Marking layer for whole eFUSE Element                           | 80     | 5         |
| Marking    | MCELL\_FEOL\_MK (13) | Marking layer to define YMTP Mcell Implant region               | 11     | 17        |
| Marking    | YMTP\_MK (13)        | Marking layer to define YMTP Cell and exclude NLDD region       | 86     | 17        |
| Marking    | DEV\_WF\_MK          | LVS marking layer for Fab special purposes layout               | 128    | 17        |
| EDAMark    | Metal1\_BLK          | Place & Route Metal1 Blockage                                   | 34     | 5         |
| EDAMark    | Metal2\_BLK          | Place & Route Metal2 Blockage                                   | 36     | 5         |
| EDAMark    | Metal3\_BLK          | Place & Route Metal3 Blockage                                   | 42     | 5         |
| EDAMark    | Metal4\_BLK          | Place & Route Metal4 Blockage                                   | 46     | 5         |
| EDAMark    | Metal5\_BLK          | Place & Route Metal5 Blockage                                   | 81     | 5         |
| EDAMark    | MetalT\_BLK          | Place & Route MetalTop Blockage                                 | 53     | 5         |
| EDAMark    | PR\_bndry            | PR Boundary for cell, block or chip                             | 0      | 0         |
| EDAMark    | MDIODE               | MDiode Mark                                                     | 116    | 5         |
| EDAMark    | Metal1\_Res (11)     | Metal 1 Resistor                                                | 110    | 11        |
| EDAMark    | Metal2\_Res (11)     | Metal 2 Resistor                                                | 110    | 12        |
| EDAMark    | Metal3\_Res (11)     | Metal 3 Resistor                                                | 110    | 13        |
| EDAMark    | Metal4\_Res (11)     | Metal 4 Resistor                                                | 110    | 14        |
| EDAMark    | Metal5\_Res (11)     | Metal 5 Resistor                                                | 110    | 15        |
| EDAMark    | Metal6\_Res (11)     | Metal6 Resistor                                                 | 110    | 16        |
| DevMark    | Border               | Border                                                          | 63     | 0         |



| Term | Definition         |
|---------------------|-----------------------------|
| NCOMP               | COMP AND Nplus              |
| PCOMP               | COMP AND Pplus              | 
| Field               | NOT COMP                    |
| Transistor gate     | Poly2 AND COMP              | 
| N-channel gate      | Nplus AND Poly2 AND COMP    | 
| P-channel gate      | Pplus AND Poly2 AND COMP    | 
