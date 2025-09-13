# Process Control Comparison — DS vs ZN vs Smith Predictor

**Tags:** Simulink, time delay, tuning, chemical process

## Goal
Design and compare controllers for a **delayed second-order process** (chemical concentration loop, ~12-min transport delay). :contentReference[oaicite:2]{index=2}

## Controllers
- **Direct Synthesis (DS):** model-based, good stability/performance trade-off  
- **Ziegler–Nichols (ZN):** empirical tuning, fast but overshoot-prone  
- **Smith Predictor:** explicit delay compensation, smoother response

## Method
Step-response studies in Simulink; recorded **rise time, overshoot, settling, control effort**.

## Results (summary)
- **ZN:** quickest response, highest overshoot
- **DS:** balanced metrics across scenarios
- **Smith:** best at delay handling; low oscillation, good stability

## Reflection
Clear view of **empirical vs model-based** design and the value of **delay compensation** in industrial loops. :contentReference[oaicite:3]{index=3}
