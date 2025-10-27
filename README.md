
# LED Morse Code & Smart Thermostat Projects

## Project Overview
This repository contains two projects demonstrating hardware control with Python:

1. **LED Morse Code Controller (Module 5)**
   - Controls red and blue LEDs to display messages in Morse code.
   - Uses a state machine for LED patterns and button-based message switching.
   - Displays feedback on a 16x2 LCD screen.

2. **Smart Thermostat Prototype (Module 7)**
   - Reads temperature via an I2C sensor and manages system states: off, heating, cooling.
   - Uses LEDs to indicate system status and buttons to adjust the temperature setpoint.
   - Simulates sending data to a server via UART.
   - State machine diagram included for clear visualization of system logic.

## Key Achievements
- Functional state machines for both LED patterns and thermostat operations.
- Smooth hardware interactions using GPIO, I2C, and UART interfaces.
- Modular, well-commented Python code for maintainability and adaptability.


## Areas for Improvement
- **Error handling for sensor or input failures**  
  - The hardware occasionally threw errors during readings, which required additional handling. Several techniques were tested, but ultimately a `try-except` approach was used to catch the errors and prevent them from affecting the user experience.

- **Further modularization for code reuse across projects**  
  - Some functions could have been refactored into reusable libraries to simplify integration in future projects and reduce duplication of code.


## Tools & Resources
- Python with GPIOZero library
- I2C and UART peripherals
- 16x2 LCD display, LEDs, buttons
- Draw.io for state machine diagram creation


## Transferable Skills

This project strengthened several skills that will be valuable for future coursework and projects. Working with the LED Morse code controller and smart thermostat prototype provided hands-on experience in embedded system design and hardware interfacing, including GPIO, I2C, and UART communication. Implementing state machines for both projects improved the ability to structure complex system logic and debug transitions effectively.  

The projects also reinforced best practices in writing maintainable and modular Python code, emphasizing separation of concerns, clear function design, and thorough commenting. Finally, integrating hardware and software components while documenting the process enhanced skills in system-level design, troubleshooting, and producing clear, professional documentation.

## Maintainability & Readability
- **Good documentation:** The code includes clear comments and explanations for each function, state machine transition, and hardware interaction. Additionally, the state machine diagram provides a visual reference that supports understanding and future modifications.  
- **Debugging:** By separating logic from hardware control and using modular functions, the code is easier to debug. Errors in sensor readings or button inputs can be isolated and handled without affecting unrelated parts of the system.  
- **Testing:** Functions and state machine transitions were tested individually and in combination with the hardware to ensure correct behavior. This approach allows for easier verification of each component and reduces the risk of introducing bugs when making changes.  