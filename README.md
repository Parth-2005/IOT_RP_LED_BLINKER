# LED Blinker with Raspberry Pi Pico W

Welcome to my first IoT project! This repository contains the code and instructions for creating a simple LED blinker using the Raspberry Pi Pico W.

## Project Overview

This project demonstrates the basics of IoT and microcontroller programming by making an LED blink at regular intervals. It serves as an introductory project for those looking to get started with IoT and the Raspberry Pi Pico W.

## Hardware Requirements

- Raspberry Pi Pico W
- LED
- Breadboard
- Jumper wires
- Resistor (to protect the LED)

## Software Requirements

- [MicroPython](https://micropython.org/) (for programming the Raspberry Pi Pico W)
- [Thonny IDE](https://thonny.org/) (for code execution and deployment)

## Circuit Diagram

Here's how to connect the components:

1. Connect the anode (longer leg) of the LED to GPIO pin 15 on the Raspberry Pi Pico W.
2. Connect the cathode (shorter leg) of the LED to one end of a resistor.
3. Connect the other end of the resistor to the ground (GND) pin on the Raspberry Pi Pico W.

## Code

The following MicroPython code will make the LED blink at 1-second intervals:

```python
from machine import Pin
from time import sleep

led = Pin(15, Pin.OUT)

while True:
    led.toggle()
    sleep(1)
```

## Setup Instructions

1. **Install MicroPython**:
   - Follow the [official guide](https://docs.micropython.org/en/latest/rp2/quickref.html) to install MicroPython on your Raspberry Pi Pico W.

2. **Install Thonny IDE**:
   - Download and install Thonny IDE from [here](https://thonny.org/).

3. **Upload the Code**:
   - Open Thonny IDE.
   - Connect your Raspberry Pi Pico W to your computer via USB.
   - Copy the provided code into Thonny.
   - Save the file as `main.py` on the Raspberry Pi Pico W.
   - Run the code.

## How It Works

The code initializes GPIO pin 15 as an output pin and then enters an infinite loop. Within the loop, it toggles the state of the LED (on/off) and pauses for 1 second using the `sleep` function. This creates a blinking effect with the LED.

## Future Improvements

- Add a button to control the LED blinking.
- Integrate more LEDs with different blinking patterns.
- Explore using sensors and actuators for more advanced projects.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Contributions and suggestions are always welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

A big thank you to the IoT community for the resources and support available online. 

## Connect with Me

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/parth-panot-005b01245/) if you have any tips, resources, or just want to discuss all things IoT!
