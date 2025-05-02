# Human Following Robot

This project is a simple, sensor-based human-following robot built using an Arduino Uno. It can track and follow a person using an ultrasonic sensor for distance measurement and IR sensors for directional movement. The robot adjusts its movement accordingly—moving forward, stopping, or reversing—and includes a buzzer alert when moving backward for added safety.

---

## Key Features

- Follows a human based on distance and direction
- IR sensors detect left or right movement
- Ultrasonic sensor measures proximity for motion control
- Buzzer alerts during reverse motion
- Servo rotates the ultrasonic sensor for better range detection
- Ideal for personal assistance, delivery bots, and basic automation

---

## Components Used

| Component            | Function                                           |
|---------------------|----------------------------------------------------|
| Arduino Uno          | Processes sensor input and controls motors        |
| HC-SR04 Ultrasonic Sensor | Measures distance to the target object       |
| IR Sensors           | Detects left or right movement                    |
| L293D Motor Driver   | Controls motor direction and speed                |
| DC Motors (x2)       | Drives the robot forward, backward, or turns      |
| Servo Motor          | Rotates the ultrasonic sensor for better scanning |
| Buzzer               | Alerts during reverse motion                      |

---

## Working Principle

The robot follows simple decision-making logic based on sensor inputs:

- **0–7 cm**: Robot moves **backward** and the **buzzer beeps** (too close to the target)
- **7–15 cm**: Robot **stops** and waits for further movement
- **15–25 cm**: Robot moves **forward**, following the human
- **IR Sensor Detection**:
  - Left IR signal: Robot **turns left**
  - Right IR signal: Robot **turns right**

---

## Applications

- **Personal Assistance**: Helping elderly or differently-abled individuals
- **Smart Delivery Robots**: Indoor autonomous delivery systems
- **Security Patrolling**: Automated surveillance
- **Industrial Use**: Material transport in controlled environments

---

## Future Enhancements

- Integrating **AI-based tracking** for more accurate human detection
- Using **camera vision** for facial or color-based object following
- Adding **wireless control** or **app-based monitoring**
- Expanding functionality for **outdoor navigation**

---
