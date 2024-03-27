# Smart Door Lock

## Introduction

In response to the moderate to high concern about home break-ins, our team developed a smart door-locking system designed to enhance security and provide convenience to homeowners. Our system is engineered to permit access only to authorized individuals and to maintain a log of any unauthorized attempts to enter, significantly improving upon conventional lock and key systems.

## Getting Started

### Prerequisites

- Raspberry Pi (Tested on Raspberry Pi 3 Model B)
- Ultrasonic Sensor (HC-SR04)
- Pi Camera
- Temperature and Humidity Sensor (DHT22)
- Various electronic components (LEDs, resistors, wires, etc.)
- Software requirements include Python 3.x with libraries: RPi.GPIO, pandas, Adafruit_DHT, sklearn, pickle

### Installation

1. Set up your Raspberry Pi with the latest version of Raspbian.
2. Connect the hardware components according to the schematics provided in the diagrams section.
3. Install the required Python libraries using pip:

```bash
pip install RPi.GPIO pandas Adafruit_DHT sklearn pickle
```

4. Clone this repository to your Raspberry Pi:

```bash
git clone https://github.com/DRSNAJ/SmartDoorLock.git
```

5. Navigate to the project directory and run the setup script:

```bash
cd SmartDoorLock
python setup.py install
```

## Usage

To start the Smart Door Lock system, execute the main script:

```bash
python main.py
```

The system initializes and waits for interaction at the door. Authorized users can enter their credentials through the GUI, and the door will unlock if the credentials are validated. Unauthorized access attempts trigger an alert to the homeowner.

## Features

- **User Authentication**: Secure login and password GUI for premises access.
- **Intruder Alert**: Detects presence and records video of unknown individuals, alerting the homeowner.
- **Gesture Control**: Allows unlocking/locking doors via hand gestures.
- **Environmental Awareness**: Provides real-time weather information.
- **Enhanced Security**: Incorporates web security features to protect against data breaches.

## Credits

Special thanks to our team members:

- Don Randike Jayathilake: Project coordination, coding of core functionalities.
- Mohammed Sadequl Alam: Contribution to user authentication and GUI development.
- Nafiz Uddin Nayan: Developed the gesture recognition and environmental awareness features.
- Abhinav Jayaprakash: Implemented security features, including encryption and decryption algorithms.

## Acknowledgments

- Inspired by the need for improved home security solutions.
- Thanks to the open-source community for providing the necessary tools and libraries.
