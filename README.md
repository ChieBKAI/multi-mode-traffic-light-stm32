# Traffic Light Control System

Traffic Light Control System
This project is a traffic light control system implemented using an STM32 microcontroller. The system simulates the operation of a traffic light at a crossroad, with features for controlling the timing of the red, amber, and green lights, as well as displaying the current mode and time duration on seven-segment LEDs.

## Features

- 12 LEDs representing the traffic lights (4 red, 4 amber, 4 green)
- 4 seven-segment LEDs for displaying time duration (2 for each road)
- 3 buttons for mode selection, time duration adjustment, and value setting
- 4 modes:
  - Normal mode: Traffic lights operate in a regular cycle
  - Modify red light time duration
  - Modify amber light time duration
  - Modify green light time duration
## Requirements
- STM32 microcontroller board
- Proteus schematic for circuit connections
- Timer interrupt set to 10ms

## Usage
1. Connect the circuit as per the Proteus schematic.
2. Upload the code to the STM32 microcontroller.
3. The system will start in normal mode (Mode 1).
4. Press the first button to cycle through the modes (1 to 4, then back to 1).
5. In modes 2, 3, and 4:
    - The corresponding color LEDs will blink at 2 Hz.
    - Two seven-segment LEDs will display the mode.
    - The other two seven-segment LEDs will display the time duration value.
    - Use the second button to increase the time duration value (range: 1-99).
    - Use the third button to set the chosen time duration value.

## Implementation
The project consists of several exercises:
1. Sketch a finite state machine (FSM) for the system.
2. Draw a Proteus schematic for the circuit connections.
3. Create an STM32 project with timer interrupt set to 10ms.
4. Modify timer parameters for adjustable interrupt duration without affecting the overall system.
5. Add code for button debouncing and mode selection.
6. Add code for displaying modes and blinking LEDs based on the selected mode.
7. Add code for adjusting the time duration of the red LEDs.
8. Add code for adjusting the time duration of the amber LEDs.
9. Add code for adjusting the time duration of the green LEDs.
