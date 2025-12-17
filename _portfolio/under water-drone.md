---
title: "5-DOF Underwater Drone"
collection: portfolio
header:
  image: /images/500x300.png
  teaser: /images/500x300.png
---

<img src="{{ site.baseurl }}/images/rov.jpg">
<br>End-to-end design and testing of a 5-DOF underwater ROV based on the CPS5 desgin

5-DOF Underwater ROV (CPS5-Based)<br>

Underwater Robotics • Mechatronics • Systems Integration<br><br>

Built a 5-DOF underwater ROV based on the CPS5 design, taking ownership of the full engineering workflow. Adapted the mechanical structure in SolidWorks, integrated the electronics stack (Pixhawk, Raspberry Pi, ESCs, motors, sensors), and designed custom wiring and waterproof housings.<br><br>
<img src="{{ site.baseurl }}/images/rov-electronics pipe.jpg" width="300"><br>
Performed bench testing of power distribution, motor control, communication, and sensors before moving to pool testing. Diagnosed and resolved issues including leaks, unstable buoyancy, electrical noise, and motor calibration through iterative design improvements such as sealing upgrades, wiring reorganization, ferrite filtering, and control parameter tuning.<br><br>

# Advanced 5-Degree-of-Freedom Remotely Operated Vehicle (ROV) with AI-Powered Hazard Detection<br>
<br>
Advanced 5-degree-of-freedom Remotely Operated Vehicle (ROV) with AI-powered hazard detection, designed for underwater exploration and marine research up to 85m depth.<br>
<br>
Robotics • Mechatronics • Computer Vision • Embedded Systems • AI • Underwater Engineering<br>
<br>
## Overview<br>
Developed a sophisticated underwater drone (ROV) capable of precise 5-DOF navigation and real-time object detection. The project, titled CPS5, was engineered at Al-Balqa' Applied University to address challenges in traditional ROVs such as limited maneuverability and communication delays.<br>
<br>
The system features a unique semi-flooded design where only critical electronics are sealed in a pressure-resistant housing, improving stability and reducing buoyancy issues.<br>
<br>
## Project Objectives<br>
- Achieve stable movement with 5 brushless DC motors.<br>
- Integrate a dual-controller architecture (Raspberry Pi 4 & Pixhawk).<br>
- Implement real-time AI vision for underwater threat detection (Lionfish).<br>
- Ensure structural integrity at depths up to 85 meters.<br>
<br>
## System Design<br>
<br>
### Mechanical System<br>
- Modular frame combining CNC-machined and 3D-printed PLA components.<br>
- Cylindrical pressure vessel made of 5mm thick Acrylic (PMMA).<br>
- Calculated Safety Factor: ~11.7 at target depth.<br>
- Waterproofing via dual O-ring grooves and epoxy-sealed cable feedthroughs.<br>
- Hydrodynamic optimization resulting in a maximum velocity of 1.5 m/s.<br>
<br>
### Propulsion & Maneuverability<br>
- 5-Degree-of-Freedom thrust vectoring.<br>
- Horizontal Thrusters (x2): Sunnysky 980 KV motors for longitudinal motion and yaw.<br>
- Vertical Thrusters (x3): A2212 930 KV motors in a triangular configuration for heave, pitch, and roll.<br>
- Custom 3D-printed propellers (60mm horizontal, 50mm vertical) optimized for torque in dense water.<br>
<br>
### Electrical & Power Architecture<br>
<br>
#### Dual-Controller System<br>
- Raspberry Pi 4: Handles high-level tasks, BlueOS, and AI vision processing.<br>
- Pixhawk (ArduSub): Manages low-level flight control, sensor fusion (IMU/Barometer), and PWM motor signals.<br>
<br>
#### Power System<br>
- 3S2P Li-ion battery pack with Integrated BMS.<br>
- Power Distribution: 12V for thrusters/lights, regulated 5V for logic.<br>
- Safety: 60A main fuse and MOSFET-based battery switching circuit.<br>
<br>
## AI and Vision System<br>
- Detection Model: YOLOv8n (nano) trained specifically to identify invasive Lionfish in the Red Sea.<br>
- Edge AI: Real-time inference performed locally on the Raspberry Pi 4 to minimize latency.<br>
- Visual Enhancement: High-intensity LEDs integrated for low-light deep-sea visibility.<br>
- Communication: Tethered Ethernet connection for low-latency H.264 video streaming and telemetry to QGroundControl.<br>
<br>
## Control & Ground Station<br>
- Software Stack: BlueOS (onboard) paired with QGroundControl (surface).<br>
- Input: PS4 Controller mapped for intuitive manual navigation.<br>
- Sensors: MS5837 depth sensor, MPU6000 IMU, and magnetometer for stabilized "Depth Hold" and "Stabilize" modes.<br>
<br>
## Results & Specifications<br>
- Max Depth: 85 meters.<br>
- Max Speed: 1.5 – 2.0 m/s.<br>
- Endurance: Approximately 14.1 minutes at adjusted peak power.<br>
- Functionality: Successfully demonstrated real-time hazard detection and stable 5-DOF underwater maneuvering.<br>
<br>
## Technologies Used<br>
- Raspberry Pi 4 & Pixhawk 2.4.8<br>
- YOLOv8 & PyTorch<br>
- BlueOS & ArduSub<br>
- QGroundControl<br>
- SolidWorks (Hydrodynamic Simulation)<br>
- BLHeli (ESC Programming)<br>
<br>
## Project Team<br>
- Students: Hossam Aladham, Hazem Almasri, Yaman Abu Lebdeh, Hisham Alsaif, Zaid Aldasht, Zakaria Aladem<br>
- Supervisor: Prof. Mohammad Abu Zalata<br>

