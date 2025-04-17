# linux-based-scout-uav
 Linux based scout UAV

 LinuxベースのスカウトUAV

# What it is:
Hobby project to create a UAV (Unmanned aerial vehicle) in a quadcopter drone format, based on the OSD32MP1 SiP which is a Linux capable system. 

Linux 対応システムである OSD32MP1 SiP をベースに、クアッドコプター ドローン形式の UAV (無人航空機) を作成する趣味のプロジェクト。

# Requirements & components
![](/doc/requirements_components_v0.6.jpg.jpeg)

# Block diagram

The system block diagram is still a work in progress.
Still looking for a good option on ESC (electronic speed controller) for the drone. Maybe CAN bus based systems can be used as there is a CAN bus available in the OSD32MP1 SiP. 

![](/doc/block_diagram_v0.8.jpeg)

System block diagram
![](/doc/system_block_diagram_v0.1.jpeg)

# Software/Firmware 

## Operating system 

Octavo develops and mantains a Debian based image that supports their development boards.  I plan to start prototyping with this image. 

## Device tree

I will base my work on Octavo's OSD32MP1-BRK device tree and modify it as needed. 

# Hardware 

## OSD32MP1 SiP

Based on the OSD32MP1: 

    ST32MP15x Features:
    Arm® Cortex®-A7 up to 800MHz x2
    Arm® Cortex®-M4 up to 209MHz
    NEON™SIMD Coprocessor x2
    USB 2.0 HS + PHY x2
    Ethernet 10/100/1000
    CAN FD/TTCAN x2, UART x4, USART x4,SPI x6, I2C x6, SAI x4, QSPI, SPDIF, I2S x3
    eMMC/SD/SDIO Ports x3
    GPIO x148
    24-bit RGB Display, MIPI DSI
    Camera Interface
    22 Channel 16-bit ADC x2, 12-bit DAC x2
 
The SiP has an embedded ARM Cortex M4 sub-system which can be used by creating firmware in ST Cube IDE. 

## Schematic capture

Started working on the schematic capture, schematic in PDF format will be added as it is updated. 

## Board placement/layout 

Started work on board by trying board shapes and importing the DXF files. Already placed the initial components available, will update as needed. 

![](/doc/3d-viewer.JPG)

![](/doc/ratnest-placement.JPG)


## EDA

Hardware being designed in KiCad 8.0

# License

Released under the Creative Commons Attribution 4.0 License
https://creativecommons.org/licenses/by/4.0/
