# LED Control System

![Project Image](Images/screenshot.png)

A simple embedded system that allows you to control LED lighting using Arduino and Raspberry Pi. This project showcases basic embedded programming, hardware interfacing, and understanding of GPIO (General-Purpose Input/Output) pins. You can also interact with the LEDs through push buttons or a mobile app.

## Table of Contents
- [Hardware Components](#hardware-components)
- [Project Overview](#project-overview)
- [Setup](#setup)
  - [Arduino Setup](#arduino-setup)
  - [Raspberry Pi Setup](#raspberry-pi-setup)
- [Usage](#usage)
- [Mobile App Control (Optional)](#mobile-app-control-optional)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Hardware Components

- Arduino (e.g., Arduino Uno)
- Raspberry Pi (e.g., Raspberry Pi 4)
- LEDs (different colors)
- Resistors (220-330 ohms)
- Breadboard and jumper wires
- Push buttons (optional)
- Smartphone or computer (for mobile app control, if desired)

## Project Overview

This project demonstrates how to create a simple embedded system to control LEDs using two popular platforms, Arduino and Raspberry Pi. You can toggle the LED states using push buttons and, if desired, control them via a mobile app.

## Setup

### Arduino Setup

1. Connect the LEDs to the Arduino's GPIO pins:
   - Connect the cathode (shorter lead) of each LED to the GND pin of the Arduino.
   - Connect the anode (longer lead) of each LED to the following GPIO pins on the Arduino:
     - LED 1: Pin 2
     - LED 2: Pin 3
     - LED 3: Pin 4

2. Add current-limiting resistors (220-330 ohms) to each LED anode to prevent excessive current flow.

3. If you're using push buttons:
   - Connect one terminal of each push button to a GPIO pin on the Arduino.
   - Connect the other terminal of each push button to the GND pin.
   - Add pull-up or pull-down resistors (10k ohms) to the GPIO pins connected to the push buttons for stable readings.

4. Upload the Arduino code (arduino_code.ino) to your Arduino board using the Arduino IDE.

### Raspberry Pi Setup

1. Connect the LEDs to the Raspberry Pi's GPIO pins:
   - Connect the cathode (shorter lead) of each LED to the GND pin of the Raspberry Pi.
   - Connect the anode (longer lead) of each LED to the following GPIO pins on the Raspberry Pi:
     - LED 1: GPIO 2
     - LED 2: GPIO 3
     - LED 3: GPIO 4

2. Add current-limiting resistors (220-330 ohms) to each LED anode to prevent excessive current flow.

3. If you're using push buttons:
   - Connect one terminal of each push button to a GPIO pin on the Raspberry Pi.
   - Connect the other terminal of each push button to GND.
   - Ensure you've enabled the internal pull-up resistors for the GPIO pins connected to the push buttons in your code.

## Usage

1. Run the Arduino code on your Arduino board.

2. Execute the Raspberry Pi Python code (raspberry_pi_code.py) on your Raspberry Pi.

3. Use the push buttons to toggle the LED states on both the Arduino and Raspberry Pi.

## Mobile App Control (Optional)

If you wish to control the LEDs via a mobile app:

1. Create a mobile app using a platform like MIT App Inventor, Thunkable, Flutter, or React Native.

2. Establish a Bluetooth or Wi-Fi connection between your mobile app and the Arduino/Raspberry Pi.

3. Implement controls in the mobile app to send commands to the microcontroller to change LED patterns and colors.

## Documentation

For detailed instructions and explanations, please refer to our [documentation](Documentation/README.md).

## Contributing

Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
