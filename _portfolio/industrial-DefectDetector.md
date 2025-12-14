---
title: "Industrial Defect Detection"
collection: portfolio
header:
  image: /images/500x300.png
  teaser: /images/500x300.png
---


<img src="{{ site.baseurl }}/images/Defect-Detection.png" width="500">


[Link to video](https://www.linkedin.com/posts/zakaria-aladem-7b1659224_%D8%AE%D9%84%D8%A7%D9%84-%D8%AA%D8%AF%D8%B1%D9%8A%D8%A8%D9%8A-%D9%81%D9%8A-injo40-%D8%B9%D9%85%D9%84%D8%AA-%D8%B9%D9%84%D9%89-%D9%85%D8%B4%D8%B1%D9%88%D8%B9-%D9%8A%D8%AC%D9%85%D8%B9-activity-7393681430783975424-EyMQ?utm_source=share&utm_medium=member_desktop&rcm=ACoAADhWXjUBoSEkF3AIS0oyOwbEJ9wNAyvrbsA)



During my time at InJo4.0, I worked on a project that combined computer vision, and IoT communication to automate post-production quality inspection something traditionally done manually and prone to error.
The challenge was clear:
<br>How can we teach a machine to detect manufacturing defects as accurately as a human, but in real time?
<br>To solve this, I built a Defect Detection System powered by YOLOv8. The system captures an image after the robot completes assembly, identifies the product based on each product component (top, bolt, and bottom), and compares the configuration with the expected setup in node red.
<br>If the product meets specifications, it automatically sends an “Accept” command; otherwise, it flags it as “Reject.”
 This communication happens through MQTT, ensuring seamless real-time interaction between the AI system and the production line robot.

