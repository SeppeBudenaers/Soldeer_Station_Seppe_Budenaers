# Soldeer_Station_Seppe_Budenaers
The purpose of this project is to build a soldering station able to fit the JBC C245 soldering iron. The design relies on the soldering station described in the Elektor magazine (issue 507) (Elektor Magazine, 2021), which provided a good basis to start from. However, some modifications were brought in to enable it to suit the JBC C245. For instance, replacing the power supply by a bigger one and adding a Hirose connector.

"Elektor's PCB (Printed Circuit Board) leans more towards hobbyists as it utilizes only THT (Through-Hole Technology) components. For this project, the PCB was designed with SMT (Surface-Mount Technology) in mind to simulate the way the electronic industry designs their PCB.
# Bill of Material 
| item             | store              | Package          | price/unit | amount | total price |
|------------------|--------------------|------------------|------------|--------|-------------|
| Resistors        |                    |                  |            |        |             |
| 47 ohm           | lcsc               | 805              | € 0,0015   | 28     | € 0,0420    |
| 18 Kohm          | lcsc               | 805              | € 0,0010   | 3      | € 0,0030    |
| 1 Mohm           | lcsc               | 805              | € 0,0015   | 1      | € 0,0015    |
| 68 Kohm          | lcsc               | 805              | € 0,0016   | 1      | € 0,0016    |
| 5,6 Kohm         | lcsc               | 805              | € 0,0014   | 4      | € 0,0056    |
| 10 Kohm          | lcsc               | 805              | € 0,0010   | 6      | € 0,0060    |
| 100 ohm          | lcsc               | 805              | € 0,0018   | 3      | € 0,0054    |
| 10 Mohm          | lcsc               | 805              | € 0,0014   | 1      | € 0,0014    |
| 4,7 Kohm         | lcsc               | 805              | € 0,0015   | 6      | € 0,0090    |
| Inductor         |                    |                  |            |        |             |
| L1               | lcsc               | 805              | € 0,1271   | 1      | € 0,1271    |
| L2               | Mouser             | 2545             | € 2,3000   | 1      | € 2,3000    |
| Capacitor        |                    |                  |            |        |             |
| 4700 uF          | lcsc               | D25xL25mm plugin | € 0,8289   | 1      | € 0,8289    |
| 10 uF            | lcsc               | D4XL5,4          | € 0,0237   | 3      | € 0,0711    |
| 100 nF           | lcsc               | 805              | € 0,0023   | 6      | € 0,0138    |
| 100 uF           | lcsc               | SMD,D8xL10mm     | € 0,1362   | 2      | € 0,2724    |
| 10 nF            | lcsc               | 805              | € 0,0033   | 7      | € 0,0231    |
| Semiconductors   |                    |                  |            |        |             |
| 1n4007           | lcsc               | SOD-123Fl        | € 0,0048   | 1      | € 0,0048    |
| Zener            | lcsc               | SOD-123Fl        | € 0,0127   | 1      | € 0,0127    |
| 1n14148          | lcsc               | SOD-123Fl        | € 0,0064   | 1      | € 0,0064    |
| Brug             | lcsc               | TTF              | € 0,3166   | 2      | € 0,6332    |
| BC847C           | lcsc               | SOT-23           | € 0,0146   | 3      | € 0,0438    |
| MOSFET-P 30v     | Mouser             | TO-263-3(DPAK)   | € 1,2900   | 1      | € 1,2900    |
| MOSFET-P 20V     | lcsc               | TO-252-2(DPAK)   | € 0,2785   | 1      | € 0,2785    |
| BC857C           | lcsc               | SOT-23           | € 0,0231   | 1      | € 0,0231    |
| DC/DC            | Mouser             | OKI78SR8         | € 7,0500   | 1      | € 7,0500    |
| MCP6002-E/MS     | Mouser             | MSOP-8           | € 0,4400   | 1      | € 0,4400    |
| Mircocontroler   | Mouser             | TQFP-48          | € 1,8200   | 1      | € 1,8200    |
| relay            | Mouser             | RT424005f        | € 5,3800   | 1      | € 5,3800    |
| IC2 7seg         | lcsc               | SOP-20           | € 0,1861   | 1      | € 0,1861    |
| encoder          | lcsc               | PEC11R4220F      | € 1,6500   | 1      | € 1,6500    |
| Ledfilament      | aliexpress         | 20MM             | € 0,2915   | 28     | € 8,1620    |
| fuse             | Mouser             | 5x20mm           | € 0,4230   | 1      | € 0,4230    |
| pcb              |                    |                  |            |        | € 0,0000    |
| sevensegment     | JCLPCB             |                  | € 0,5153   | 4      | € 2,0613    |
| soldeerbout      | JLCPCB             |                  | € 0,7280   | 1      | € 0,7280    |
| SMT stencil      | JLCPCB             |                  | € 6,3800   | 1      | € 6,3800    |
| others           |                    |                  |            |        |             |
| glass tube       | aliexpress         | D30mm            | € 0,6592   | 4      | € 2,6367    |
| switch           | aliexpress         | 29x13x54mm       | € 1,7300   | 1      | € 1,7300    |
| screw terminal   | aliexpress         | Pitch 5mm        | € 0,0880   | 4      | € 0,3520    |
| testpoints       | Mouser             | 3,5x1,78mm       | € 0,4230   | 7      | € 2,9610    |
| ac connector     | Mouser             | 24x30mm          | € 2,3200   | 1      | € 2,3200    |
| hirose connector | Mouser             | 20x20mm          | € 2,9000   | 1      | € 2,9000    |
| triplex 6mm      | Makerspace Hasselt |                  | € 6,0000   | 1      | € 6,0000    |
| shipping + tax   |                    |                  |            |        |             |
| mouser           | mouser             |                  | € 58,7500  | 1      | € 58,7500   |
| lcsc             | lcsc               |                  | € 15,0200  | 1      | € 15,0200   |
| JLCPCB           | JLCPCB             |                  | € 30,6750  | 1      | € 30,6750   |
| price total      |                    |                  |            |        | € 163,63    |