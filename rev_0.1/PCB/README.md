## Description
A bare-bones hexagon-shaped LED panel with recillinear LED spacing. Uses SK9822-A LEDS in a 4-wire serial configuration and serpentine routing. Can be manufactured with a single copper layer on PCB materials such as aluminum for better heat dissipation. Clock and Data input pins are positioned at the top of the board with daisy-chainable outputs at the bottom. Similarly, there are two contacts for 5V and GND on each end of the board.

![alt text](img/render_rev0.1.png)

## Specifications
- 107x SK9822-A LEDs
- 5V operating voltage
- 2mm-pitch solderable pads for Clock and Data signal lines (input and output)
- 0-ohm jumpers for clean power traces and low-impedence return path to ground

## Caution
With all onboad LEDs set to full bright white, the total current draw of the panel can be up to 5.5A! Even on aluminium substrate, this is far too much power for the small board to dissipate safely. 5V fans or heatsinks can be attached to the back of the aluminum board for better heat distribution and the ability to run brighter for longer without overheating.

Use caution and limit the current draw to 2-3A in firmware when possible and avoid running the LEDs at full white for extended periods. Always use a physical fuse (2-3A) on the input power supply line to prevent hardware failures or firmware glitches from exceeding the recomended current draw and safety margins. 
