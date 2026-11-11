# AUTONOMOUS OBSTACLE AVOIDING ROBOT
### Project Report

**Department:** Robotics and Automation Engineering  
**Project Type:** Embedded Systems and Mobile Robotics  
**Author:** Hitesh Kadam  
**Institution:** Zeal College of Engineering, Pune  
**Repository:** Autonomous Obstacle Avoiding Robot  
**Project Status:** [In Progress / Completed]

---

# 1. Abstract

The Autonomous Obstacle Avoiding Robot is a mobile robotic system designed to detect obstacles in its surroundings and navigate without continuous human intervention.

The system uses an Arduino Uno as its main controller, an ultrasonic sensor to measure the distance between the robot and nearby objects, and a servo motor to scan different directions.

Based on the distance measurements, the Arduino processes the sensor data and sends appropriate control signals to the L298N motor driver, which controls the movement and direction of the DC motors.

The primary objective of this project is to understand the practical implementation of robotics, embedded programming, sensor integration and autonomous navigation.

---

# 2. Introduction

Robotics and automation play an important role in modern industries, transportation, healthcare and various other fields.

An autonomous robot is capable of performing tasks with minimal human intervention by using sensors, controllers and actuators.

This project focuses on developing a two-wheel autonomous obstacle avoiding robot that can identify obstacles in its path and change its direction to avoid collisions.

The robot combines hardware components and embedded programming to demonstrate the basic principles of autonomous mobile robotics.

## 2.1 Project Overview

<img width="391" height="290" alt="image" src="https://github.com/user-attachments/assets/453ce046-5a93-47d9-b75c-433e945b92a5" />


*Figure 1: Complete view of the Autonomous Obstacle Avoiding Robot.*

---

# 3. Objectives

The main objectives of this project are:

1. To design and develop an autonomous mobile robot.
2. To detect obstacles using an ultrasonic sensor.
3. To measure the distance between the robot and nearby objects.
4. To implement automatic decision-making using Arduino.
5. To control DC motors using an L298N motor driver.
6. To use a servo motor for scanning different directions.
7. To understand the integration of sensors, actuators and microcontrollers.
8. To demonstrate a practical application of robotics and automation.

---

# 4. Hardware Components

The following hardware components are used in the development of this project.

## 4.1 Arduino Uno

The Arduino Uno acts as the main processing unit of the robot. It receives distance measurements from the ultrasonic sensor, processes the information and controls the motors through the motor driver.

![Arduino Uno](../Components/Arduino_Uno.jpg)

*Figure 2: Arduino Uno Microcontroller.*

## 4.2 Ultrasonic Sensor (HC-SR04)

The HC-SR04 ultrasonic sensor detects obstacles by transmitting ultrasonic waves and measuring the time taken for the reflected waves to return.

It provides distance information to the Arduino for obstacle detection.

![Ultrasonic Sensor](../Components/Ultrasonic_Sensor.jpg)

*Figure 3: HC-SR04 Ultrasonic Sensor.*

## 4.3 Servo Motor

The servo motor rotates the ultrasonic sensor to different angles, allowing the robot to scan its surroundings and identify a suitable direction for movement.

![Servo Motor](../Components/Servo_Motor.jpg)

*Figure 4: Servo Motor.*

## 4.4 L298N Motor Driver Module

The L298N motor driver controls the direction and speed of the DC motors based on signals received from the Arduino Uno.

![L298N Motor Driver](../Components/L298N_Motor_Driver.jpg)

*Figure 5: L298N Motor Driver Module.*

## 4.5 DC Motors

DC geared motors provide mechanical movement to the robot by converting electrical energy into rotational motion.

![DC Motors](../Components/DC_Motors.jpg)

*Figure 6: DC Geared Motors.*

## 4.6 Battery Pack

The battery pack supplies electrical energy to the robot's electronic and motor systems.

![Battery Pack](../Components/Battery_Pack.jpg)

*Figure 7: Battery Pack.*

## 4.7 Switch

The switch is used to control the power supply and turn the robot ON or OFF.

![Switch](../Components/Switch.jpg)

*Figure 8: Power Switch.*

---

# 5. Software Requirements

## 5.1 Arduino IDE

Arduino IDE is used to write, compile and upload the program to the Arduino Uno.

**Main functions:**
- Writing and editing embedded C/C++ code.
- Compiling the program.
- Uploading code to the microcontroller.
- Debugging through Serial Monitor.

Official Website: https://www.arduino.cc/en/software

---

# 6. System Architecture

The robot consists of three major sections:

1. **Input Section:** Ultrasonic sensor detects obstacles and measures distance.
2. **Processing Section:** Arduino Uno processes the sensor readings and makes movement decisions.
3. **Output Section:** Servo motor and DC motors perform the required movements.



# 7. Circuit Diagram

The circuit connects the Arduino Uno, ultrasonic sensor, servo motor, L298N motor driver, DC motors and battery supply.

The Arduino acts as the central controller and coordinates the operation of the connected components.



![Circuit Diagram](../Circuit_Diagram/circuit_diagram.png)

*Figure 10: Circuit Diagram of the Autonomous Obstacle Avoiding Robot.*

**Note:** Actual pin connections, power ratings and wiring should be documented according to the implemented circuit.

---

# 8. Working Principle

The robot operates using an ultrasonic distance measurement technique and automatic motor control.

The general working sequence is as follows:

1. The robot starts when the power supply is switched ON.
2. The Arduino initializes the ultrasonic sensor, servo motor and motor driver.
3. The ultrasonic sensor measures the distance between the robot and the obstacle.
4. If the path is clear, the robot continues moving forward.
5. If an obstacle is detected within the defined threshold distance, the robot stops.
6. The servo motor rotates the ultrasonic sensor to scan the left and right directions.
7. The Arduino compares the available distances.
8. The motor driver receives control signals to move the robot in the selected direction.
9. The process repeats continuously.



![Obstacle Detection](../Images/obstacle_detection.jpg)

*Figure 11: Obstacle Detection Demonstration.*

---

# 9. Algorithm

**Step 1:** Start the robot.

**Step 2:** Initialize all input and output pins.

**Step 3:** Measure the distance using the ultrasonic sensor.

**Step 4:** Check whether an obstacle is present within the predefined threshold.

**Step 5:**
- If no obstacle is detected, move forward.
- If an obstacle is detected, stop the robot.

**Step 6:** Rotate the servo motor to scan the surroundings.

**Step 7:** Measure the distances in different directions.

**Step 8:** Compare the measured distances and select a suitable direction.

**Step 9:** Control the DC motors through the L298N motor driver.

**Step 10:** Repeat the process continuously.

---

# 10. Flowchart



![Flowchart](../Images/flowchart.png)

*Figure 12: Algorithm Flowchart.*

---

# 11. Source Code

The complete Arduino source code is available in the Code directory of this repository.

**Source Code:** [View Arduino Program](../Code/obstacle_avoiding_bot.ino)

The program handles:
- Ultrasonic distance measurement.
- Servo motor positioning.
- Obstacle detection.
- Motor direction control.
- Automatic navigation decisions.

---

# 12. Project Implementation

The hardware components are assembled on the robot chassis and interconnected according to the circuit design.

The Arduino Uno is programmed with the obstacle avoidance algorithm. After completing the connections and uploading the program, the robot is tested under different obstacle conditions.



![Robot Assembly](../Images/robot_assembly.jpg)

*Figure 13: Hardware Assembly.*



![Robot Working](../Images/robot_working.jpg)

*Figure 14: Robot During Testing.*

---

# 13. Testing and Observations

The robot should be tested under different environmental and obstacle conditions.

| Test No. | Test Condition | Expected Behaviour | Actual Observation |
|---|---|---|---|
| 1 | Clear path | Move forward | [Update] |
| 2 | Obstacle in front | Stop and scan | [Update] |
| 3 | Obstacle on left | Select a suitable direction | [Update] |
| 4 | Obstacle on right | Select a suitable direction | [Update] |
| 5 | Obstacles in multiple directions | Select the available clear path | [Update] |



![Testing Results](../Images/testing_results.jpg)

*Figure 15: Experimental Testing.*

---

# 14. Applications

The basic obstacle avoidance mechanism demonstrated in this project can be applied in:

- Autonomous mobile robots.
- Educational robotics.
- Automated material transportation.
- Warehouse automation.
- Robotic navigation systems.
- Basic collision avoidance systems.

---

# 15. Limitations

Some limitations of the current system may include:

1. Ultrasonic sensors can produce inaccurate readings under certain environmental conditions.
2. The robot may not identify very small or irregularly shaped obstacles reliably.
3. The navigation strategy is limited to the sensor's detection range and scanning directions.
4. Uneven surfaces may affect motor movement.
5. Battery capacity limits the operating duration.

---

# 16. Future Scope

The project can be improved through the following developments:

- Integration of multiple ultrasonic sensors.
- Implementation of more advanced navigation algorithms.
- Addition of wheel encoders for movement feedback.
- Integration of Bluetooth or wireless monitoring.
- Battery level monitoring.
- Implementation of SLAM for mapping and navigation.
- Improved obstacle detection and decision-making.

---

# 17. Conclusion

The Autonomous Obstacle Avoiding Robot demonstrates the fundamental principles of autonomous mobile robotics through the integration of sensors, actuators, motor control and embedded programming.

The project provides practical experience in Arduino programming, ultrasonic distance measurement, servo motor control and DC motor interfacing.

It also establishes a foundation for developing more advanced autonomous robotic systems with intelligent navigation and obstacle detection capabilities.

---

# 18. References

1. Arduino Official Documentation: https://docs.arduino.cc/
2. HC-SR04 Ultrasonic Sensor Datasheet.
3. L298N Motor Driver Datasheet.
4. Arduino IDE Official Website: https://www.arduino.cc/en/software

---

**Project Author:** Hitesh Kadam  
**Department:** Robotics and Automation Engineering  
**Institution:** Zeal College of Engineering, Pune

*This report documents the design, development and testing of the Autonomous Obstacle Avoiding Robot.*
