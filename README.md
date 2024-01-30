# Arduino Radar Visualization

An Arduino project for visualizing distance measurements using an ultrasonic sensor and servo motor, with a Processing sketch for real-time graphical representation.

## Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Hardware Setup](#hardware-setup)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project combines Arduino and Processing to create a radar-like visualization of distance measurements. The Arduino code reads data from an ultrasonic sensor and a servo motor, while the Processing sketch renders a real-time graphical representation of the measurements.

## Requirements

- Arduino board (e.g., Arduino Uno)
- Ultrasonic sensor (e.g., HC-SR04)
- Servo motor
- Arduino IDE
- Processing IDE

## Hardware Setup

1. Connect the ultrasonic sensor to the Arduino:
   - Connect VCC to 5V on Arduino.
   - Connect GND to GND on Arduino.
   - Connect Trig to digital pin 10 on Arduino.
   - Connect Echo to digital pin 11 on Arduino.
   
2. Connect the servo motor to the Arduino:
   - Connect VCC to 5V on Arduino.
   - Connect GND to GND on Arduino.
   - Connect Signal to digital pin 12 on Arduino.

![Circuit Diagram](https://github.com/Churanta/Arduino-Radar-Visualization/assets/83538805/6a5d7944-218f-468c-b349-20ddcc07158d)

## Installation

1. Upload the Arduino code (`Arduino_Radar.ino`) to your Arduino board using the Arduino IDE.
2. Open the Processing sketch (`Processing_RadarVisualizer.pde`) in the Processing IDE.
3. Adjust the COM port in the Processing sketch to match the port your Arduino is connected to (`myPort = new Serial(this, "COM10", 9600);`).
4. Run the Processing sketch.

## Usage

1. Execute the Arduino code to start measuring distances with the ultrasonic sensor.
2. Run the Processing sketch to visualize real-time radar-like graphics.
3. The graphical interface displays the angle and distance measurements as the servo motor sweeps.

## Configuration

No specific configuration is required. However, you may customize the Arduino code or Processing sketch based on your project requirements.

## Contributing

Feel free to contribute to this project! If you have any ideas, bug fixes, or improvements:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Make your changes and commit: `git commit -am 'Add new feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

