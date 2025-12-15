---
title: "PET-Machine"
collection: portfolio
header:
  image: /images/500x300.png
  teaser: /images/500x300.png
---


<img src="{{ site.baseurl }}/images/PET2.png">
<img src="{{ site.baseurl }}/images/petPCB.jpg">
<br>Developed a PET-Machine for recycling plastic bottles into 3D printer filament, implementing a PID-controlled heating system to maintain precise extrusion temperatures.



<br>
Sustainability • Mechatronics • Embedded Systems • 3D Printing<br>
<br>
## Overview<br>
Designed and built a cost-effective "PETamontor" machine capable of recycling waste plastic bottles (PET) into functional 3D printer filament. The system utilizes a pultrusion process to cut, heat, and extrude plastic strips into 1.75mm filament, providing an environmentally friendly alternative to commercial materials.<br>
<br>
## Problem<br>
Standard 3D printing filament is expensive (approx. 30 JOD/kg), while plastic waste continues to harm the environment. Creating DIY filament is technically difficult due to:<br>
- **Inconsistent Quality:** Varying bottle properties can lead to poor filament.<br>
- **Crystallization:** If temperature control is inadequate, PET material crystallizes, changing its density and melting point.<br>
- **Clogging:** Improper heating causes material to crystallize inside the hotend.<br>
<br>
## Solution<br>
Developed a semi-automated pultrusion machine that:<br>
- Mechanically converts bottles into uniform ribbons using a variable cutter.<br>
- Precisely heats the plastic to 200°C to soften and reshape it without crystallizing.<br>
- Automates the spooling process using a high-torque gear reduction system.<br>
<br>
## System Architecture<br>
- **Mechanical Stage:** Custom fixture with razor blade for ribbonizing bottles.<br>
- **Thermal Stage:** V6 Heating block with a 12V 40W heater and K-Type thermocouple for thermal feedback.<br>
- **Control Stage:** Arduino Uno R3 utilizing a PID control loop to manage temperature stability.<br>
- **Drive System:** 12V High-Torque Worm Gear Motor (90 RPM) with PWM speed control.<br>
<br>
## Key Features<br>
- **PID Temperature Control:** Solves the crystallization issue by maintaining a stable 200°C, preventing clogging.<br>
- **Variable Cutter:** Adjustable blade height to control tape thickness and final filament diameter.<br>
- **High-Torque Spooling:** 3D-printed gear reduction converts high RPM to the high torque required to pull the filament through the nozzle.<br>
- **Customizability:** Allows for the creation of filament in various colors based on the source bottle.<br>
<br>
## Hardware & Component Selection<br>
- **Controller:** Arduino Uno R3.<br>
- **Sensors:** MAX6675 K-Type Thermocouple Module for high-temp readings.<br>
- **Actuators:** JGY-370 Worm Gear Motor (Reversible, High Torque).<br>
- **User Interface:** 16x2 LCD (Blue Screen) with Rotary Encoder for menu navigation.<br>
- **Power:** 12V 10A AC-DC Power Supply.<br>
<br>
## Technical Implementation<br>
- **Nozzle Modification:** Drilled standard nozzle to meet the 1.75mm filament requirement.<br>
- **Thermal Logic:** Implemented PID algorithm to handle the thermal inertia of the heating block.<br>
- **Motor Control:** Utilized PWM (Pulse Width Modulation) via a 1203B governor to fine-tune pulling speed.<br>
<br>
## Performance<br>
- Successfully reaches and maintains the target temperature of 200°C.<br>
- Reduces plastic waste by upcycling used bottles.<br>
- Produces usable filament compatible with standard 3D printers.<br>
<br>
## Technologies Used<br>
- Arduino (C++)<br>
- PID Control Algorithms<br>
- Circuit Design (Power regulation, Sensor integration)<br>
- CAD & 3D Printing (Gear reduction, Enclosure parts)<br>
- Thermal Dynamics<br>
<br>
## My Role<br>
- Designed the mechanical assembly for the spooler and cutter.<br>
- Selected and integrated electronic components (Arduino, MAX6675, Motor Drivers).<br>
- Programmed the PID controller to resolve crystallization issues.<br>
<br>
## Outcome<br>
Built a functional prototype that successfully turns trash into a manufacturing resource, providing a deep learning experience in joint mechanical and electrical engineering principles.<br>
