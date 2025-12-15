---
title: "Defect Detection System for Industrial Production Line (YOLOv8)"
collection: portfolio
header:
  image: /images/500x300.png
  teaser: /images/500x300.png
---


<img src="{{ site.baseurl }}/images/Defect-Detection.png" width="500">
<br>Real-time system using YOLOv8 and MQTT to detect assembly defects and automate accept/reject decisions, enhancing speed and reliability.<br>

[Link to video](https://www.linkedin.com/posts/zakaria-aladem-7b1659224_%D8%AE%D9%84%D8%A7%D9%84-%D8%AA%D8%AF%D8%B1%D9%8A%D8%A8%D9%8A-%D9%81%D9%8A-injo40-%D8%B9%D9%85%D9%84%D8%AA-%D8%B9%D9%84%D9%89-%D9%85%D8%B4%D8%B1%D9%88%D8%B9-%D9%8A%D8%AC%D9%85%D8%B9-activity-7393681430783975424-EyMQ?utm_source=share&utm_medium=member_desktop&rcm=ACoAADhWXjUBoSEkF3AIS0oyOwbEJ9wNAyvrbsA)


<br>
Computer Vision • Industrial Automation • IoT • Deep Learning<br>
<br>
## Overview<br>
Designed and implemented an automated defect detection system for an industrial production line at InJo 4.0, using YOLOv8 for real-time visual inspection and MQTT for seamless integration with robotic and SCADA systems.<br>
The system performs post-assembly quality control, automatically accepting or rejecting products based on detected components and expected configurations.<br>
<br>
## Problem<br>
Manual inspection was:<br>
- Slow and inconsistent<br>
- Error-prone under high throughput<br>
- Difficult to synchronize with robotic assembly<br>
<br>
## Solution<br>
Built an end-to-end AI-based inspection pipeline that:<br>
- Detects assembled components (top, bolt, bottom)<br>
- Generates a unique product code<br>
- Compares detected configuration with expected assembly<br>
- Sends ACC / REJ commands to the production system in real time<br>
<br>
## System Architecture<br>
- YOLOv8 Object Detection for component recognition<br>
- Python + Ultralytics for training and inference<br>
- MQTT (paho-mqtt) for real-time communication<br>
- Robot state synchronization to ensure inspection only occurs when the product is ready<br>
<br>
## Key Features<br>
- Real-time inspection after robot assembly confirmation<br>
- Component-level verification (missing or incorrect parts)<br>
- Automatic decision-making (Accept / Reject)<br>
- Robust timing control to prevent duplicate commands<br>
- Designed for industrial reliability, not demos<br>
<br>
## Dataset & Training<br>
- Custom dataset annotated using CVAT<br>
- YOLO format (YOLOv8 / YOLO1.1)<br>
- Multiple product configurations and defect classes<br>
- Data augmentation (rotation, scaling, color jitter)<br>
<br>
## Training Highlights<br>
- Model: YOLOv8s<br>
- Custom augmentation strategy<br>
- GPU-accelerated training<br>
- Evaluation using mAP, precision, recall, and qualitative predictions<br>
<br>
## Performance<br>
- Accurate detection of assembled components<br>
- Reliable rejection of defective products<br>
- Stable real-time operation on production line timing constraints<br>
<br>
## Technologies Used<br>
- YOLOv8 (Ultralytics)<br>
- Python<br>
- PyTorch<br>
- MQTT (paho-mqtt)<br>
- CVAT<br>
- Industrial automation protocols<br>



