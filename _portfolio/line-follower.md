---
title: "Line Follower Robot – Line Follower Competition"
collection: portfolio
header:
  image: /images/500x300.png
  teaser: /images/500x300.png
---


<img src="{{ site.baseurl }}/images/lineFollower.jpg" width="500">
<br>High-speed autonomous line follower robot using PID control on ESP32, designed and tested in a large-scale university competition.<br>

<br>Robotics • Embedded Systems • Control • PID • ESP32


# Overview<br>

Designed and built a high-speed autonomous line follower robot for the Line Follower 2025 Competition, organized by ELCoM Team – Hashemite University.<br>
The robot competed in a large-scale event with ~50 teams, undergoing multiple elimination rounds over a 12-hour competition.<br><br>


## Robot constraints:<br>
  • Max size: 25 × 25 cm<br>
  • No AI / vision, classic control only<br><br>

## Robot Design<br><br>

### Mechanical<br>

Maximum length ~24 cm (near competition limit)<br>

Acrylic chassis (3 mm laser-cut)<br>

Rear-biased weight distribution to reduce rotational inertia<br>

Tradeoff: long body reduced tight-turn performance<br>
  → mitigated by adding side sensors<br><br>

### Drive System<br>

Differential drive (2 DC motors)<br>

L298N motor driver<br>

PWM speed control using ESP32 hardware timers<br><br>

Sensing<br>

10 IR line sensors<br>
  • QTR-8RC array (main)<br>
  • 2 additional side sensors for sharp turns and recovery<br>

Digital thresholding used instead of analog readings<br>
  • Analog values proved unstable under lighting variation<br><br>

### Electronics & Power<br>

ESP32 microcontroller<br>

Power system:<br>
  • 3× Li-ion batteries (12V nominal)<br>
  • Step-down regulator to 3.3V ESP32 rail<br>
  • Purpose: bypass ESP32 internal regulator overheating under load<br><br>

### Control Strategy<br><br>

Line Detection<br>

Weighted sensor array for position estimation<br>

Sensor weights mapped from left to right to compute lateral error<br>

Fallback logic when line is temporarily lost (uses last valid error)<br><br>

PID Control<br>

Closed-loop PID controller for steering correction<br>

Tuned empirically for competition track<br>

Parameters:<br>
  • Kp = 45<br>
  • Ki = 0.0001<br>
  • Kd = 60<br><br>

### Motion Logic<br>

Normal operation: PID-based differential speed control<br>

Sharp turns:<br>
  • Dedicated recovery routines (sharpLeft / sharpRight)<br>
  • Motors briefly reversed until line reacquired<br>

Start sequence via physical push button<br><br>

Software<br>

Platform: ESP32 (Arduino framework)<br>

Libraries:<br>
  • QTRSensors<br>

Features:<br>
  • Hardware PWM (ESP32 LEDC)<br>
  • Serial PID telemetry for tuning<br>
  • Modular motor and sensor functions<br>

Two independently developed control implementations were tested<br>
  (my version + teammate’s), sharing the same control philosophy<br><br>

Results & Lessons Learned<br>

Successfully completed all competition rounds<br>

Robot behavior was stable and predictable under high-speed conditions<br>

Key limitations identified:<br>
  • Excessive chassis length limited cornering<br>
  • Future versions should shorten the frame by 5–7 cm<br>

Reinforced importance of:<br>
  • Sensor placement over brute-force speed<br>
  • Clean power design on ESP32-based systems<br>
  • Robust line-loss recovery logic<br><br>

## Technologies Used<br>

ESP32<br>

QTR-8RC IR Sensor Array<br>

PID Control<br>

PWM Motor Control<br>

Embedded C++ (Arduino)<br><br>

## My Role<br>

Mechanical layout decisions<br>

Power system design<br>

PID tuning and control logic<br>

Sensor weighting and recovery behavior<br>

Debugging under competition conditions<br><br>
