# Atmospheric Turbulence Theory for FSO Communication

## Overview

Atmospheric turbulence is one of the major impairments in free-space optical (FSO) communication systems.

Random temperature and pressure variations create fluctuations in the atmospheric refractive index, causing variations in optical intensity at the receiver.

These intensity fluctuations are known as optical scintillation.

The turbulence strength is characterized by the refractive index structure parameter:

\[
C_n^2
\]

where:

- \(C_n^2\) represents the strength of atmospheric turbulence.
- Higher values indicate stronger turbulence.

---

# Refractive Index Structure Parameter

The refractive index fluctuation is commonly represented using the Kolmogorov turbulence model:

\[
\Phi_n(\kappa)=0.033C_n^2\kappa^{-11/3}
\]

where:

- \(\Phi_n(\kappa)\) is the refractive index power spectrum.
- \(\kappa\) is the spatial frequency.

---

# Optical Wave Propagation

The strength of turbulence experienced by an optical wave depends on:

- wavelength
- propagation distance
- atmospheric conditions

The optical wave number is:

\[
k=\frac{2\pi}{\lambda}
\]

where:

- \(\lambda\) is the optical wavelength.

---

# Rytov Variance

The Rytov variance is used to quantify turbulence effects:

\[
\sigma_R^2=
1.23 C_n^2 k^{7/6}L^{11/6}
\]

where:

- \(L\) is the propagation distance.
- \(k\) is the optical wave number.

The turbulence regime is classified as:

| Rytov variance | Turbulence condition |
|---|---|
| \(\sigma_R^2 < 1\) | Weak turbulence |
| \(\sigma_R^2 \approx 1\) | Moderate turbulence |
| \(\sigma_R^2 > 1\) | Strong turbulence |

---

# Role in Present Work

In this research, the turbulence strength is varied through \(C_n^2\).

The Gamma-Gamma model is used to generate irradiance fluctuations and evaluate the influence of atmospheric turbulence on SOA and EDFA amplified FSO links.

The turbulence model provides the scintillation contribution:

\[
\Delta SNR_{scint}
\]

which is compared against the amplifier noise penalty:

\[
\Delta SNR_{NF}
\]

to determine the SOA–EDFA crossover condition.
