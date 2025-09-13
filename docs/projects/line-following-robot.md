# Line-Following Robot (LCD + Obstacle Avoidance)

**Module:** Professional Practice Interactive Project  
**Tags:** robotics, embedded, sensors, LCD, safety

## Goal
Build a robot that follows a **black line on white floor**, **stops** safely for obstacles, then **continues**, with **audible alerts** and **LCD telemetry**. :contentReference[oaicite:13]{index=13}

## System & Pin Map
- **Motor Driver:** L293D (two DC motors)  
  - Motor A: **enA=9, in1=8, in2=7**  
  - Motor B: **enB=3, in3=5, in4=4**
- **Ultrasonic (HC-SR04):** **Trig=11, Echo=10**
- **Buzzer:** **D6**
- **LCD 16×2 (LiquidCrystal):** **RS=A2, EN=A3, D4=A4, D5=A5, D6=A6, D7=A7**  
- **IR sensors:** Analog inputs for line detection (threshold tuned via potentiometer) :contentReference[oaicite:14]{index=14}

## Approach
- Decision-logic (**if/else**) to follow line; stop/alert when obstacle within threshold; continue when clear.
- LCD shows **state + distance**; buzzer emits square-wave tone on obstacle.
- PWM on **enA/enB** for speed control; helper fns `moveForward()`, `turnLeft()`, `turnRight()`, `stopMotors()`. :contentReference[oaicite:15]{index=15}

## Issues & Fixes
- **Power brownouts** → regulated supply and wiring cleanup  
- **IR tuning** → threshold calibration for surface reflectance  
- **LCD over-voltage** → corrected wiring & current draw management  
- **Motor speed** → tuned PWM for smoother tracking :contentReference[oaicite:16]{index=16}

## Reflection
Robustness came from **pin-clean wiring**, sensible **PWM limits**, and **sensor calibration**.  
Next iteration: PID line control, better chassis, and cable management. :contentReference[oaicite:0]{index=0}

---

## Media

### Prototype Picture
![Line-Following Robot Prototype](assets/images/Line-Following-Robot-Picture.jpeg)

### Demo Videos
<video controls width="500">
  <source src="../assets/videos/line-following-robot-video-1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<video controls width="500">
  <source src="../assets/videos/line-following-robot-video-2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
