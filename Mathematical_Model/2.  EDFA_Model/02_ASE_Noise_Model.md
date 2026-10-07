# Amplified Spontaneous Emission (ASE) Noise Model for EDFA

## Overview

Amplified spontaneous emission (ASE) noise is the dominant noise source in erbium-doped fiber amplifiers (EDFAs).

In this work, the ASE noise contribution of the EDFA is included to evaluate the amplifier noise penalty and compare the performance with a semiconductor optical amplifier (SOA) in a turbulent free-space optical (FSO) communication system.

The EDFA noise performance is characterized through:

- ASE power spectral density
- Optical signal-to-noise ratio (OSNR)
- Noise figure (NF)

---

# ASE Noise Generation

The ASE noise originates from spontaneous emission of excited erbium ions during optical amplification.

The ASE power generated within an optical bandwidth \(B_o\) is approximated as:

\[P_{ASE} = 2n_{sp}.(G_{EDFA}-1)hv.B_o]

where:

- \(P_{ASE}) is the ASE noise power
- \(n_{sp}) is the spontaneous emission factor
- \(G_{EDFA}) is the amplifier gain
- \(hv) is the photon energy
- \(B_o) is the optical bandwidth

The factor of 2 accounts for two orthogonal polarization modes.

---

# Spontaneous Emission Factor

The spontaneous emission factor is related to the population inversion of erbium ions:

\[n_{sp} = {N_2}/{N_2-N_1}]

where:

- \(N_2\) is the excited-state population density
- \(N_1\) is the ground-state population density

A higher population inversion reduces ASE noise and improves amplifier performance.

---

# Optical Signal-to-Noise Ratio

The output OSNR is calculated as:

\[OSNR = {P_{signal}}/{P_{ASE}}]

where:

- \(P_{signal}\) is the amplified optical signal power.
- \(P_{ASE}\) is the accumulated ASE noise power.

The OSNR reduction due to ASE directly affects the receiver performance.

---

# ASE Noise in EDFA-Based FSO Link

For the turbulent FSO system considered in this work, the received signal power can be expressed as:

\[P_r = G_{EDFA}.P_{in}.h_{atm}]

where:

- \(G_{EDFA}\) is the EDFA gain.
- \(P_{in}\) is the incident optical power.
- \(h_{atm}\) represents atmospheric turbulence-induced fading.

The receiver SNR is therefore limited by both:

1. Atmospheric scintillation noise.
2. EDFA ASE noise.

---

# Importance for SOA–EDFA Crossover Analysis

The ASE noise contribution creates the noise figure advantage of EDFA over SOA.

At weak turbulence:

\[C_n^2 < C_{n,crossover}^{2}]

the ASE noise contribution dominates system performance.

Therefore, the lower EDFA noise figure provides improved receiver sensitivity.

At strong turbulence:

\[C_n^2 > C_{n,crossover}^{2}]

the scintillation suppression capability of SOA becomes more significant than the ASE noise advantage of EDFA.

This trade-off defines the SOA–EDFA crossover condition.

---

# Simulation Parameters

Typical EDFA ASE parameters used for modelling:

| Parameter | Symbol | Value |
|---|---|---|
| Operating wavelength | λ | 1550 nm |
| Noise figure | NF | 4–6 dB |
| Gain | \(G_{EDFA}\) | 20–25 dB |
| Spontaneous emission factor | \(n_{sp}\) | 1.2–1.5 |
| Optical bandwidth | \(B_o\) | 0.1–1 nm |

---

# Summary

The ASE noise model provides the noise-performance baseline for EDFA amplification.

This model is used together with the Gamma-Gamma turbulence channel and SOA carrier-dynamics model to determine the turbulence-dependent amplifier selection criterion.
