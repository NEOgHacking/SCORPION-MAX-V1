# 3D printer / CNC Mainboard
<img width="1024" height="1024" alt="LOGO SCORPION MAX V1" src="https://github.com/user-attachments/assets/78c953fb-4a00-4f39-add0-f267267d94c1" />
A main-board for a 3d printer or CNC with wide possibilities with the use of the expansion board and thermister boards to not get locked in to one type of thermister or display. I started this design to place it into my Ultimaker 2+ for better Stepper drivers and more options. Also in the future I want to make a cnc and this would be the perfect board for this application. This whole idea started about the 15 of December very close to the deadline of blueprint, recently it got extended but its still a LOT to do. For compatibility i went with overkill amounts of everything and some expansion headers. Also because there are a lot of different thermister available i made an port for a thermister board where you could place the board for your thermister to have wide compatibility. There are also a bunch of extra stuff: 5x Stepper motor drivers 4x Bed / Nozzle heater output 4x Fan / Led output 4x End stops 3x Thermisters 3x Thermister boards 1x Expansion port (for displays, sd card readers or extra stuf)
<img width="3840" height="2160" alt="PCB SCORPION MAX V1" src="https://github.com/NEOgHacking/SCORPION-MAX-V1/blob/main/Pictures/Renders/SCORPION-MAX-V1.png" />

# Reason
So long story longer I have an ultimaker 2+ laying at home doing nothing because of the noisy stepper drivers and recently getting an ultimaker S5 so I wanted to make it quieter and more useful. I was amazed by the Prusa mini being so quiet so I thought why not build my own mainboard, also I am planing to build a CNC somewhere in the future so I thought it would be a genius idea to build my own 3D printer / CNC mainboard with my own overkill specs and the best stepper drivers.

# Specs
5x Stepper driver TMC2130

4x Power Mosfets for controlling beds, heaters, ext.

4x Fan controller with tacho input

4x Limit switches for homing

3x Thermister inputs with possibilities for NTC's and PTC's

2x Safety inputs for disabling cutting power via a relay to the stepper drivers and mosfets

Expansion port for displays, sd cards, ext.

STM32H743VIT6 for big storage and calculation power

Standard 4 pin power connector and 2 pin screw terminal

USB ports, USB-C for programming and external control and USB-A for USB flash drives

# Schematic
There are 3 schematics for this project:
1. Main board
2. Thermister modules
3. Expansion module

These are way to long to display here (14 pages) so in the PCB folder there in folder for the board you want to see there is a pdf file of the schematic

# PCB

Main board

<img width="791" height="1213" alt="image" src="https://github.com/user-attachments/assets/9d89f777-38f0-4c66-9863-240889c675c4" />

Thermister boards

<img width="773" height="1210" alt="image" src="https://github.com/user-attachments/assets/f7b15966-5c3e-4ec2-b687-ad664149b507" />

Expansion board

<img width="793" height="1207" alt="image" src="https://github.com/user-attachments/assets/5762f186-36b8-47c7-b935-f281b614ceeb" />

# BOM
The BOM is located in the BOM folder because its way to long to display here

# Credits
@Kai Pereira for all my random questions regarding PCB design and blueprint custom project. and for telling me long journals are the best, sorry for the short ones at the beginning. whoops.
Henk, someone i know that is way better in PCB design that me that looked over my schematic and layout ext.
