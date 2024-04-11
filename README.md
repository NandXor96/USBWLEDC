# USBWLEDC
USB Sound Reactive WLED Controller

## Features

- USB-C for flashing and power (max. 3A)
- Small size (30mm x 35mm)
- Cheap components
- GSA4737 MEMS Microphone (similar to SPM1423)
- Solder Pads instead of Screw Terminal Blocks
- Files for panelized version (4x4)
- Files for 3D printed case
- Front side can be populated by JLCPCB

<img src="https://github.com/NandXor96/USBWLEDC/blob/main/images/usbwledc_front.png?raw=true" width="250" height="300" /> <img src="https://github.com/NandXor96/USBWLEDC/blob/main/images/usbwledc_back.png?raw=true" width="250" height="300" />

## Case

<img src="https://github.com/NandXor96/USBWLEDC/blob/main/images/usbwledc_case.png?raw=true" width="275" height="375" />

## Entering Flash Mode

To enter the Flash mode of the USBWLEDC, simply hold down the button as you connect the USB cable to a computer.

## WLED Config

| Name | Value |
|------|-------|
| LED Output 1: GPIO | 32 |
| LED Output 2: GPIO | 33 |
| Button 0: GPIO | 0 |
| Digitalmic: Type | Generic I2S PDM |
| Digitalmic: Pin I2S SD | GPIO 23 |
| Digitalmic: Pin I2S WS | GPIO 22 |

## BOM

|Designators   |Footprint                                       |Quantity|Value                  |LCSC Part #|
|--------------|------------------------------------------------|--------|-----------------------|-----------|
|C1*, C2, C4|Capacitor_SMD:C_0603_1608Metric                           |3    |100nF                  |C14663  |
|C3, C5, C7 |Capacitor_SMD:C_0805_2012Metric                           |3    |10uF                   |C15850  |
|C6         |Capacitor_SMD:C_0603_1608Metric                           |1    |1uF                    |C15849  |
|C8         |Capacitor_SMD:CP_Elec_5x5.4                               |1    |100uF                  |C131115 |
|J10        |Connector_USB:USB_C_Receptacle_G-Switch_GT-USB-7010ASV    |1    |USB-C Receptacle       |C2988369|
|MK1*       |Microphone:Microphone-6pin                                |1    |GSA4737 MEMS Microphone|C5142171|
|R1*        |Resistor_SMD:R_0603_1608Metric                            |1    |100k                   |C25803  |
|R2, R3     |Resistor_SMD:R_0603_1608Metric                            |2    |10k                    |C25804  |
|R4, R5     |Resistor_SMD:R_0603_1608Metric                            |2    |5.1k                   |C23186  |
|SW1        |Button_Switch_SMD:SW_Push_1P1T_XKB_TS-1187A               |1    |Push Button Flash      |C318884 |
|U1         |Package_SO:SOP-8_3.9x4.9mm_P1.27mm                        |1    |CH340N                 |C2977777|
|U2         |Package_TO_SOT_SMD:SOT-223-3_TabPin2                      |1    |AMS1117-3.3            |C6186   |
|U3**       |RF_Module:ESP32-WROOM-32                                  |1    |ESP32-WROOM-32         |C701341 |


\* You can build it without the microphone. Then you don't need R1, C1 and MK1.

\*\* The ESP32-WROOM Module can be purchased at a lower cost on AliExpress.

## Assembly

When ordering from JLCPCB, you have the option to get the front side of the board pre-populated - A service I strongly endorse. Subsequently, you'll only need to solder the ESP32-WROOM module onto the reverse side. With sufficient flux, this task can be accomplished with relative ease.

For those looking to populate the whole board, I suggest using a hot plate or a reflow oven for the front side.

    Be careful to keep Isopropyl Alcohol away from the hole of the microphone when cleaning the board!

## Disclaimer

The circuit board provided on this GitHub repository is offered "as is," without any warranties or guarantees of any kind. By accessing and utilizing this circuit board, you acknowledge and agree that you do so at your own risk.

The creator and contributor of this repository, shall not be held responsible or liable for any damages, losses, or injuries that may occur as a result of building and / or using this circuit board. This includes but is not limited to any direct, indirect, consequential, or incidental damages.

Electricity is dangerous. Only attempt this project if you know what you're doing.
