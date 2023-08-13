# USBWLEDC
USB Sound Reactive WLED Controller

## Features

- USB-C Power supply (max. 3A)
- Small size
- Cheap components
- ICS-43434 MEMS Microphone (optional)
- Solder Pads instead of Screw Terminal Blocks

<img src="https://github.com/NandXor96/USBWLEDC/blob/main/images/front.png?raw=true" width="250" height="300" /> <img src="https://github.com/NandXor96/USBWLEDC/blob/main/images/back.png?raw=true" width="250" height="300" />

## BOM

|Designator    |Part                                            |Quantity|Value                  |LCSC Part #| Mouser Part # |
|--------------|------------------------------------------------|--------|-----------------------|-----------|---------------|
|C1*, C2, C4   |0805 MLCC                                       |3       |100nF 50V              |C49678     ||
|C3, C7        |0805 MLCC                                       |2       |22uF 25V               |C45783     ||
|C5            |0805 MLCC                                       |1       |10uF 25V               |C15850     ||
|C6            |0805 MLCC                                       |1       |1uF 50V                |C28323     ||
|C8            |D8.0mm P3.50mm ELKO                             |1       |330uF 25V              |C3008476   ||
|J10           |USB-C Receptacle                                |1       |USB_C_Receptacle_USB2.0|C2988369   ||
|MK1*          |InvenSense_ICS-43434 MEMS Microphone            |1       |ICS-43434              |           |410-ICS-43434|
|R1*           |0805 Resistor                                   |1       |100k                   |C149504    ||
|R2, R3        |0805 Resistor                                   |2       |10k                    |C17414     ||
|R4, R5        |0805 Resistor                                   |2       |5.1k                   |C27834     ||
|SW1           |Tactile Switch 6x3.5mm                          |1       |SWITCH                 |C3726366   ||
|U1            |USB-UART IC CH340N                              |1       |CH340N                 |C2977777   ||
|U2            |3.3V LDO AMS1117-3.3                            |1       |AMS1117-3.3            |C6186      ||
|U3            |ESP32-WROOM-32 D or E                           |1       |ESP32-WROOM-32         |C701341    |356-ESP32WRM32E132PH|

\* You can build it without the microphone. Then you don't need R1, C1 and MK1.

## Assembly

To assemble the PCB, I recommend using a hot plate or soldering oven for the upper side, and hand-soldering for the ESP32 on the back.
**Preheat** the PCB before soldering anything by hand and use a **powerful soldering iron**!  

## Disclaimer

The circuit board provided on this GitHub repository is offered "as is," without any warranties or guarantees of any kind. By accessing and utilizing this circuit board, you acknowledge and agree that you do so at your own risk.

The creator and contributor of this repository, shall not be held responsible or liable for any damages, losses, or injuries that may occur as a result of building and / or using this circuit board. This includes but is not limited to any direct, indirect, consequential, or incidental damages.

Electricity is dangerous. Only attempt this project if you know what you're doing.
