# eagle-parts-library
Simple parts designed customly to fit my custom CNC machine.  

## Parts included
Resistors: Horizontally placed, 1/4W and 1/2W axial, through hole.  
TODO: Vertically placed resistors  
TODO: Capacitors  
TODO: LEDS, Diodes and transistors  
TODO: 3mm and 5mm connectors with 2 and 3 terminals  
TODO: DIP8 chips with 8 and 16 legs  
TODO: 5 pin relays  

## EAGLE settings
Trace width: 0.4mm  
Pads: Circle with diameter of 2.5mm, drill diameters are according to lead diameter of the parts.  

## EAGLE pcb-gcode settings
Spot drill holes: -0.3mm  

Isolation:  
Min: 0.0  
Max: 0.2mm  
Step size: 0.2mm  

Z-down: -0.3mm for Proxxon V bit in 28710 package  

Feed rates in mm/min:  
Etch -> XY: 200, Z: 100  
Drill -> Z: 100  
Mill -> XY: 100, Z: 50  

Drill depth: 1.7mm (or PCB thickness + 0.2mm)  
