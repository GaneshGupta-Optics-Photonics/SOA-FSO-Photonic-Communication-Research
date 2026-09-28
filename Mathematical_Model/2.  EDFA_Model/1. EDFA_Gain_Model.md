# EDFA Gain Model

## Overview

Erbium-doped fiber amplifiers (EDFAs) are widely used optical amplifiers because of their high gain, low noise figure, and mature fabrication technology.

In this work, the EDFA model is used as a reference amplifier for comparison with the semiconductor optical amplifier (SOA) in a turbulent free-space optical (FSO) communication system.

The EDFA performance is evaluated through:

- optical gain
- amplified spontaneous emission (ASE) noise
- noise figure
- received signal-to-noise ratio (SNR)

---

# EDFA Gain Equation

The small-signal gain of an EDFA can be expressed as:

\[G_{EDFA} =exp^⁡[(g.N_2-α.N_1 )⋅L_EDF]]        

where:

- \(G_{EDFA}\) is the optical gain
- \(g) is the emission cross-section
- \(α) is the absorption cross-section
- \(N_2\) is the excited erbium population density
- \(N_1\) is the ground-state population density
- \(L_EDF) is the erbium-doped fiber length

---

# Gain Saturation

At high input optical power, the EDFA gain decreases due to population depletion.

The saturated gain can be approximated as:

\[G_{sat}= {G_0}/{1+{P_{in}}/{P_{sat}}}]

where:

- \(G_0\) is the small-signal gain
- \(P_{sat}\) is the saturation power
- \(P_{in}\) is the input optical power

---

# EDFA Characteristics Used in Simulation

The EDFA parameters are selected based on typical C-band amplifier operation:

| Parameter | Symbol | Value |
|-|-|-|
| Operating wavelength | λ | 1550 nm |
| Small signal gain | \(G_0\) | 20–25 dB |
| Noise figure | NF | 4–6 dB |
| Saturation power | \(P_{sat}\) | 10–15 dBm |

---

# Role in SOA–EDFA Comparison

The EDFA model provides the baseline performance.

Under weak turbulence conditions, EDFA benefits from:

- lower noise figure
- lower ASE noise
- higher receiver sensitivity

However, unlike SOA, EDFA has slower carrier dynamics and limited capability for suppressing fast intensity fluctuations caused by atmospheric turbulence.
