###  [LINK General guide for laser cutters](../README.md)  
###  [LINK Maintenance](../Maintenance.md)  

# Eduard-x1250
### Laser
9 % seems to be the lowest level, under 9% the laser tube will not fire, it is supposedly rated 120 watts

### Machine
The machine itself is an EDUARD x1250 https://www.eduard.dk/eduart-x1250/ and is based around a Ruida 644XS controller (https://variometrum.hu/pdf/rdc6442g.pdf)

___

## Material cutting parameters guidelines [150W]
| Material                              | Cut params                          |
| ------------------------------------- | ----------------------------------- |
| Cardboard 2 layer                     | 120 mm/s  92%                       |
| Cardboard 3 layer                     | 80 mm/s  92%                        |
| ---                                   | ---                                 |
| MDF 3 mm                              | 18 mm/s  92%                        |
| MDF 6 mm                              | 12 mm/s  92%                        |
| MDF 10 mm                             | 6 mm/s  92%                         |
| ---                                   | ---                                 |
| Plywood 6 mm                          | --5 mm/s -- max 92%, min 92%  <br>--Use high air flow 4bar pressure. <br>-- z-offset 3 mm in <br>-- pwm 0.2kHz <br>-- start end pause time 200 ms cut through = true                                          |
| ---                                   | ---                                 |
| Acrylic 3 mm                          | 20 mm/s 100%                        |
| Acrylic 12 mm                         | 3 mm/s 100%                         |
| ---                                   | ---                                 |
| <span style="color:red">PVC </span>   | <span style="color:red">ABSOLUTELY NEVER EVER CUT PVC. <br>IT PRODUCES TOXIC AND CORROSIVE GASSES THAT IS BAD FOR YOU AND THE MACHINE. </span>                                                              |
| ---                                   | ---                                 |
| Polycarbonate                         | Can not be cut! PC produces bad smelling and toxic gasses. <br>Burns really easily and your cuts will get brown melty edges |

## Material engraving parameters guidelines [150W]
| Material                              | Engrave params                                     |
| ------------------------------------- | -------------------------------------------------- |
| Cardboard 2 layer                     | 520mm/s 25%   -6mm z-offset                        |
| ---                                   | ---                                                |
| MDF                                   | 300mm/s 30% -4mm Z-offset, 0.1mm line interval     |
| MDF Vector engrave                    | 20 mm/s 13% power Z-offset = 2mm in                |
| ---                                   | ---                                                |
| Acrylic Deep engrave                  | 200 mm/s 30% -1 mm Z-offset, 0.1 mm line interval  |
| Acrylic Fine. Good for images         | 500 mm/s 20% 600 dpi/0.041 mm line interval        |
| Acrylic Vector engrave                | 20 mm/s 13% power Z-offset = 2mm in                |
| ---                                   | ---                                                |
| <span style="color:red">PVC </span>   | <span style="color:red">ABSOLUTELY NEVER EVER CUT PVC. <br>IT PRODUCES TOXIC AND CORROSIVE GASSES THAT IS BAD FOR YOU AND THE MACHINE. </span> |
| ---                                   | ---                                                |
| Polycarbonate                         | Can be engraved similarly to Acrylic at slightly lower power but results may varry. Polycarbonate melts and burns easily so be aware. |

