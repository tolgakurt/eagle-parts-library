# eagle-parts-library
Simple devices designed from scratch and specialized to fit my custom CNC machine hardware and settings.  

## Parts included in the library
Resistors: Horizontally placed, 1/4W and 1/2W axial, through hole.  
TODO: Vertically placed resistors  
TODO: Capacitors  
TODO: LEDS, Diodes and transistors  
TODO: Connectors with 2 and 3 terminals which have 3mm or 5mm spans  
TODO: DIP8 chips with 8 and 16 legs  
TODO: 5 pin relays  

## EAGLE settings
Trace width: 0.4mm  
Pads should preferably be circular with a diameter of at least 2.5mm  
Drill diameters should preferably be 0.1mm more than the lead diameter of the physical parts.  

## EAGLE pcb-gcode settings
Spot drill holes: -0.2mm  

Drill depth: -1.7mm (or PCB thickness - 0.2mm)  

Z-down when etching: -0.3mm for Proxxon V bit in 28710 package  

Isolation:  
Min: 0.0  
Max: 0.2mm  
Step size: 0.2mm  

Feed rates in mm/min:  
Etch -> XY: 200, Z: 100  
Drill -> Z: 100  
Mill -> XY: 100, Z: 50  
