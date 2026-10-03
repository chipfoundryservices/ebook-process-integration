# Chapter 2: Middle-of-Line (MOL): Contact Engineering & Self-Aligned Vias

## 2.1 The Parasitic Contact Bottleneck
As contacted poly pitch (CPP) shrinks below $45\text{nm}$, source/drain contact area scales down to $<100\text{ nm}^2$. Total source-to-drain series resistance $R_{\text{SD}}$ becomes dominated by the specific contact resistivity $\rho_c$:

$$R_c = \frac{\rho_c}{A_{\text{contact}}}$$

At $\rho_c = 10^{-9}\ \Omega\cdot\text{cm}^2$ and $A = 50\text{ nm}^2$, $R_c = 2,000\ \Omega$ per contact, crippling transistor drive current ($I_{\text{on}}$).

## 2.2 Silicide / Germanide Contact Metallurgy
To lower $\rho_c$, fabs integrate advanced transition-metal contacts:
- **Cobalt & Nickel Silicide ($\text{CoSi}_2, \text{NiSi}$):** Replaced legacy titanium silicide.
- **Ruthenium & Titanium Silicide ($\text{TiSi}_x$):** Formed by atomic layer deposition of titanium followed by laser spike annealing ($>1000^\circ\text{C}$ for $<1\text{ms}$) to maximize dopant segregation at the interface without agglomerating into disconnected islands.

## 2.3 Self-Aligned Contact (SAC) Architecture
To prevent catastrophic short circuits between the gate electrode and adjacent source/drain contact plugs:
- Gate metal is recessed and capped with a hard silicon nitride dielectric cap ($\text{Si}_3\text{N}_4$).
- The contact opening is etched with extreme chemical selectivity ($>20:1$ oxide to nitride), allowing the contact via to overlap the gate without etching through the protective nitride helmet.
