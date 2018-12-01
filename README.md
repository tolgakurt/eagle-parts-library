# eagle-parts-library
Simple devices designed from scratch and specialized to fit my custom CNC machine hardware and settings. Will be extended whenever a new part is required in a circuit I wish to make.  

## Parts included in the library
Resistors: Horizontally and vertically placed, 1/4W, 1/2W, and 1W axial, through hole.  
Apolar capacitors: 3.2mm and 5.6mm leg spacings. Also one film capacitor with 17mm leg spacing.  
Electrolytic capacitors: 3.2mm and 5.6mm leg spacings and diameters from 4mm to 13.2mm.  
X2 rated capacitors: 14.7mm, 22.3mm, and 27.6mm leg spacings.  
Transistors: BJT-NPN and BJT-PNP type transistors in TO18 and TO92 packages.  
Rectifier diodes: 1N series in 3 packages.  
Zener diodes: 3.3V to 30V, common package.  
Light emitting diodes: Low power leds with 3.2mm leg spacing and 5mm diameter.  
Terminal connectors: 2 and 3 terminal connectors with 3mm and 5mm leg spacings.  
78xx and LM1117 voltage regulators: In TO220 package.  
LM317 voltage adjuster: In TO220 package.  
TDA2005L integrated cirtcuit: In 11 pin DIP package.  
Fuse mounts: For PCB and box surface.  
Relays: Generic 5 pin relay with 12mm leg spacing in corners and common leg placed in between signal legs.  
Pin/plug connectors: With 2 and 8 (4x2) legs.  
ESP8266E01: Development board.  

## EAGLE settings
Trace width: 0.4mm  
Pads should preferably be circular with a diameter of at least 2.5mm and preferably 3.0mm for easy soldering. However, sometimes the legs should not be bent to achieve these numbers, as in the case of pin/plug connectors with 2.54 mm leg spacings. The number can be diminished to the limits as long as the result fits DRC rules.  
Drill diameters should preferably be 0.1mm more than the lead diameter of the physical parts. However, 0.9mm can be used for most of the parts, even if the lead diameter is 0.5, to avoid tool change.  

## EAGLE DRC rules
Since the isolation step is 0.15mm and maximum isolation distance is set to 0.3mm, the pad perimeters should not be closer than 0.3mm. The traces come out to be generally greater than this, so they should have a minimum spacing of 0.45mm. TODO: check these numbers.   

## EAGLE pcb-gcode settings
Spot drill holes: Off  

Milling depth: -1.5  

Drill depth: -1.7mm (or PCB thickness - 0.2mm)  

Z-down when etching: -0.3mm for Proxxon V bit in 28710 package  

Isolation:  
Min: 0.0  
Max: 0.3mm  
Step size: 0.15mm  

Feed rates in mm/min:  
Etch -> XY: 250, Z: 100  
Drill -> Z: 100  
Mill -> XY: 100, Z: 50  
