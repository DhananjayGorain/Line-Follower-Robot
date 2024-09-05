<h1>Problem Statement</h1>
<br>
The Line Follower Robot is an autonomous robot designed to follow a pre-defined path (usually a black line on a white surface or vice versa). The robot uses sensors to detect the line and adjust its movement accordingly. The primary challenge is to control the robot's motors based on sensor feedback so that it stays on the path without deviating.

In this project, two infrared (IR) sensors are used to detect the line. Based on the sensor inputs, the robot takes the necessary actions to either move forward, take a left turn, or take a right turn. The aim of the project is to implement efficient motor control using the 8051 microcontroller to allow the robot to follow the line smoothly.

<h1>Solution</h1>
<br>
The solution involves using an 8051 microcontroller to control two DC motors based on sensor feedback. The robot is equipped with two IR sensors that provide input to the microcontroller. The sensors check the presence of the line and send the input to the microcontroller, which then decides the motor action. If both sensors detect the line, the robot moves forward. If only one sensor detects the line, the robot takes a corresponding turn to adjust its position.

The code implements the following functions:

1.move_forward(): Both motors move the robot forward.<br>
2.take_left_turn(): The right motor is active, while the left motor stops, causing the robot to turn left.<br>
3.take_right_turn(): The left motor is active, while the right motor stops, causing the robot to turn right.<br>
The continuous loop ensures the robot constantly checks the sensors' status and adjusts its movement in real-time, allowing it to effectively follow the line on the surface.
