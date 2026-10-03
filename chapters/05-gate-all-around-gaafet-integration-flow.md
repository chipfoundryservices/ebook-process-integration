# Chapter 5: Gate-All-Around (GAAFET) Nanosheet Full Integration Flow

## 5.1 The 10-Step GAA Integration Sequence
Transitioning from FinFET to Gate-All-Around nanosheets (TSMC N2, Samsung 3GAP, Intel 20A) requires a revolutionary integration flow:
1. **Superlattice Epitaxy:** Alternating epitaxial growth of 3 to 4 periods of $\text{Si}_{0.7}\text{Ge}_{0.3}$ ($8\text{nm}$) and pure $\text{Si}$ ($5\text{nm}$) on bulk silicon.
2. **Fin Cut & Isolation:** Deep anisotropic etching of fin columns through the superlattice stack, followed by STI filling and recess.
3. **Dummy Gate & Spacer:** High-aspect-ratio polysilicon dummy gate patterning.
4. **Inner Spacer Cavity Etch:** Selective isotropic lateral recess of $\text{SiGe}$ layers adjacent to the channel ($2\text{–}3\text{nm}$ deep).
5. **Inner Spacer Deposition:** Conformal ALD deposition of low-k dielectric ($\text{SiBCN}$) and isotropic dry etch pullback to form the inner dielectric spacers that protect source/drain epitaxy from gate metal shorts.
6. **Source/Drain Epitaxy:** In-situ Boron-doped SiGe (pFET) and Phosphorus-doped Si (nFET) selective growth.
7. **Interlayer Dielectric (ILD) & CMP:** Oxide fill and CMP planarization down to dummy gate top.
8. **Dummy Gate Removal:** Selective chemical removal of polysilicon dummy gate.
9. **Nanosheet Release:** Highly selective isotropic chemical dry etch of sacrificial $\text{SiGe}$ layers, leaving suspended silicon nanosheet bridges.
10. **Dual-Workfunction HKMG:** Conformal ALD wrapping of $\text{HfO}_2$ and workfunction setting metal gates completely around all 4 sides of each suspended nanosheet.
