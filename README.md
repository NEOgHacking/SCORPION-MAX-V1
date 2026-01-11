# 3D printer / CNC Mainboard
<img width="3840" height="2160" alt="PCB SCORPION MAX V1" src="https://github.com/NEOgHacking/SCORPION-MAX-V1/blob/main/Pictures/Renders/SCORPION-MAX-V1.png" />
A main-board for a 3d printer or CNC with wide possibilities with the use of the expansion board and thermister boards to not get locked in to one type of thermister or display. I started this design to place it into my Ultimaker 2+ for better Stepper drivers and more options. Also in the future I want to make a cnc and this would be the perfect board for this application. This whole idea started about the 15 of December very close to the deadline of blueprint, recently it got extended but its still a LOT to do. For compatibility i went with overkill amounts of everything and some expansion headers. Also because there are a lot of different thermister available i made an port for a thermister board where you could place the board for your thermister to have wide compatibility. There are also a bunch of extra stuff: 5x Stepper motor drivers 4x Bed / Nozzle heater output 4x Fan / Led output 4x End stops 3x Thermisters 3x Thermister boards 1x Expansion port (for displays, sd card readers or extra stuf)

# Reason
So long story longer I have an ultimaker 2+ laying at home doing nothing because of the noisy stepper drivers and recently getting an ultimaker S5 so I wanted to make it quieter and more useful. I was amazed by the Prusa mini being so quiet so I thought why not build my own mainboard, also I am planing to build a CNC somewhere in the future so I thought it would be a genius idea to build my own 3D printer / CNC mainboard with my own overkill specs and the best stepper drivers.

# Specs
5x Stepper driver TMC2130

4x Power Mosfets for controlling beds, heaters, ext.

4x Fan controller with tacho input

4x Limit switches for homing

3x Thermister inputs with possibilities for NTC's and PTC's
  These possibilities are posible because of the 2 thermister boards i have designed, and the NTC thermister board has a solder jumper to select the resistance of you NTC.

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

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/43165db2-4d8f-4cc0-9059-1ee0730a7d48" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/52caef36-1e10-4eb2-ac98-f21f186d6244" />


Thermister boards

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/c14a4ed3-f2bb-43c3-bbb0-4784e126a25b" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/dab7153a-a234-427c-9592-91ccd7a6a961" />


Expansion board

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/d631b2df-7358-48ad-856a-71c7ff6eed91" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/bd1ac5fb-a070-4766-a22c-e94fdb3c53dc" />

# Panelization
I have panelized the thermister boards for better price per board, the panel still is under the 100x100 limit for the 2 dollar offer on jlcpcbway so its still very cheap. I needed 6 thermisters for 2 boards and minimum order quantity on jlcpcb is 5, so i made a panel.

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/842d4744-9c13-46f3-a9d8-be3a0595093c" />


# BOM
I have made a bom for LCSC and a global bom for all the parts and pcbs these are in the BOM folder

# Credits
@Kai Pereira for all my random questions regarding PCB design and blueprint custom project. and for telling me long journals are the best, sorry for the short ones at the beginning. whoops.
Henk, someone i know that is way better in PCB design that me that looked over my schematic and layout ext.
