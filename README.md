IR Based Object Detection Alarm
A simple, low-cost, hardware-based object detection alarm using an FC-51 infrared (IR) sensor module. When an object is detected within the sensor's range, the system provides an audible alert through an active buzzer and visual indication using two blue LEDs.
Project Overview
This project demonstrates basic IR-based proximity detection and alarm indication. The circuit is assembled on a copper board and powered by a 9V battery, making it portable and suitable for a beginner-level electronics project.

Important: This README reflects the actual project components confirmed by the project team. An NPN transistor / BC547 is not included in the actual component list.
Components Used
- FC-51 IR sensor module
- Active buzzer
- 2 blue LEDs
- Copper board (general-purpose PCB)
- 9V battery
- 9V battery snap connector
- Connecting wires
Working Principle
1. The FC-51 sensor emits infrared light.
2. When an object enters the detection area, some IR light reflects back to the sensor.
3. The sensor module detects the reflected IR and changes its output state.
4. The circuit activates the active buzzer and blue LED indicators to alert the user.
Block Diagram
Object
  ↓ reflected IR
FC-51 IR Sensor Module
  ↓ output
Alarm / Indicator Circuit
  ├── Active Buzzer
  └── 2 Blue LEDs
Assembly
The components are assembled on a copper board. The IR sensor module is connected to the board using wires, and the circuit is powered by a 9V battery through its snap connector.

Before powering the circuit, check the polarity of the battery and LEDs, confirm the sensor's VCC/GND/OUT connections, and inspect solder joints for shorts.
Reported Results
The project report describes the following observed performance:
- Approximate detection range for a hand: 2–25 cm
- Approximate response time: 55 ms
- Audible and visual alarm on detection
- Portable 9V battery operation
Actual detection distance may vary with object surface, sensor adjustment, and ambient light. The report notes reduced detection range for dark or transparent surfaces and possible interference in direct sunlight.
Features
- Low-cost and simple circuit
- Non-contact object detection
- Audible and visual indication
- Portable battery-powered operation
- No microcontroller or programming required for the basic implementation
Applications
- Short-range object or obstacle detection
- Entry or approach alert
- Educational electronics demonstrations
- Basic proximity alarm experiments
Limitations
- Short detection range
- Performance depends on surface reflectivity and sensor adjustment
- Direct sunlight may cause false triggering
- Provides a local alarm only; no wireless or remote notification
Future Improvements
- Add an enclosure for protection
- Improve mounting and sensor positioning
- Explore a more reliable sensor for longer-range detection
- Add wireless notification in a future version
Skills Demonstrated
- Basic sensor interfacing
- Electronic circuit assembly
- Copper-board soldering
- Hardware testing and troubleshooting
Team
- V. Asritha
- V. Navya Deepthi
- Y. Rajesh
- V. Uday Shankar
Project Details
- Project: IR Based Object Detection Alarm
- Department: Electronics and Communication Engineering
- Institution: Aditya University
- Academic year: 2025–2026
