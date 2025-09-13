# DSBAM under AWGN (Simulink Study)

**Module:** Local Communication System & Application  
**Tags:** communications, modulation, Simulink, SNR

## Goal
Investigate how **Additive White Gaussian Noise (AWGN)** impacts a **Double Side-Band AM** system at different **SNR** levels, and verify observations against AM equations. :contentReference[oaicite:3]{index=3}

## Setup (Simulink)
- Sources: **Sine** and **Square** message signals
- Blocks: **DSB-AM Modulator (Passband)** → **AWGN Channel** (SNR mode) → **DSB-AM Demodulator (Passband)**
- Instruments: **Spectrum Analyzer** + **Scopes**
- Runs: **SNR = 0, 3, 6, 10, 20 dB**; total sim time ≈ **100 s** per run :contentReference[oaicite:4]{index=4}

## Results (Observed Trends)
- **Spectrum:** Peaks at **carrier + sidebands** become progressively **sharper & well-defined** as SNR increases; noise floor drops.  
- **Scope:** Time-domain waveforms stabilize with higher SNR—less amplitude jitter/shape distortion; **square** messages show the same trend. :contentReference[oaicite:5]{index=5}

## Recreate This
1. Build the chain (Mod → AWGN → Demod) with Spectrum/Scopes.  
2. Sweep SNR: 0 → 20 dB; capture screenshots.  
3. Compare **measured** sideband amplitudes vs **AM theory** (carrier/message indices). :contentReference[oaicite:6]{index=6}

## Reflection
Understanding **SNR thresholds** for acceptable clarity helps size **link budgets**, choose **filtering**, and set **minimum quality** for receivers in noisy channels. :contentReference[oaicite:7]{index=7}
