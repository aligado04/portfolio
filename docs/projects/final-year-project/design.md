# Design & Methodology

## Approach
Iterative path: **Tinkercad simulation → breadboard prototype → integrated enclosure**. Tools: **Arduino IDE**, **SolidWorks** for enclosure design. :contentReference[oaicite:6]{index=6}

## Hardware Choices
- **Ultrasonic (HC-SR04):** 2–400 cm range, ~±3 mm accuracy, robust to lighting (chosen over IR).  
- **Vibration motors:** fast response, low power, clear directional cues.  
- **Arduino Uno R3:** simplicity, community support, adequate I/O for 3 sensors + 3 motors + buzzer/LED.  
- **9V battery, LED, switches:** simple UX & maintenance. :contentReference[oaicite:7]{index=7}

## System Mapping
- **Ultrasonics:** front (7/8), left (9/10), right (11/12) on digital pins for precise pulse timing.  
- **Haptics:** motors on 3/4/5 (binary on/off).  
- **Buzzer:** D13 with **1 kΩ** series resistor (tone control + pin safety). 

## Enclosure Strategy
Printed a **modular box** that mounts on an off-the-shelf cane (don’t 3D-print the whole stick → size, durability, waste). SolidWorks enabled tight tolerances and serviceability. :contentReference[oaicite:9]{index=9}
