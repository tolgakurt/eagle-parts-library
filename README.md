# eagle-parts-library
Simple devices designed from scratch and specialized to fit my custom CNC machine hardware and settings. Will be extended whenever a new part is required in a circuit I wish to make.  

## Parts included in the library
Resistors: Horizontally and vertically placed, 1/4W, 1/2W, and 1W axial, through hole.  
Apolar capacitors: 3.2mm and 5.6mm leg spacings. Also one film capacitor with 17mm leg spacing.  
Electrolytic capacitors: 3.2mm and 5.6mm leg spacings and diameters from 4mm to 13.2mm.  
X2 rated capacitors: 14.7mm, 22.3mm, and 27.6mm leg spacings.  
Transistors: BJT-NPN and BJT-PNP type transistors in TO18 and TO92 packages.  
Rectifier diodes: 1N series in 4 packages.  
Zener diodes: 3.3V to 30V, common package.  
Bridge diodes: Only 2W10 model.  
Light emitting diodes: Low power leds with 3.2mm leg spacing and 5mm diameter.  
Terminal connectors: 2 and 3 terminal connectors with 3mm and 5mm leg spacings.  
78xx and LM1117 voltage regulators: In TO220 package. An additional package for a regular heatsink.  
LM317 voltage adjuster: In TO220 package. An additional package for a regular heatsink.  
TDA2005L IC: In 11 pin DIP package.  
Fuse mounts: For PCB.  
Relays: Generic 5 pin relays in which the common leg is placed in between signal legs.  
Pin/plug connectors: With 1, 2, 3, 4, 5, 6, 7, 8, 4x2, and 8x2 legs.  
ESP8266-01: Development board.  
Enclosed PCB transformers: With single or double primary windings.  
Shortcuts: Since I cannot (and don't want to) print double sided PCBs, but I have to, these will behave as simple shortcuts over the PCB. Now, only a shortcut with 5mm pad spacing exists.  
IC mounts: With 8, 10, 14, and 16 legs.  

## EAGLE settings
Trace width: 0.4mm for signal, 1.0mm for AC line  
Pads should preferably be circular with a diameter of at least 2.0mm and preferably 2.5mm for easy soldering. These number can be diminished to the limits as long as the result fits DRC rules.  
Drill diameters should preferably be 0.1mm more than the lead diameter of the physical parts. However, 0.9mm can be used for most of the parts, even if the lead diameter is 0.5, to avoid tool change.  

## EAGLE DRC rules
Pad perimeters should not be closer than 0.3mm.   

## EAGLE pcb-gcode settings
Bottom side mirror: Off  

Spot drill holes: Off  

Milling depth: -1.5 (if only perimeter will be milled)  
Milling depth: -0.5 (if an inner path will also be milled)  

Drill depth: -1.8mm (or PCB thickness - 0.3mm)  

Z-down when etching: -0.4mm for 15 degree etching bit  

Isolation: single pass  

Feed rates in mm/min:  
Etch -> XY: 250, Z: 100  
Drill -> Z: 100  
Mill -> XY: 150, Z: 100  
