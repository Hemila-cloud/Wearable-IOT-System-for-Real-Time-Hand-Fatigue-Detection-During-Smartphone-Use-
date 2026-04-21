# Wearable-IOT-System-for-Real-Time-Hand-Fatigue-Detection-During-Smartphone-Use-

## Project Overview
This project presents a wearable IoT-based system to monitor hand fatigue during prolonged smartphone usage and provide real-time adaptive feedback.

The system uses a smart glove equipped with sensors to track grip force, thumb activity, and wrist posture. A fatigue score is computed in real time, and haptic feedback (vibration alerts) is provided to encourage ergonomic corrections.



## Objectives
- Monitor hand fatigue continuously during smartphone usage  
- Detect repetitive thumb movements and sustained grip  
- Estimate fatigue using sensor-based features  
- Provide adaptive feedback to prevent discomfort  
- Promote healthy smartphone usage habits  



## System Architecture

### Sensing Layer
- FSR Sensors (Thumb & Palm) → Measure grip force and pressure  
- MPU6050 IMU → Tracks wrist posture and motion  

### Processing Layer
- ESP32 Microcontroller  
  - Sensor data acquisition  
  - Feature extraction  
  - Fatigue score computation  

### Actuation Layer
- Vibration Motor  
  - Provides haptic alerts based on fatigue level  

## Workflow
1. User wears the smart glove  
2. Sensors collect real-time data  
3. ESP32 processes and calculates fatigue score  
4. Threshold-based logic detects fatigue  
5. Vibration motor provides feedback  
6. User adjusts behavior → fatigue reduces  



## Fatigue Detection Logic

Fatigue is estimated based on:
- Grip force duration  
- Thumb repetition rate  
- Wrist posture stability  

Example:
If high grip force + repeated thumb motion + low wrist variation → Fatigue score increases  


## Feedback Mechanism

| Fatigue Level | Feedback |
|--------------|---------|
| Low | No alert |
| Medium | Short vibration (relax grip) |
| High | Repeated vibration (slow usage) |
| Critical | Long vibration (take break) |

---

## Hardware Components
- ESP32 Microcontroller  
- MPU6050 IMU Sensor  
- FSR Sensors  
- Vibration Motor  
- Connecting wires and wearable glove  



## Software & Tools
- Arduino IDE  
- Embedded C / Arduino programming  
- Serial Monitor  


## Features
- Real-time fatigue monitoring  
- Lightweight wearable design  
- Sensor fusion (IMU + FSR)  
- Edge computing (no cloud required)  
- Adaptive haptic feedback  
- Low-cost and portable  


## Limitations
- Rule-based fatigue model  
- Requires sensor calibration  
- Limited to hand/wrist monitoring  
- No mobile app integration  



## Future Enhancements
- Mobile app for visualization  
- Cloud data logging  
- Machine learning-based fatigue prediction  
- Personalized feedback system  
- Integration with smart devices  



## Applications
- Smartphone overuse monitoring  
- Ergonomic health tracking  
- Rehabilitation systems  
- Workplace fatigue monitoring  



## Conclusion
This project provides a practical solution for monitoring hand fatigue using wearable IoT technology. It combines sensor fusion and real-time feedback to promote ergonomic smartphone usage.

---

## Author
Hemila
