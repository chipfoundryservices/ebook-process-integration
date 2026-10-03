# Chapter 3: Back-End-of-Line (BEOL): Multilevel Interconnects & Low-k Integration

## 3.1 Interconnect RC Signal Delay Scaling
In sub-5nm logic, transistor intrinsic switching delay ($\tau_{\text{gate}} \approx C_g V / I_{\text{on}}$) drops below $1\text{ picosecond}$. In contrast, interconnect wire RC delay increases quadratically with scaling:

$$RC = \left( \rho \frac{L}{W \cdot H} \right) \cdot \left( 2\epsilon \frac{H \cdot L}{S} + 2\epsilon \frac{W \cdot L}{T_{\text{ILD}}} \right) \propto \rho \epsilon \frac{L^2}{W \cdot S}$$

Where $W$ is metal wire width and $S$ is wire spacing. As linewidth shrinks below $15\text{nm}$, copper resistivity $\rho$ surges by $5\text{–}10\times$ due to electron surface scattering (Fuchs-Sondheimer) and grain boundary scattering (Mayadas-Shatzkes).

## 3.2 Ruthenium and Alternative Metallization
To defeat copper's electron scattering catastrophe, the industry is transitioning lower metal layers (M0, M1, M2) to **Ruthenium ($\text{Ru}$)** and **Molybdenum ($\text{Mo}$)**:
- Ruthenium has a much shorter electron mean free path ($\lambda_{\text{mfp}} = 4.9\text{nm}$ vs. $39.9\text{nm}$ for Cu).
- At dimensions below $12\text{nm}$, pure Ruthenium lines exhibit lower total resistance than copper and require no resistive diffusion barrier layer ($\text{TaN}$), maximizing conductive cross-sectional area.
