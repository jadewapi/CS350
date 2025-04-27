# CS 350 Portfolio Artifacts

## Selected Projects

1. **Thermostat Control System**  
   - A Python-based thermostat prototype using Raspberry Pi, sensors, LEDs, and an LCD display.
   - Manages three states (off, heat, cool) based on real-time temperature readings.
   - Provides visual feedback with LEDs, user controls through buttons, and serial communication to a temperature server.

2. **Morse Code Transmitter**  
   - A Python-based Morse code LED transmitter on Raspberry Pi.
   - Uses red and blue LEDs to blink out messages ("SOS" and "OK") in Morse code.
   - Allows toggling between messages via a button, with a state machine handling transitions.

## Reflection

### Project Summary
These two projects demonstrate my ability to design and implement hardware-software systems on Raspberry Pi. The **Thermostat Control System** automated heating and cooling logic, using a sensor to monitor temperature, LEDs for visual status, and serial communication for reporting data. The **Morse Code Transmitter** converted text into Morse code using LEDs and a state machine, offering hands-on practice with timing, control flow, and user input.

### What I did well
I implemented **state machines** effectively in both projects, which kept the logic organized and easy to manage. The thermostat's heating and cooling transitions worked smoothly alongside the display updates, while the Morse code transmitter handled timing and message toggling without glitches. I also applied **multithreading** to keep processes like LED control and display updates running in parallel, ensuring responsiveness.

### Where I could improve
While the code is functional, I could improve **error handling**, especially for hardware interactions like serial communication and sensor readings. Adding more checks and fallback routines would make the system more robust. I also realized that trimming and refining my comments would help keep the documentation clearer and focused on explaining *why* certain design choices were made.

### Tools and Resources Added to My Support Network
- **gpiozero** for GPIO control on Raspberry Pi.
- **Adafruit sensor libraries** for integrating I2C temperature and humidity sensors.
- **Python threading module** for concurrent tasks.
- Community resources like Raspberry Pi forums and Adafruit documentation for troubleshooting and learning hardware integration.

### Transferable Skills
- **State machine design** for managing hardware states.
- **Multithreading** to handle concurrent hardware tasks.
- **Serial communication** to connect devices and exchange data.
- Hands-on experience with **GPIO hardware interfacing** and **sensor integration**, skills applicable to embedded systems and IoT projects.

### Making the Project Maintainable, Readable, and Adaptable
I structured the code using **modular classes**, like the `ManagedDisplay` for the LCD handling, and kept method names clear and descriptive. The state machines were encapsulated in their own classes, making it easy to expand or modify behavior. This structure allows future changes, like adding new thermostat modes or different Morse code messages, without major rewrites.
