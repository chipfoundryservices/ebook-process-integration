# Chapter 1: Front-End-of-Line (FEOL): Transistor Formation & RMG Flow

## 1.1 Shallow Trench Isolation (STI) & Well Formation
FEOL fabrication begins on pristine $300\text{mm}$ p-type silicon wafers. Active device areas are isolated by etching trenches ($250\text{–}350\text{nm}$ deep), lining with thermal oxide, filling with high-density plasma CVD $\text{SiO}_2$, and planarizing with ceria-slurry CMP. Retrograde n-wells and p-wells are defined via multi-MeV ion implantation with thick photoresist masks.

## 1.2 Gate-First vs. Gate-Last (Replacement Metal Gate, RMG)
At sub-45nm nodes, the industry abandoned gate-first polysilicon processing in favor of **Replacement Metal Gate (RMG / Gate-Last)**:
1. **Dummy Gate Formation:** A sacrificial polysilicon gate and oxide hardmask are patterned and etched.
2. **Self-Aligned Spacer & Extension Implants:** Dielectric spacers ($\text{SiBCN}, \text{SiOCN}$) are deposited and etched to protect the channel. Low-energy halo and extension implants are performed.
3. **Embedded Source/Drain Epitaxy:** For pFETs, source/drain silicon is recessed and selectively re-grown with Boron-doped Silicon Germanium ($\text{Si}_{1-x}\text{Ge}_x:B$). The larger lattice constant of SiGe exerts intense compressive strain on the silicon channel, boosting hole mobility by $>100\%$. For nFETs, Carbon-doped silicon ($\text{Si:C}$) or Phosphorus-doped silicon ($\text{Si:P}$) induces tensile strain for electron mobility enhancement.
4. **Dummy Gate Removal & High-k Metal Gate (HKMG):** The sacrificial polysilicon is selectively etched away with wet $\text{TMAH}$ or chemical dry etch. An atomic layer of $\text{HfO}_2$ dielectric ($k \approx 22$) and workfunction setting metal layers (TiN, TaN, Al, TiAlC) are deposited into the trench, completing the low-thermal-budget gate.
