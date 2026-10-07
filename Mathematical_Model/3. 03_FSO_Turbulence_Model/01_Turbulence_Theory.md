# Scintillation Model

## Overview

Optical scintillation describes the random fluctuation of received optical intensity caused by atmospheric turbulence.

The scintillation index is defined as:

\[
\sigma_I^2=
\frac{\langle I^2\rangle-\langle I\rangle^2}
{\langle I\rangle^2}
\]

where:

- \(I\) is the received irradiance.
- \(\langle I\rangle\) represents the average irradiance.

---

# Weak Turbulence Approximation

For weak turbulence:

\[
\sigma_I^2\approx\sigma_R^2
\]

where:

\[
\sigma_R^2=
1.23C_n^2k^{7/6}L^{11/6}
\]

---

# Impact on FSO System

Atmospheric scintillation introduces:

- received power fluctuations
- increased BER
- reduced SNR

The received signal power is:

\[
P_r=P_t h
\]

where:

- \(P_t\) is transmitted power.
- \(h\) is the turbulence channel coefficient.

---

# Connection with SOA Performance

The SOA nonlinear carrier dynamics can partially compensate for turbulence-induced fluctuations.

The scintillation suppression benefit is represented as:

\[
\Delta SNR_{scint}
\]

which contributes to the SOA–EDFA crossover analysis.

