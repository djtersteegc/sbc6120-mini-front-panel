![cased](docs/sbc6120-mini-front-panel-cased.jpg)

Project thread at https://forum.vcfed.org/index.php?threads/sbc6120-mini-front-panel.1245272/

# Switches

The current PCB and dress panel are drilled for miniature toggles with a 6mm diameter bushing/stem.  1/4-40 switches will NOT fit since I wanted a tight fit on the dress panel and the switches are spaced to tightly to use the dress nuts.  Plus I think this stype looks nicer (same as an Altair).

These are commonly listed as MTS-102 (ON-ON) and MTS-112 (ON-Momentary ON) on Aliexpress.  I tried all the different red and blue models and ended up using the ones linked below in the BOM.  Total cost shipped to the US for twenty MTS-102 and ten MTS-112 switches was less than ten bucks, versus the $40 it would cost to buy something like E-Switch 100 Series which was the cheapest domestic option I could find.  C&K 7000 series were over $160 for 20 minature toggles.  Maybe the action is a bit better, but at the end of the day this is a toy for me, so I would personally rather spend the budget on the next project.

# Electrical BOM

There's an interactive BOM [here](https://djtersteegc.github.io/sbc6120-mini-front-panel/ibom.html), and CSV version with footprint info [here](https://djtersteegc.github.io/sbc6120-mini-front-panel/bom.html).

I  buy pretty much everything from UTSource (for logic) or AliExpress suppliers these days with the exception of the capacitors (whatever is on clearance at Newark) and the rotary switch is only available from C&K.  If you are shopping local everything should be available from Mouser/DigiKey/Newark with the exception of the Amtel GAL chips.

C16 is a bulk storage cap for the 5V line.  I speced it at 470uF, but anything from 100uF and up will probably be fine.  You may not even really need it.

| Component                                       | Qty  | Notes                | Link                                                         |
| ----------------------------------------------- | ---- | -------------------- | ------------------------------------------------------------ |
| 10nF Ceramic Capacitor                          | 1    | 5.08mm Lead Spacing  | [AliExpress](https://www.aliexpress.us/item/2251832786944590.html) |
| 100nF Ceramic Capacitor                         | 13   | 5.08mm Lead Spacing  | [AliExpress](https://www.aliexpress.us/item/2251832786944590.html) |
| 1uF Ceramic Capacitor                           | 1    | 5.08mm Lead Spacing  | [AliExpress](https://www.aliexpress.us/item/2251832786944590.html) |
| 470uF 16V Electrolytic Capacitor                | 1    | 3.5mm Lead Spacing   | [Newark](https://www.newark.com/multicomp-pro/mcmr16v477m8x9/cap-470uf-16v-alu-elec-radial/dp/39T1477) |
| 10K 1/4W Resistor                               | 3    |                      | [AliExpress](https://www.aliexpress.us/item/2251832766343175.html) |
| 17.4K 1/4W Resistor                             | 2    |                      | [AliExpress](https://www.aliexpress.us/item/2251832766343175.html) |
| 560R SIP9 Resistor Network                      | 4    | I used 510R          | [AliExpress](https://www.aliexpress.us/item/3256801607747550.html) |
| 4.7K SIP5 Resistor Network                      | 1    |                      | [AliExpress](https://www.aliexpress.us/item/2251832653789055.html) |
| 4.7K SIP6 Resistor Network                      | 3    |                      | [AliExpress](https://www.aliexpress.us/item/2251832653789055.html) |
| 4.7K SIP7 Resistor Network                      | 3    |                      | [AliExpress](https://www.aliexpress.us/item/2251832653789055.html) |
| 5mm LED (Red)                                   | 28   |                      | [AliExpress](https://www.aliexpress.us/item/2255800226642152.html) |
| Subminature ON-ON Toggle                        | 13   | MTS-102 - 6mm Stem   | [AliExpress](https://www.aliexpress.us/item/3256805560180852.html) |
| Subminature ON-(ON) Momentary Toggle            | 7    | MTS-112 - 6mm Stem   | [AliExpress](https://www.aliexpress.us/item/3256802276750993.html) |
| SPDT Right Angle Slide Switch                   | 1    | 2.54mm Spacing       | [AliExpress](https://www.aliexpress.us/item/2251832665517359.html) |
| C&K RM104772BCB Rotary Switch                   | 1    | 4 Position           | [Newark](https://www.newark.com/c-k-components/rm104772bcb/rotary-switch-1p-0-5a-24v-45deg/dp/69AH1990) |
| 74HC05                                          | 1    |                      |                                                              |
| 74HC74                                          | 1    |                      |                                                              |
| 74HC174                                         | 2    |                      |                                                              |
| 74HC366                                         | 4    |                      |                                                              |
| 74HC373                                         | 2    |                      |                                                              |
| 7555 Timer                                      | 1    |                      |                                                              |
| ATF16V8                                         | 1    |                      | UTSource/Ali/eBay                                            |
| ATF22V10                                        | 1    |                      | UTSource/Ali/eBay                                            |
| 2x25 2.54mm Pin Header                          | 1    |                      | [AliExpress](https://www.aliexpress.us/item/2251832485909733.html) |
| 1x2 2.54mm Pin Socket                           | 1    | Cut down a 40p strip | [AliExpress](https://www.aliexpress.us/item/2251832484668248.html) |
| 5.08mm 2p Terminal Block (or original 4P Molex) | 1    | KF301-2P             | [AliExpress](https://www.aliexpress.us/item/2251832480927324.html) |

# Mechanical BOM

| Component                      | Qty  | Notes                | Link                                                         |
| ------------------------------ | ---- | -------------------- | ------------------------------------------------------------ |
| 12mm M3 Standoff               | 5    | SBC6120 to Panel     | 3D Print                                                     |
| 15.6mm M3 Standoff             | 7    | Panel to Dress Panel | 3D Print                                                     |
| 2mm High M3 Rubber Bumpers     | 7    | TS-2.7 Option        | [AliExpress](https://www.aliexpress.us/item/3256805089368820.html) |
| M3 x 6mm Taper Head Screws     | 16   |                      | [AliExpress](https://www.aliexpress.us/item/3256801858523146.html) |
| M2.5 x 6mm Taper Header Screws | 6    |                      | [AliExpress](https://www.aliexpress.us/item/3256801858523146.html) |
| 15mm Diameter Knob             | 1    | "Plum Shaft" Option  | [AliExpress](https://www.aliexpress.us/item/2251832788673272.html) |

# Other Parts

| Component                              | Notes              | Link                                                         |
| -------------------------------------- | ------------------ | ------------------------------------------------------------ |
| IDE to CF Adapater                     | CF-IDE40 or HX-168 | [AliExpress](https://www.aliexpress.us/item/3256804514420229.html) |
| DB9 to IDC 10                          | May need to rewire | [AliExpress](https://www.aliexpress.us/item/3256803077047244.html) |
| 5.5 x 2.1mm DC Input Jack for 8mm Hole | DC-025M            | [AliExpress](https://www.aliexpress.us/item/2255801022148508.html) |

# Case

TBD

# Assembly

TBD