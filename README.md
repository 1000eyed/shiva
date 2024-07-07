# SHIVA
A 12U 40% keyboard supporting multiple layouts, offset space bar row, and LEDs.

![Front1](img/PXL_20240621_071407905.PORTRAIT.jpg)

## About

This keyboard supports as many different layouts as possible. Currently supported are: ortho, alpha stagger, uniform 0.25U stagger, normal stagger, plus multiple space row configurations. After all, you got 5 PCBs. Note: only alpha stagger is tested.
- designed around Gateron KS27/KS33 low profile switches.
- rotary encoder support.
- bluetooth connection only. USB connection possible with an appropriate case.
- leds to display connection/battery status.
- nice!nano MCU.
- ZMK keyboard firmware support.
- open source.

## KLE

See possible configurations below:
![](img/shiva-kle.png)

## How to build one

I provide all the production files you will need in order to assemble the keyboard. In [prod](prod/) folder you will find the PCB gerbers and STLs for case (only one configuration is supported now). I intended the case to be CNC'd from PC, however it is not tested yet and only 3D printed it so far. There are no build instructions, as everything should be self-explanatory.

### Part list
| #     | name                 | comments                                  |
|-------|----------------------|-------------------------------------------|
| 1     | main PCB             | Order at fabricator of your choice        |
| 1     | Nice!nano v2         | Controller board. Make sure you have enough sockets for all pins. |
| 1     | EC11                 | Rotary Encoder through hole style (optional)         |
| ~45   | 1N4148 - SOD-123     | Diodes                                    |
| 3     | LED 3mm              | Choose red, yellow (orange), and green        |
| 1     | MSK-12C02            | Power switch                              | 
| 1     | JST 1.25mm pitch     | Battery connector, 2pin. I used S2B-PH-K-S(LF)(SN)        |
| 1     | 3.7V LiPo            | Battery                     |
| ~45   | KS33 or KS27         | Gateron Low Profile switches              |
| ~45   | Keycaps              | MX-compatible keycaps of your choice      |

My personal ZMK config: https://github.com/1000eyed/zmk-config-shiva

## Open source

In [source](source/) directory you will find the source files for the PCB and the case. You may use them however you like, I kindly ask you though to link back to my project, should you build it or update something.

## Gallery

![](img/PXL_20240621_071457859.PORTRAIT.jpg)
![](img/PXL_20240621_071651733.PORTRAIT.jpg)
![](img/PXL_20240621_071921859.PORTRAIT.jpg)
![](img/PXL_20240609_154801265.PORTRAIT.jpg)
