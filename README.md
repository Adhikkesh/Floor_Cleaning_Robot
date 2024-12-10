# Smart Floor Cleaning robot with Obstacle Evasion

## Project Overview

This is an Arduino-based autonomous vacuum cleaning robot capable of navigating and cleaning indoor spaces using ultrasonic sensing and adaptive movement strategies.

## Features

- **Autonomous Navigation**: Uses ultrasonic sensor for obstacle detection and avoidance
- **Adaptive Movement**: Dynamically adjusts route when encountering obstacles
- **360-Degree Scanning**: Servo-mounted ultrasonic sensor for comprehensive room scanning
- **Gradual Speed Control**: Smooth acceleration and deceleration of motors

## Hardware Components

- Arduino UNO
- Adafruit Motor Shield
- NewPing Ultrasonic Sensor
- Servo Motor
- 4 DC Motors
- Chassis and Wheels

## Pin Configuration

- Ultrasonic Sensor:
  - Trigger Pin: A1
  - Echo Pin: A0
- Servo Motor Pin: 10
- Motor Shield: Utilizing motors 1-4

## Robot Behavior

The robot operates with the following core behaviors:
1. Move forward continuously
2. Detect obstacles within 15 cm
3. Stop and scan surroundings when obstacle detected
4. Choose optimal direction (right or left) to avoid obstacle
5. Resume forward movement in chosen direction

## Key Functions

- `lookDirection()`: Rotates servo to scan specific angles
- `readPing()`: Measure distance using ultrasonic sensor
- `moveForward()`, `moveBackward()`: Controlled motor movement
- `turnLeft()`, `turnRight()`: Navigation maneuvers

## Installation and Setup

### Prerequisites
- Arduino IDE
- Libraries:
  - AFMotor
  - NewPing
  - Servo

### Steps
1. Install required libraries
2. Connect hardware components
3. Upload code to Arduino UNO
4. Power on and deploy robot

## Customization

Easily modify parameters like:
- `MAX_SPEED`: Adjust overall robot speed
- `MAX_DISTANCE`: Change obstacle detection range
- Servo angle configurations

## Limitations

- Designed for indoor, flat surfaces
- Requires open spaces for effective navigation
- Battery life dependent on motor and battery specifications

## Future Improvements

- Add battery level monitoring
- Implement more sophisticated navigation algorithms
- Integrate cleaning mechanism
- Add remote control capabilities

## Troubleshooting

- Check all connections
- Ensure libraries are correctly installed
- Verify motor and sensor alignments
- Monitor serial output for diagnostic information

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests with improvements or bug fixes.


## Acknowledgments

- Adafruit for Motor Shield library
- NewPing library contributors
- Arduino community
