# Documentation for WRO Future Engineer 2023
**by Team YBR-Sunflower**

<p align="center">
  <img src="https://ybrobot.club/image/YB%20Robot%20logo.png" width="200"/>
</p>
<p align="center">
  <b>By Yothinburana School Robot Club</b>
</p>

## Our Works (YouTube Links)
[Watch our robot in action](https://youtu.be/MBe6ZsyGE-E)

## Table of Contents
- [About Our Team](#about-our-team)
- [Robot Design](#robot-design)
- [Robot Wiring Diagram](#robot-wiring-diagram)
- [Program Explanation](#program-explanation)

## About Our Team
*YBR-Sunflower* is a team of three talented students from Yothinburana School:
1. Vorawet Narkglom, 15 years old, programmer.
2. Sakolnat Raktaengan, 15 years old, robot designer.
3. Vichaiwat Koonsap, 15 years old, document designer.

## Robot Design
### The Robot

Designing a robot is a challenging endeavor. We aimed to create a small, lightweight, fast, and effective robot. A heavy robot would be slower, a large one would struggle to evade obstacles, and an ineffective one wouldn't detect walls or obstacles properly. Balance was key.

For this competition, specific rules governed robot design:
- The vehicle must be a four-wheeled vehicle with one driving axle and one steering actuator.
- Dimensions must not exceed 300x200 mm, with a height limit of 300 mm.
- Weight must not exceed 1.5 kilograms.

### Our Robot Components
- **Driving Motor**: We selected the Power Functions Large Motor made by LEGO™ for its user-friendliness, speed, and versatility.

![Driving Motor](https://ae01.alicdn.com/kf/Sc4433b091f32440e8094b8ab8c003eacI/2pcs-Enhanced-Red-L-Servo-Motor-Compatible-With-Legoeds-Power-Functions-MOC-Parts-Building-Blocks.jpg)

Specifications:
- Speed: 380 rpm
- Maximum torque: 40 Ncm
- Voltage: 9 V

- **Servo**: We opted for the GEEKSERVO-270, a 180-degree servo, for its ease of attachment and suitable degree of rotation.

![Servo](https://thepihut.com/cdn/shop/products/geekservo-building-brick-180-rotation-block-servo-geekservo-104134-28717056917699_1000x.jpg?v=1646869335)

Specifications:
- Working voltage: 3.3V~6V
- Rated voltage: 4.8V
- Rated current: 200 mA
- Stall current: 700 mA
- Sliding current: 450 mA
- Maximum torque: 500g.cm
- Angle speed: 60°/0.12s

- **Ultrasonic Sensor**: We integrated the Gravity URM 09 ultrasonic distance sensor to guide the robot's navigation by detecting distances between the robot and obstacles.

![Ultrasonic Sensor](https://robotools.in/wp-content/uploads/2022/10/DFRobot-Gravity-URM09-Analog-Ultrasonic-Sensor-5-1-1200x900.jpg)

Specifications:
- Supply Voltage: 3.3~5.5V DC
- Operating Current: 20 mA
- Operating Temperature Range: -10°C to +70°C
- Measurement Range: 2 cm to 500 cm
- Resolution: 1 cm
- Accuracy: 1%
- Frequency: 50Hz Max

- **7.4V LiPo Battery**: This 2-cell LiPo battery serves as our robot's power source, offering the right voltage for efficient operation.

![LiPo Battery](https://github.com/Snackels/WRO_Future-Engineer/assets/92850241/4b0e6cb0-ba45-4377-bb51-b34038d68638.png)

Specifications:
- 2 cells Voltage: 7.4V
- Capacity: 1100mAh 30C
- Can be charged at a current of up to 5 times the capacity (5C)
- Equipped with JST-type connectors for easy disconnection.

- **Light Sensors**: We employed both blue and red light sensors from INEX and Design By Sopon to help the robot detect lines on the race track.

![Blue Light Sensor](https://github.com/Snackels/WRO_Future-Engineer/assets/92850241/950eeb1d-ead4-4641-aa64-07414d3dd939.png)
![Red Light Sensor](https://github.com/Snackels/WRO_Future-Engineer/assets/92850241/b7f66634-942b-4f5c-b01d-777ba5d78d62.png)

These sensors not only enable the robot to see lines but also differentiate between red and blue lines, enhancing its navigation capabilities.

- **GyroCompass (GY-25)**: Equipped with the GY-25 component, our robot can discern its orientation, allowing it to make precise turns.

![GyroCompass](https://github.com/Snackels/WRO_Future-Engineer/assets/92850241/ed4a0af9-6420-498d-9d8f-a17c8bb455b0.png)

Specifications:
- Measuring range of axes: -180 to +180 degrees
- Resolution: 0.01 degrees
- Frequency Response: 100 Hz (115200bps)
- Operating Current: 15 mA
- Operating Temperature: -20 to 85°C

- **Camera (Pixy2.0)**: The Pixy2.0 camera identifies color blocks (obstacles) and transmits signals to the robot for navigation.

![Camera](https://github.com/Snackels/WRO_Future-Engineer/assets/92850241/bf7a29f9-a2cf-4b85-a056-3f12b4e75966.png)

Specifications:
- Resolution: 1296 x 976
- Processor: NXP LPC4330
- Clock Speed: 204 MHz
- RAM: 264KB
- Flash: 2 MB
- Framerate: 60 fps
- Connection: USB, UART, SPI, I²C

- **Controller (POP-32)**: Our robot is equipped with a 32-bit controller for faster reaction times, better multitasking, and more.

![Controller](https://github.com/LEST0808/LEST0808/blob/main/POP32.png)

Specifications:
- Microcontroller: 32-bit STM32F103CBT6 with 128KB flash memory
- Clock Signal: 20 MHz
- JST 3-Pin Ports: 11 points for connecting sensors and devices
- LED Indicators: Power status, low battery alert, USB port connection
- RESET Switch: RESET switch
- USB Port: For program downloading and data communication
- Power Input: 6V to 9V with power switch
- Digital and Analog Ports: 9 digital/analog input/output ports (A0 to A8)
- I2C Ports: 2 sets of I2C ports (SDA and SCL)
- UART Port: UART communication via PB7 (RxD) and PB6 (TxD)
- Motor Driver Circuit: 4-channel motor driver with overcurrent protection
- Servo Motor Ports: 6 servo motor ports
- Speaker: Piezo speaker for generating sound
- OLED Display: 1.5-inch OLED display with a resolution of 128 x 64 pixels
- Push Buttons and Knob: Push buttons (OK, SW-A, SW-B) and an adjustable knob (KNOB) for input and testing

### Robot Wiring Diagram
To understand how our robot is wired, please refer to our [robot wiring diagram](#).

## Program Explanation
To use the program for our robot, you will need the following programs and libraries:

### Programs:
- [Arduino IDE 2.1.1](https://www.arduino.cc/en/software): For programming your Arduino UNO.
- [Pixymon V2](https://pixycam.com/downloads-pixy2/): For displaying and configuring your Pixy.

### Required Libraries:
- `Mapf.h`
- `Servo.h`
- `PID_v2.h`
- `Pixy2I2C.h`

You can install these libraries using the library manager in the Arduino IDE. However, for the Pixy library, you will need to download it from [this website](https://pixycam.com/downloads-pixy2/) as it is required to communicate with the servo, sensor, and other functions.

Our program consists of several main components, each with its own purpose:

- **Main_program_no_obstacles:** [Link](https://github.com/Snackels/WRO_Future-Engineer/blob/main/scr/no%20obstacle/Main_no_obj.ino)
  - This program utilizes the ultrasonic sensor to calculate the distance between the robot and walls, ensuring it maintains an optimal distance.

- **Function_no_obstacles:** [Link](https://github.com/Snackels/WRO_Future-Engineer/blob/main/scr/no%20obstacle/function.ino)
  - The robot uses the gyro sensor to determine the steering degree and employs a PID controller to maintain a consistent distance from the wall.

- **Main_program_obstacles:** [Link](https://github.com/Snackels/WRO_Future-Engineer/blob/main/scr/obstacle/Main_obj.ino)
  - In this program, we use the camera, gyro, and ultrasonic sensors to calculate the steering degree for navigation.

- **Function_obstacles:** [Link](https://github.com/Snackels/WRO_Future-Engineer/blob/main/scr/obstacle/function.ino)
  - Similar to the previous program, the robot employs PID control but also considers obstacle avoidance in its navigation.

Thank you for exploring our documentation. We hope you find it useful, and we wish all the participants of WRO Future Engineer 2023 the best of luck!
