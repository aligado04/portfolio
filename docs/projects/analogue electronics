# Current → Voltage Converter for Remote Motor Sensor

**Module:** Analogue Electronics  
**Tags:** op-amp, filters, Proteus, instrumentation

## Goal
Convert a **±2.5 mA** sensor current into a **2–3 V** signal suitable for downstream analysis/control, while suppressing high-frequency noise. :contentReference[oaicite:6]{index=6}

## Design & Method
- **Front-end:** Op-amp amplifier (LM741) sized for required **gain**; voltage divider biasing.  
- **Filtering:** **1st-order RC low-pass at 50 Hz** (≈ 91 nF & 35 kΩ) to reject noise above the sensing band.  
- **Simulation:** Built and validated in **Proteus**; verified gain/bandwidth and −3 dB cutoff. :contentReference[oaicite:7]{index=7}

## Outcome
- Achieved stable **2–3 V** output range from the simulated sensor current; frequency response matched the design (**50 Hz −3 dB**). :contentReference[oaicite:8]{index=8}

## Reflection
- Instrumentation chain thinking (biasing, gain, bandwidth) + practical filter sizing; next step would be **precision op-amp** and **PCB** for noise/layout control.
