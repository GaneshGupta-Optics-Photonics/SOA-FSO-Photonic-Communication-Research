# Noise Figure Model for EDFA

## Overview

The noise figure (NF) is a fundamental parameter used to evaluate the degradation of signal-to-noise ratio (SNR) introduced by an optical amplifier.

In this work, the EDFA noise figure is used as a reference parameter for comparison with the semiconductor optical amplifier (SOA).

The noise figure difference between SOA and EDFA contributes to the amplifier noise penalty term in the analytical SOA–EDFA crossover model.

---

# Definition of Noise Figure

The noise figure is defined as the ratio between the input and output signal-to-noise ratios:

\[NF= {SNR_{in}}/{SNR_{out}}]

In decibel form:

\[NF_{dB}=10\log_{10}(NF)]

where:

- \(SNR_{in}\) is the signal-to-noise ratio before amplification.
- \(SNR_{out}\) is the signal-to-noise ratio after amplification.

An ideal amplifier would have:

\[NF=1]

or:

\[NF_{dB}=0\]

---

# EDFA Noise Figure

For an EDFA, the noise figure is mainly determined by amplified spontaneous emission (ASE) noise.

The approximate noise figure relationship is:

\[NF_{EDFA}\approx 2n_{sp}\]

where:

- \(n_{sp}\) is the spontaneous emission factor.

For a highly inverted EDFA:

\[n_{sp}\approx1\]

giving:

\[NF_{EDFA}\approx3\,dB\]

In practical C-band EDFAs, typical noise figures are:

\[NF_{EDFA}=4-6\,dB\]

---

# Noise Penalty Between SOA and EDFA

The noise figure difference is expressed as:

\[\∆ NF = NF_{SOA}-NF_{EDFA}\]

Because SOAs generally exhibit higher carrier-related noise contributions, the noise figure of SOA is typically higher than EDFA.

Therefore:

\[\∆ NF >0\]

indicating an EDFA noise advantage.

The corresponding SNR penalty can be written as:

\[\∆ SNR_{NF} = 10\log_{10}.({NF_{SOA}}/{NF_{EDFA}}]

---

# Role in SOA–EDFA Crossover Criterion

The noise figure difference competes with the scintillation suppression benefit of SOA.

The crossover occurs when:

\[ \∆ SNR_{scintillation} = \∆ SNR_{NF} \]

where:

- \(\∆ SNR_{NF}\) represents the EDFA noise advantage.
- \(\∆ SNR_{scintillation}\) represents the SOA turbulence suppression improvement.

At weak turbulence:

\[ C_n^2<C_{n,crossover}^{2}\]

the noise figure advantage dominates:

\[ \∆ SNR_{NF}> \∆ SNR_{scintillation}\]

Therefore, EDFA provides better performance.

At strong turbulence:

\[ C_n^2>C_{n,crossover}^{2} \]

the scintillation suppression benefit of SOA becomes dominant.

---

# Parameters Used for Comparison

| Parameter | EDFA | SOA |
|---|---|---|
| Typical noise figure | 4–6 dB | 6–10 dB |
| Main noise source | ASE noise | ASE + carrier noise |
| Recovery mechanism | Erbium population dynamics | Carrier dynamics |
| Response time | ms range | ps–ns range |

---

# Summary

The noise figure model establishes the low-turbulence performance advantage of EDFA.

Together with the Gamma-Gamma turbulence model and SOA carrier dynamics model, the noise figure contribution enables the development of a turbulence-dependent amplifier selection criterion for FSO communication systems.
