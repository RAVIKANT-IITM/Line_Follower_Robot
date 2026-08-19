# 🤖 Line Follower Robot

A PID-controlled line follower robot built using **Arduino Nano, TB6612FNG motor driver, N20 motors, and an 8-channel QTR sensor array**.

## 🚀 Project Overview

This robot is designed to follow a predefined line using real-time feedback from an 8-channel QTR sensor array. A **PID control algorithm** continuously calculates the position error and adjusts the speed of the left and right motors accordingly.

This results in smoother movement, better stability, and improved handling of turns, even at higher speeds.

## 🔧 Hardware Used

* Arduino Nano
* TB6612FNG Motor Driver
* N20 Geared Motors
* QTR-8RC / QTR 8-channel Sensor Array
* Robot Chassis
* Battery
* Connecting Wires

## ⚙️ Working Principle

1. The QTR sensor array detects the line.
2. Sensor readings are processed to calculate the line position.
3. The position is compared with the desired center position.
4. The PID controller calculates the required correction.
5. Motor speeds are adjusted based on the correction.
6. The robot continuously repeats this process in real time.

### PID Control

The controller uses three parameters:

```text
Correction = Kp × Error + Ki × Integral + Kd × Derivative
```

Current PID parameters:

```cpp
Kp = 0.13;
Ki = 0.0;
Kd = 0.5;
```

These values can be tuned according to the track, motor speed, sensor setup, and robot weight.

## 📊 Features

* Real-time sensor processing
* PID-based control
* Adjustable motor speed
* Adjustable PID parameters
* Serial monitoring of sensor values
* Smooth line tracking
* Better stability during turns

## 💻 Software

* Arduino IDE
* Embedded C/C++
* PID Control Algorithm

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

* Embedded systems
* Robotics
* Real-time data processing
* Sensor interfacing
* Motor control
* PID control and tuning
* Hardware-software integration

I also had the opportunity to **present this project at IIT Madras Spark**, where I demonstrated the robot and discussed its design and working.

## 🔮 Future Improvements

* Automatic PID tuning
* Higher-speed optimization
* Better line-loss recovery
* Sensor calibration
* Advanced control algorithms
* Improved mechanical design

