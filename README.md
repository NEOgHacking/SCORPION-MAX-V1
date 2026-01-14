# 3D printer / CNC Mainboard
<img width="3840" height="2160" alt="PCB SCORPION MAX V1" src="https://github.com/NEOgHacking/SCORPION-MAX-V1/blob/main/Pictures/Renders/SCORPION-MAX-V1.png" />
A main board for a 3d printer or CNC with wide possibilities with the use of the expansion board and thermistor boards! This board is based on the STM32H743 for its massive power. And everyone hates loud stepper motors, so it uses the TMC2130 silent stepper drivers, these are not only very quiet but have a lot of other functions!

# Reason
So long story longer I have an ultimaker 2+ laying at home doing nothing because of the noisy stepper drivers and recently getting an ultimaker S5 so I wanted to make it quieter and more useful. I was amazed by the Prusa mini being so quiet, so I thought why not build my own mainboard with way more quiet stepper drivers and more functions. The second reason is that I am planning to build a CNC somewhere in the future so I thought it would be a genius idea to build my own 3D printer / CNC mainboard with my own overkill specs and the best stepper drivers. And most of all A LOT of power in amps and compute!

# Specs
5x Stepper driver TMC2130

4x Power Mosfets for controlling heated beds, heaters, ext.

4x Fan controller with tacho input

4x Limit switches for homing

3x Thermistor inputs with possibilities for NTC's and PTC's
  These possibilities are possible because of the 2 thermistor boards I have designed, and the NTC thermistor board has a solder jumper to select the resistance of you NTC.

2x Safety inputs for disabling cutting power via a relay to the stepper drivers and mosfets

Expansion port for displays, SD cards, ext.

STM32H743VIT6 for big storage and calculation power

Standard 4 pin power connector and 2 pin screw terminal

USB ports, USB-C for programming and external control and USB-A for USB flash drives

# Design
This board is designed with a lot of safety features and well thought out design, it has a safety circuit to cut power to the steppers and heaters, good pcb design, followed design recommendation from datasheets, used the right components, and allot more! The pcb has been designed with the right trace width and good trace layout with no sharp bends. Also have good pcb layout.
# Schematics
There are 3 schematics for this project:
1. Main board
2. Thermistor modules
3. Expansion module

These are way too long to display here (14 pages) so in the PCB folder there in folder for the board you want to see there is a pdf file of the schematic, but here are a few.
<img width="2000" height="1414" alt="Printer Mainboard page 1" src="https://github.com/user-attachments/assets/057f2683-0a0b-43bf-b409-4fbbd7585089" />
<img width="2000" height="1414" alt="Printer Mainboard page 9" src="https://github.com/user-attachments/assets/7a6da1a1-000d-45e8-9d8b-16ca31f195a4" />
<img width="2000" height="1414" alt="Printer Mainboard page 10" src="https://github.com/user-attachments/assets/6e5a2f28-ed79-4aae-bbf1-3c1e7deba906" />
<img width="2000" height="1414" alt="Expansion board" src="https://github.com/user-attachments/assets/478c7bf2-6cee-4eb3-a968-4431a25ee28c" />
<img width="2000" height="1414" alt="PTC" src="https://github.com/user-attachments/assets/84e0e13c-a185-4221-bb72-271f29c23621" />
<img width="2000" height="1414" alt="NTC" src="https://github.com/user-attachments/assets/2d8213a4-8334-43ca-a30f-642f86d53528" />



# PCB

Main board

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/43165db2-4d8f-4cc0-9059-1ee0730a7d48" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/52caef36-1e10-4eb2-ac98-f21f186d6244" />


Thermistor boards

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/c14a4ed3-f2bb-43c3-bbb0-4784e126a25b" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/dab7153a-a234-427c-9592-91ccd7a6a961" />


Expansion board

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/d631b2df-7358-48ad-856a-71c7ff6eed91" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/bd1ac5fb-a070-4766-a22c-e94fdb3c53dc" />

# Penalization
I have panelized the thermistor boards for better price per board, the panel still is under the 100x100 limit for the 2 dollar offer on jlcpcb so it’s still very cheap. I needed 6 thermistors for 2 boards and minimum order quantity on jlcpcb is 5, so I made a panel.

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/842d4744-9c13-46f3-a9d8-be3a0595093c" />

# Firmware
The firmware provided is Marlin, but I plan to expand this to more firmware’s like Clipper ext. The board is based on the STM32H743 so it's very powerful and can run almost any firmware!

# BOM
I have made a BOM for LCSC and a global BOM for all the parts and PCBs these are in the BOM folder
The price of the LCSC BOM for all the parts is about 180 dollars for 2 boards and the JLCPCB order is at the 54 dollar.
This is not the cheapest board but it does have the most functions!

# Credits
@Kai Pereira for all my random questions regarding PCB design and blueprint custom project. and for telling me long journals are the best, sorry for the short ones at the beginning. whoops.
Henk, someone I know that is way better in PCB design than me that looked over my schematic and layout ext.
