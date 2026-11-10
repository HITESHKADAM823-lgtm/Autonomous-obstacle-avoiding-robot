Hardware Components & Software Requirements

This section provides an overview of the hardware components and software used in the development of the Autonomous Obstacle Avoiding Robot.

1. Arduino Uno

Description:
Arduino Uno is the main microcontroller board responsible for processing sensor data and controlling the robot's movements.

Function:

- Processes data received from the ultrasonic sensor.
- Controls the servo motor and motor driver.
- Executes the obstacle avoidance algorithm.



---

2. Ultrasonic Sensor (HC-SR04)

Description:
The HC-SR04 ultrasonic sensor is used to detect obstacles by measuring the distance between the robot and nearby objects using ultrasonic waves.

Function:

- Measures the distance to nearby objects.
- Detects obstacles in the robot's path.
- Provides distance data to the Arduino Uno.



---

3. Servo Motor

Description:
A servo motor is used to rotate the ultrasonic sensor to different angles, allowing the robot to scan its surroundings.

Function:

- Rotates the ultrasonic sensor.
- Scans the left, right and front directions.
- Helps determine a suitable direction for movement.



---

4. Motor Driver Module (L298N)

Description:
The L298N motor driver is an electronic module used to control the speed and direction of the DC motors.

Function:

- Controls the forward and reverse movement of motors.
- Enables left and right turning.
- Receives control signals from the Arduino Uno.



---

5. DC Motors

Description:
DC geared motors are used to provide mechanical movement to the robot. They convert electrical energy into rotational mechanical energy.

Function:

- Drive the robot's wheels.
- Enable forward and backward movement.
- Allow turning through independent motor control.


---

6. Battery Pack

Description:
The battery pack provides the electrical power required to operate the robot and its electronic components.

Function:

- Supplies power to the robot.
- Provides the required voltage and current.
- Enables autonomous operation without a wired power supply.


---

7. Switch

Description:
An electrical switch is used to control the power supply to the robot.

Function:

- Turns the robot ON and OFF.
- Controls the electrical connection between the power source and circuit.



---

8. Arduino IDE

Description:
Arduino IDE (Integrated Development Environment) is the software platform used to write, edit, compile and upload the program to the Arduino Uno.

Function:

- Writing and editing Arduino code.
- Compiling and checking the program for errors.
- Uploading the program to the microcontroller.
- Monitoring serial communication for debugging.

Software: "Arduino IDE Official Website" (https://www.arduino.cc/en/software)

---

Component Summary

Sr. No.| Component| Category
1| Arduino Uno| Microcontroller
2| HC-SR04 Ultrasonic Sensor| Sensor
3| Servo Motor| Actuator
4| L298N Motor Driver| Motor Controller
5| DC Motors| Actuators
6| Battery Pack| Power Supply
7| Switch| Electrical Component
8| Arduino IDE| Software

---

Project: Autonomous Obstacle Avoiding Robot
Author: Hitesh Kadam
Branch: Robotics and Automation Engineering
