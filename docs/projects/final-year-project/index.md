# Smart Assistive Navigation Cane (Final Year Project)

**Dissertation:** [Download PDF](../../assets/docs/final-year-project-dissertation.pdf)  
**Poster:** [View Poster](../../assets/docs/final-year-project-poster.pdf)

**Tags:** Arduino, ultrasonic, haptics, assistive tech, SolidWorks

## Summary
A low-cost, modular **assistive cane** that detects obstacles using **three ultrasonic sensors**
(front, left, right) and provides **directional haptic feedback**; if the user keeps approaching,
an **audible warning** escalates risk. LED status and a compact **3D-printed enclosure** complete the system. Validated with blindfold trials and iterative prototyping. 

- Sensors & mapping (example): **TRIG/ECHO** pairs on digital pins (front: 7/8; left: 9/10; right: 11/12)  
- Haptics: three vibration motors (front/left/right) on digital pins; simple on/off logic for clarity  
- Audio: buzzer with series **1 kΩ** resistor to smooth tone & protect MCU pin  
- Power/UI: **9V battery**, system switch, LED switch; modular enclosure mounted to a standard cane 

**Read more:**  
- [Design & Methodology](design.md)  
- [Implementation & Testing](testing.md)  
- [Outcomes & Future Work](outcomes.md)
