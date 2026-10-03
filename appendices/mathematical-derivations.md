# Appendix B: Mathematical Derivations

## B.1 Specific Contact Resistivity & Tunneling Derivation
For an ultra-thin Schottky barrier at the metal-silicon contact interface with barrier height $\Phi_B$ and heavy dopant concentration $N_D$, current transport is dominated by Field Emission (quantum mechanical tunneling).
The WKB tunneling probability transmission coefficient $T(E)$ yields specific contact resistivity $\rho_c$:

$$\rho_c \equiv \left( \left. \frac{\partial J}{\partial V} \right|_{V=0} \right)^{-1} \propto \exp\left( \frac{4\pi\sqrt{m^* \epsilon_s}}{h} \frac{\Phi_B}{\sqrt{N_D}} \right)$$

This demonstrates that to achieve target $\rho_c < 10^{-9}\ \Omega\cdot\text{cm}^2$:
1. The barrier height $\Phi_B$ must be engineered below $0.15\text{ eV}$ through workfunction tuning.
2. The active substitutional dopant concentration $N_D$ at the interface must exceed $2 \times 10^{20}\text{ cm}^{-3}$ via laser spike annealing.

## B.2 Negative Binomial Yield Formulation
In integrated circuit manufacturing, defects are not randomly distributed (Poisson); they cluster on wafers.
Assuming a gamma distribution of local defect density $D$ with mean $D_0$ and variance $\sigma^2 = D_0 + D_0^2 / \alpha$:

$$Y = \int_0^\infty \exp(-A D) \cdot f(D) \, dD$$

Where $f(D) = \frac{\alpha^\alpha D^{\alpha-1}}{\Gamma(\alpha) D_0^\alpha} \exp\left(-\frac{\alpha D}{D_0}\right)$.
Evaluating the integral:

$$Y = \frac{\alpha^\alpha}{\Gamma(\alpha) D_0^\alpha} \int_0^\infty D^{\alpha-1} \exp\left( -D \left[ A + \frac{\alpha}{D_0} \right] \right) \, dD$$

Using the definition of the Gamma function $\int_0^\infty x^{n-1} e^{-ax} dx = \frac{\Gamma(n)}{a^n}$:

$$Y = \frac{\alpha^\alpha}{\Gamma(\alpha) D_0^\alpha} \cdot \frac{\Gamma(\alpha)}{\left( A + \frac{\alpha}{D_0} \right)^\alpha} = \left( \frac{\alpha}{D_0 \left( A + \frac{\alpha}{D_0} \right)} \right)^\alpha = \left( 1 + \frac{A D_0}{\alpha} \right)^{-\alpha}$$

This proves the negative binomial yield model used universally by TSMC and Intel to predict die yields.
