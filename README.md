# IR-Based Object Detection Alarm

A low-cost, portable object detection alarm built using an FC-51 infrared (IR) sensor module. When an object enters the sensor's detection zone, the circuit activates an audible buzzer and two blue LEDs.

## Project Overview

This project demonstrates a simple hardware-based proximity alarm using infrared reflection. It is assembled on a general-purpose copper board and powered by a 9V battery, so it can operate without a microcontroller or mains power.

**Project type:** B.Tech ECE Cornerstone Project  
**Academic year:** 2025–2026  
**Institution:** Aditya University  
**Department:** Electronics and Communication Engineering

## Team

| Name | Roll Number |
|---|---|
| V. Asritha | 25B11EC802 |
| V. Navya Deepthi | 25B11EC823 |
| Y. Rajesh | 25B11EC837 |
| V. Uday Shankar | 25B11EC853 |

**Project guides:** M. Suneel and P. Sailaja

## Objectives

- Detect nearby objects using an IR sensor module.
- Activate an audible alarm and visual indication when an object is detected.
- Build a compact, low-cost and portable circuit.
- Understand IR reflection, sensor comparator output and transistor switching.
- Assemble and test a practical circuit on a copper board.

## Components Used

| Component | Specification / Quantity | Purpose |
|---|---|---|
| IR sensor module | FC-51, 1 | Detects objects through reflected IR |
| Active buzzer | 1 | Audible alarm |
| Blue LEDs | 2 | Visual alarm indication |
| NPN transistor | BC547, 1 | Switching the alarm outputs |
| Copper board | 1 | Circuit assembly base |
| Battery | 9V, 1 | Portable power supply |
| Battery connector | 9V snap, 1 | Battery connection |
| Connecting wires | As required | Electrical connections |

The implementation described in the project report does not use an Arduino or other microcontroller.

## Working Principle

1. The FC-51 module emits infrared light from its IR transmitter.
2. When an object is in front of the sensor, some IR light reflects back to the receiver.
3. The module's LM393 comparator compares the received signal with a threshold set using its potentiometer.
4. On object detection, the sensor's digital output changes to its active-LOW state.
5. The circuit's transistor switching stage activates the buzzer and both blue LEDs.
6. When the object leaves the detection zone, the alarm output returns to its inactive state.

The sensor sensitivity can be adjusted using the onboard potentiometer.

## System Block Diagram

```text
        Object
          |
          v
     FC-51 IR Sensor
          |
          v
   Comparator / Output
          |
          v
   Transistor Switch
       /       \
      v         v
   Buzzer    Blue LEDs
  (Sound)    (Visual)
```

## Circuit and Assembly

The circuit is assembled on a general-purpose copper board. The IR sensor module is connected using short wire leads, allowing it to be repositioned or replaced. The 9V battery connects through a snap connector.

The project report describes the following connections:

- Battery positive and negative connect to the circuit's supply and ground rails.
- The IR sensor's VCC and GND connect to the corresponding supply rails.
- The sensor output is connected to the BC547 transistor switching stage.
- The buzzer and two LEDs provide the alarm outputs.

> **Note:** Check the actual circuit diagram and component pinouts before reproducing the circuit. In particular, verify the sensor module's output behavior, transistor pin configuration, LED polarity and suitable current-limiting arrangements for your own build.

## Reported Results

The project report records the following test results:

| Parameter | Reported result |
|---|---|
| Detection range for a hand | Approximately 2–25 cm |
| Response time | Approximately 55 ms |
| Supply | 9V battery |
| Fresh battery voltage during testing | 8.9V |
| Idle current | Approximately 22 mA |
| Alarm current | Approximately 68 mA |
| Buzzer | Activates on detection |
| LED indication | Both blue LEDs turn on |
| Sunlight interference | Occasional false triggering observed |

Detection range depends on the object's surface. The report recorded longer detection distances for white paper and a human hand, and shorter distances for dark or transparent materials.

## Advantages

- Low-cost and simple construction.
- Portable battery-powered operation.
- No microcontroller or programming required.
- Audible and visual alarm outputs.
- Adjustable sensor sensitivity.
- Fast response for short-range detection.

## Limitations

- Short detection range; intended for proximity applications.
- Direct sunlight or strong IR sources may cause false triggering.
- Dark or IR-absorbing surfaces reduce detection reliability.
- A single sensor provides only one detection zone.
- No event logging or remote notification in the current version.

## Applications

- Basic home or cabinet security alert.
- Entry and proximity detection.
- Obstacle detection in educational robotics.
- Object passage indication on small conveyor demonstrations.
- Parking-slot or occupancy indication at short range.

## Future Scope

Possible improvements include:

- Add an ESP32 or ESP8266 for remote notifications.
- Add a microcontroller for event counting and logging.
- Use additional sensors for wider coverage.
- Use a longer-range sensor for larger detection zones.
- Design a protective enclosure and improved PCB.
- Add a display for system status.

## Learning Outcomes

Through this project, the team practised:

- IR reflection-based sensing.
- Understanding an IR sensor module and comparator output.
- Transistor switching for driving output devices.
- Circuit assembly and soldering on a copper board.
- Sensor interfacing and sensitivity adjustment.
- Testing, troubleshooting and documenting hardware performance.

## Project Files

Upload the following project materials to this repository as available:

- `README.md` — project overview and documentation
- `poster.pdf` — project poster
- `irfinal report.pdf` — detailed project report
- `IR Based object detection alarm demo video.mp4` — project demonstration video

## References

The project report lists these references:

- R. L. Boylestad and L. Nashelsky, *Electronic Devices and Circuit Theory*, 11th Edition, Pearson, 2013.
- D. Patranabis, *Sensors and Transducers*, 2nd Edition, PHI Learning, 2003.
- T. L. Floyd, *Digital Fundamentals*, 10th Edition, Pearson, 2009.
- FC-51 IR sensor module resources: [Components101](https://www.components101.com)
- [Arduino](https://www.arduino.cc)
- [Electronics For You](https://www.electronicsforu.com)
- [Electronics Hub](https://www.electronicshub.org)
- [SparkFun Electronics](https://www.sparkfun.com)

---

*This README summarizes the submitted project report and poster. Performance values are the results reported in those project materials.*
