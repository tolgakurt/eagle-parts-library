# eagle-parts-library
Simple devices designed from scratch and specialized to fit my custom CNC machine hardware and settings.  

## Parts included in the library
Resistors: Horizontally placed, 1/4W, 1/2W, and 1W axial, through hole.  
Resistors: Vertically placed, 1/4W, 1/2W, and 1W axial, through hole.  
Capacitors: Apolar capacitors with 3.2mm and 5.6mm leg spacings. Also one film capacitor with 17mm leg spacing. Electrolytic capacitors 3.2mm and 5.6mm leg spacings and diameters from 4mm to 13.2mm.  
Transistors: BJT-NPN and BJT-PNP type transistors with TO18 and TO92 packages.  
TODO: LEDS and Diodes  
TODO: Connectors with 2 and 3 terminals which have 3mm or 5mm spans  
TODO: DIP8 chips with 8 and 16 legs  
TODO: 5 pin relays  

## EAGLE settings
Trace width: 0.4mm  
Pads should preferably be circular with a diameter of at least 2.5mm and preferably 3.0mm for easy soldering.  
Drill diameters should preferably be 0.1mm more than the lead diameter of the physical parts. However, 0.9mm can be used for most of the parts, even if the lead diameter is 0.5, to avoid tool change.  

## EAGLE pcb-gcode settings
Spot drill holes: -0.2mm  

Drill depth: -1.7mm (or PCB thickness - 0.2mm)  

Z-down when etching: -0.3mm for Proxxon V bit in 28710 package  

Isolation:  
Min: 0.0  
Max: 0.3mm  
Step size: 0.15mm  

Feed rates in mm/min:  
Etch -> XY: 150, Z: 100  
Drill -> Z: 100  
Mill -> XY: 100, Z: 50  
