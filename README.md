# ECE484-Pinball-Machine
Creation of a pinball machine as a learning opportunity for embedded system 

## Features
- Graphical Programming: Utilizes PictoBlox, a versatile graphical programming platform with advanced capabilities.
- Custom Design: Detailed instructions for assembling the playfield, control panel, and scoring system.
- Interactive Gameplay: Features like flippers, bumpers, and score sensors enhance the pinball experience.

## Required Materials
- Hardware
- evive Starter Kit
- MDF Sheets and/or Cardboard Sheets
- IR Sensors
- DC Motors
- RGB LED Strip(optional)
- Limit Switches
- Breadboard and various electronic components (Resistors, Standoffs, Rubber Bands, etc.)
- Jumper Cables
- Plastic toy parts
- Cardboard

## Software
- PictoBlox Software ([Link to download PictoBlox](https://thestempedia.com/product/pictoblox))

## Assembly Instructions
- Step 1: Playfield Design
  Start by decorating the base of your playfield. My design is fairly standard and uses black duct tape. This is also to strenghtne the integrity of the cardboard

- Step 2: Building the Structure
  Assemble the boundary walls, score walls, and control panel according to the diagrams provided. I continued to use duct tape to adhear walls to baseplate

 - Step 3: Electronic Setup
   Install motors for flippers and bumpers, set up the IR sensors for score tracking, and connect the control buttons and RGB LED strips.

 - Step 4: Programming
   Program the gameplay and controls using PictoBlox. The code developed is shown above

## Detailed Wiring Guide
 - Infrared (IR) Sensors Connection
   - Connect the signal pin of Score 1 IR Sensor to Digital Pin 8 on the evive.
   - Attach the signal pin of Score 2 IR Sensor to Digital Pin 9 on the evive.
   - Link the signal pin of Score 3 IR Sensor to Digital Pin 10 on the evive.
   - Connect the Drain Wall IR Sensor’s signal pin to Digital Pin 11 on the evive.
   - Connect the Launchpad IR Sensor’s signal pin to Digital Pin 12 on the evive.
   - Finally, connect the VCC and GND pins of all IR sensors to the corresponding VCC and GND on the evive.

 - RGB LED Strip Connection
   - Connect the RGB LED strip to Digital Pin 13 on the evive.

 - Flipper Motors Connection
   - Attach the Left Flipper Motor to the M1 port on the evive.
   - Connect the Right Flipper Motor to the M2 port on the evive.

 - Flippers Control Connection
   - For the Left Side Flipper Switch, connect the “NC” terminal to Digital Pin 2 on the evive and a 10K ohm resistor, then connect the other end of the resistor to GND. Also, connect the “COM” terminal to the VCC on the evive.
   - Similarly, for the Right Side Flipper Switch, connect the “NC” terminal to Digital Pin 3 on the evive and a 10K ohm resistor, then connect the other end of the resistor to GND. The “COM” terminal should also be connected to VCC.

 - Bumper Motors Connection
   - Connect all three Bumper Motors in parallel, connecting one end to the VVR(+) pin and the other end to the “COM” terminal of a Relay. Attach the “NO” terminal of the relay to the VVR(-) pin on the evive.

 - Limit Switches Connection
   - Connect the “NC” terminal of the Left Side Limit Switch (Up) to VCC on the evive, and the COM terminal to Digital Pin 4, also to GND through a 10K ohm resistor.
   - Connect the “NC” terminal of the Left Side Limit Switch (Down) to VCC on the evive, and the COM terminal to Digital Pin 5, also to GND through a 10K ohm resistor.
   - Connect the “NC” terminal of the Right Side Limit Switch (Up) to VCC on the evive, and the COM terminal to Digital Pin 6, also to GND through a 10K ohm resistor.
   - Connect the “NC” terminal of the Right Side Limit Switch (Down) to VCC on the evive, and the COM terminal to Digital Pin 7, also to GND through a 10K ohm resistor.

## Acknowledgements
 - evive ([hardware](https://thestempedia.com/)) can be hard to find, purchased mine on e-bay
 - theSTEMpedia on ([Instructables](https://www.instructables.com/Tabletop-Pinball-Machine-Using-Evive-Arduino-Based/)) 
