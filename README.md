# linux-based-scout-uav
 Linux based scout UAV

 LinuxベースのスカウトUAV

# What it is:
Hobby project to create a UAV (Unmanned aerial vehicle) in a quadcopter drone format, based on the OSD32MP1 SiP which is a Linux capable system. 

# Requirements & components
![](/doc/requirements_components_v0.6.jpg.jpeg)

# Block diagram

The system block diagram is still a work in progress.
Still looking for a good option on ESC (electronic speed controller) for the drone. Maybe CAN bus based systems can be used as there is a CAN bus available in the OSD32MP1 SiP. 

![](/doc/block_diagram_v0.7.jpg.jpeg)

# Software/Firmware 

## Operating system 

Octavo develops and mantains a Debian based image that supports their development boards.  I plan to start prototyping with this image. 

## Device tree

I will base my work on Octavo's OSD32MP1-BRK device tree and modify it as needed. 

## Cortex M4

The SiP has an embedded ARM Cortex M4 sub-system which can be used by creating firmware in ST Cube IDE. 

# Hardware 

## Schematic capture

Started working on the schematic capture, schematic in PDF format will be added as it is updated. 

## Board layout 

Started work on board by trying board shapes and importing the DXF files. Already placed the initial components available, will update as needed. 

## EDA

Hardware being designed in KiCad 8.0

# License

Released under the Creative Commons Attribution 4.0 License
https://creativecommons.org/licenses/by/4.0/
