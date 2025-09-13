# Pelican Crossing System (Year 1)

**Module:** Software Development for Embedded Systems  
**Tags:** embedded, Arduino, traffic-control, safety

## Goal
Build a pedestrian crossing that safely sequences **car lights** (green/yellow/red) and **pedestrian lights** (red/green) with a **tactile button** and an **audible cue**.

## System & Approach
- **MCU:** Arduino UNO  
- **I/O mapping:** Car LEDs → D10/D11/D12; Ped LEDs → D8/D9; Button → D2; Speaker → D7  
- **Logic:** Debounced button request → yellow → red (cars) → green (ped) for a fixed **crossTime** → flashing ped green → return to car green.  
- **Prototyping:** Flowchart → Tinkercad/Proteus simulation → breadboard build.

> (Add image) Place your screenshot at `docs/assets/images/interactive-traffic-light.png` and embed:  
> `![Breadboard + UNO layout](../assets/images/interactive-traffic-light.png)`

## Code (excerpt)
```cpp
int carRed=12, carYellow=11, carGreen=10, pedRed=9, pedGreen=8, button=2, speakerPin=7;
int crossTime=5000; unsigned long changeTime;
void setup(){ pinMode(carRed,OUTPUT); pinMode(carYellow,OUTPUT); pinMode(carGreen,OUTPUT);
  pinMode(pedRed,OUTPUT); pinMode(pedGreen,OUTPUT); pinMode(button,INPUT); pinMode(speakerPin,OUTPUT);
  digitalWrite(carGreen,HIGH); digitalWrite(pedRed,HIGH);
}
void loop(){ if(digitalRead(button)==HIGH && (millis()-changeTime)>5000) changeLights(); }
