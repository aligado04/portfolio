# Implementation & Testing

## Build
- Integrated sensors, motors, buzzer, LED, battery, and switches per I/O map.  
- Breadboard → enclosed prototype; wiring kept accessible for iteration. :contentReference[oaicite:10]{index=10}

## Software
- Reusable `getDistance(trig, echo)` uses pulse timing for cm-accurate distance.  
- Tiered feedback: directional haptics first; **buzzer escalates** when within risk threshold. :contentReference[oaicite:11]{index=11}

## Trials
- **Blindfold walking tests:** consistent detection at shoulder-to-knee heights; durable modular mounting during motion. :contentReference[oaicite:12]{index=12}

## Notes
- Added **1 kΩ** series resistor on buzzer to smooth harsh tones & limit pin current. :contentReference[oaicite:13]{index=13}
