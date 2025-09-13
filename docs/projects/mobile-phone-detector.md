# Mobile Phone Detector Circuit

**Module:** Linear Design & the Environment  
**Tags:** electronics, RF, op-amp, prototyping

## Goal
Detect nearby **active mobile phones** and indicate activity with an LED, with **adjustable sensitivity** and robust power handling.

## System & Approach
- **RF pickup:** Antenna + C2 → LM358 configured as frequency detector → LED via **BC548** (Q1).  
- **Tuning:** **RV1/VR1** adjust sensitivity/range; **T1** amplifies the signal at LM358 pin-1.  
- **Power:** Voltage control/current limiting; battery powered.  
- **Note:** Designed for **2G/GPRS/manual network search**; limited with **3G/WCDMA/HSDPA** signals. :contentReference[oaicite:3]{index=3}

## Test Procedure & Results
- Power-on baseline (LED off) → bring an active phone near the antenna → **LED flashes**; move away → stops.  
- Sensitivity increases when RV1 is turned clockwise; repeatable over multiple trials; range improved with VR1. :contentReference[oaicite:4]{index=4}

## Reflection
- Clear trade-off between sensitivity and false positives; next steps: **band-select filtering** and characterization across carriers/bands. :contentReference[oaicite:5]{index=5}
