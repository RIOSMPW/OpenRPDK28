# Design for Manufacture

Design for Manufacture (DFM) is a set of guidelines that aim to optimize the design of a chip for efficient and cost-effective manufacturing. The goal of DFM is to ensure that the chip can be produced at scale, with minimal production costs, and without compromising on quality.

DFM tool involves collaboration between the design team and the manufacturing team from the early stages of product development. This collaboration ensures that the design takes into account the manufacturing process  and tooling, among other factors.
![0b1d1430a1bbd24c2e0532469c81715e_Manufacturing-design-pattern-library-from-Full-chip-mask-data-simulation-Systematic](https://github.com/RIOSMPW/OpenRPDK28/assets/100336131/a4c702ac-a5f8-4d7e-9568-b43ca1f178bb)

Manufacturing design pattern library from Full chip mask data simulation & Systematic defect detection on Silicon. (Source:Jean-Christophe Le Denmat )


Chip design establishes a chip’s vulnerability to defect-induced yield loss. The design optimization guidelines described in this section were generated following the development and use of critical area analysis tools on a wide variety of designs. Following these guidelines helps ensure:

1) Faster technology and product development because manufacturing sites typically target CA and V1  images at upper specification limits and metal spacing near lower specification limits to prevent open  circuits.

2) Improved yields because the resulting designs will be less sensitive to the random manufacturing defects  that impact yield.

3) More chips that fulfill the specifications sooner.

4) Fewer process variations, especially for contacts.

5) Fewer parasitics and improved circuit performance

Design for manufacturability does not always require drastic changes. Every change, including a change of  only one grid point, can help. The following general recommendations will help improve the manufacturability  of a design:

1) Do not compromise on area; use existing empty space.
   
3) Use the recommended rules wherever possible.

4) Increase space and width equally wherever possible.

5) For long, parallel metal or polysilicon lines, use wider spacing. (A long line is approximately 50 times the  minimum design length.


![image](https://github.com/RIOSMPW/OpenRPDK28/assets/100336131/1986b1b2-7826-459a-970a-5ac6969c0ffb)

Optical simulation of Litho( Source: Yorick Trouiller)

## 4.1 Yield Enhancement Design Techniques

1) Space out elements as much as possible.
Unless this approach grows the design beyond the available space, move elements as far apart as possible. If the design is wiring-limited, spread out the devices, and vice versa. If white space exists, use it.

![image](https://github.com/RIOSMPW/OpenRPDK28/assets/100336131/685eb9b2-53ca-4514-928d-4701a505ccec)


