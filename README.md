# CS-350
# Morse Code State Machine (Milestone 3)

## Overview
This project demonstrates a Python-based state machine for transmitting messages in Morse code using a Raspberry Pi. It controls two LEDs (red and blue) to visually represent dots and dashes and uses a physical button to toggle between two messages ("SOS" and "OK"). The artifact, `Milestone3.py`, serves as a practical example of embedded systems programming through the integration of hardware control, state machine logic, and user interaction.

## Project Summary

### What problem was it solving?
The project addresses the challenge of interfacing software with hardware to communicate messages in Morse code. By leveraging GPIO pins on a Raspberry Pi, the solution visually transmits messages using LEDs and allows dynamic message switching via a button press. This demonstrates how software can precisely control hardware components and manage state transitions in real time.

### What did you do particularly well?
- **Object-Oriented Design**: The project is structured using object-oriented principles, making the code modular and easy to extend.
- **State Machine Design**: The implementation of state machine logic via classes (`ManagedDisplay`, `CWMachine`) encapsulates hardware control and state transitions effectively.
- **Debugging Support**: Clear debug messaging was implemented, aiding in the development and troubleshooting process.
- **Asynchronous Input Handling**: The system handles user input (button presses) asynchronously, ensuring the main transmission logic isn't blocked.

### Where could you improve?
- **Exception Handling**: The handling of hardware exceptions and edge cases, such as rapid button presses or hardware failures, could be more robust.
- **Pending Refinements**: Some `TODO` sections indicate areas for further improvement, such as completing state transitions and ensuring precise timing requirements are met.

### What tools and/or resources are you adding to your support network?
For this project, I expanded my knowledge of the following tools and libraries:
- **Libraries**:
  - `gpiozero` and `digitalio` for GPIO management.
  - `statemachine` for implementing state machines in Python.
  - `adafruit_character_lcd` for LCD control.
  - `Threading` for concurrent execution.
- **Resources**:
  - Official documentation for the above libraries.
  - Community forums for troubleshooting hardware integration issues.

### What skills from this project will be particularly transferable to other projects and/or course work?
- **State Machine Design**: Modeling and implementing state transitions is valuable for any system requiring predictable, event-driven behavior.
- **Hardware-Software Integration**: Experience in interfacing Python code with physical components is directly applicable to IoT, robotics, and embedded systems.
- **Multithreading**: Managing concurrent tasks (e.g., transmission and user input) is a key skill for responsive applications.
- **Code Readability and Maintainability**: Structuring code for clarity and future modification is universally beneficial.

### How did you make this project maintainable, readable, and adaptable?
- **Clear Class Structure**: Hardware and logic are encapsulated in dedicated classes for better organization.
- **Descriptive Comments and Docstrings**: Each major section and method is well-documented, providing context for developers.
- **Modular Design**: Concerns such as display, state machine, and button handling are separated, making updates and testing more straightforward.
- **Debugging Support**: A `DEBUG` flag allows for verbose output during development and troubleshooting.
- **Extensible State Machine**: The state machine can be easily extended to support additional messages or hardware behaviors.

## Usage

### Hardware Setup
1. Connect the LEDs, button, and LCD to the specified GPIO pins on a Raspberry Pi.
2. Refer to the `Milestone3.py` file for GPIO pin assignments and setup details.

### Running the Code
1. Execute `Milestone3.py` on the Raspberry Pi.
2. The system will transmit the active message in Morse code using LEDs.
3. Press the button to toggle between "SOS" and "OK".

## Artifact Location
All project files are available in this repository. See `Milestone3.py` for the main implementation.

## Conclusion
This artifact showcases my ability to design and implement a responsive, hardware-integrated application using Python. It highlights my skills in state machine modeling, hardware interfacing, and writing maintainable code—key competencies for roles in embedded systems and emerging technology development.
