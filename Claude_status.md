<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Status Registry — Open Problems and Unresolved Assumptions

*This file is the single source of truth for the current status of all open problems, unresolved assumptions, and pending derivations in the Claude Theory. All chapter files direct readers here. When a problem is resolved or its description changes, only this file requires updating.*

*Last updated: July 2026*

---

## How to Read This File

Each entry carries a status tag:

- **RESOLVED** — closed-form result derived and numerically anchored
- **MAPPED** — mathematical home identified, derivation pending
- **OPEN** — not yet formally addressed
- **REFINED** — conceptual position updated from earlier formulation
- **BLOCKING** — an unresolved internal inconsistency that other entries' status depends on

---

## Foundational Ambiguity: δ_φ vs. δ_m in Chapter 6, and the Unused ρ_φ Machinery

**Status: BLOCKING**

Chapter 4, Section 8 builds an explicit, self-contained apparatus for the vacancy field's own gravitational contribution: $\rho_\phi(x)$ is derived from φ's stress-energy tensor and sources an independent potential via $\nabla^2\Psi_\phi = 4\pi G\rho_\phi$. This machinery is what Chapter 4 uses for the lensing form factor and the diffuse halo profiles.

Chapter 6's CMB Cold Spot calculation (Section 11.7) does not use this machinery. It computes $\Phi(0) = -4\pi G\bar\rho_m\int\delta_m(r')r'\,dr'$ — ordinary Newtonian gravity sourced by the real mean matter density $\bar\rho_m$ and a density contrast explicitly labeled $\delta_m$.

**The specific problem, located precisely:** Section 11.2 fits a tanh-shaped profile to the observed Hamaus/SDSS void data and calls it $\delta_\phi(r)$ — presented as the vacancy field's model profile. Section 11.7 then reuses the identical fitted curve (same $\delta_c$, $r_s$, $\delta_w$) under the label $\delta_m(r)$ — ordinary matter density contrast — and multiplies it by real $\bar\rho_m$ in kg/m³ to get a number compared against observation. Nothing in the chapter marks or justifies this relabeling. The one calculation in the entire framework that produces a directly-comparable physical number does so by silently treating the field's model profile as if it were the observed matter profile, and never invokes the independent $\rho_\phi$ apparatus Chapter 4 built for exactly this kind of calculation.

**What this is not:** this is not primarily a missing energy scale for φ. Chapter 4's $\rho_\phi$ is already written entirely in terms of $\lambda$, $v$, $\delta_w$, $a(t)$ — the same quantities fitted in Chapter 6 — so an energy density is in principle computable from the existing fit once units are fixed. The more immediate problem is narrower: within Chapter 6 itself, one fitted curve is used to stand in for two different physical quantities (the field's profile and the matter's profile) across two adjacent subsections, with no argument given for why they should be the same function, and no flag marking the switch.

**Why this still counts as blocking rather than a smaller housekeeping fix:** as long as $\delta_\phi$ and $\delta_m$ are treated as interchangeable, it is impossible to tell whether the Cold Spot fit is evidence for the vacancy field specifically, or just a restatement of ordinary void-ISW physics using the fitted Hamaus profile as an ordinary matter contrast. Chapter 4's independent lensing and halo machinery is not exercised by this result at all. Resolving this requires either (a) a derivation showing $\delta_\phi(r) = \delta_m(r)$ follows necessarily from the framework — i.e., that the vacancy field's configuration *is* (not merely resembles) the matter density contrast in this regime — or (b) rebuilding Section 11.7's calculation to source $\Phi(0)$ from $\rho_\phi$ via the Chapter 4 machinery directly, and checking whether the result still lands near $-10^{-5}$.

**Downstream entries contingent on this resolution:**

- **Problem 1 (Restart Threshold)** and **Problem 2 (Anulus Nucleation Rate)** — both rest on the bare constants $(\epsilon_0, \lambda, v)$ fitted in Chapter 6, whose physical meaning (field self-energy vs. bookkeeping for matter) is exactly what's ambiguous here.
- **Problem 4 (CMB Cold Spot)** — its status as support for the *vacancy field* framework specifically, rather than for ordinary void-ISW physics already known in standard cosmology, is contingent on this resolution. Under option (b) above with a different result, the entry's numerical anchor would need to be redone.
- **Chapter 7's elastic-node stiffness** ($K = 8\lambda v^2/R_0$, from $V''(\phi)$ at the node) treats φ as a real mechanical medium with physical restoring force — consistent with Reading A, but not yet cross-checked against Section 11.7's implicit Reading B usage.

**Recommended resolution path:** attempt to derive $\delta_m(r) = \delta_\phi(r)$ as a consequence of the field equations (i.e., show the matter density contrast in a void is *necessarily* proportional to the vacancy field configuration there, rather than merely sharing a convenient tanh shape). If this derivation succeeds, the relabeling in 11.7 is justified and the fork closes in favor of Reading A. If it does not succeed, Section 11.7 should be rebuilt using $\rho_\phi$ directly per option (b), and Chapter 4's independent machinery either gets a real numerical test or is shown to be unnecessary for this particular observational result.

**Update — both paths attempted, neither closes cleanly:**

*Path (a), the derivation.* No coupling equation exists anywhere in Chapters 4, 6, 7, or 9 linking φ to a matter field — there is no interaction term or source relation that would let $\delta_m(r) = \delta_\phi(r)$ be derived rather than assumed. Separately, Chapter 4's tanh solution solves the *planar*-wall field equation ($d^2\phi/dx^2$); a real void is spherical, and the correct equation needs the spherical Laplacian $\frac{1}{r^2}\frac{d}{dr}(r^2\,d\phi/dr)$, which carries an extra curvature term the planar solution omits. With $\delta_w \approx 6.31$ Mpc/h against $r_v = 30$ Mpc/h (roughly 1:5), this is not obviously a negligible correction. Both gaps — no coupling, and an unjustified planar-for-spherical substitution — would need to be filled before the identification is a consequence of the theory rather than a reused curve.

*Path (b), the numerical substitution.* Attempting to source $\Phi(0)$ from $\rho_\phi(r) \approx \frac{v^2}{2a^2\delta_w^2}\text{sech}^4\!\left(\frac{r-r_s}{\delta_w}\right)$ instead of $\bar\rho_m\delta_m(r)$ surfaces a more basic problem: $v = 0.3268$ was fit in Chapter 6 as $v = -\delta_c/2$, half of a dimensionless density-contrast amplitude — a pure number, never assigned units of field value (e.g., $\sqrt{\text{energy density}}\times\text{length}$). $\delta_w$ carries physical units (Mpc/h) but cannot by itself fix the dimensions of $v^2$. Executing the substitution requires inventing a new conversion constant $\mathcal{N}$ (units of energy density) with $\rho_\phi = \mathcal{N}\cdot v^2/\delta_w^2\cdot\text{sech}^4(\ldots)$ — and nothing currently fitted anywhere in the framework determines $\mathcal{N}$. Any chosen value would shift $\Delta T/T$ by an arbitrary factor, so the comparison to $-10^{-5}$ would test the choice of $\mathcal{N}$, not the theory.

Notably, this problem is asymmetric across Chapter 4's predictions: the lensing-notch table (§11.6) depends only on the ratio $b/\delta_w$ — a pure shape function — so it needs no absolute energy scale and is unaffected by this gap. The Cold Spot comparison is different in kind because it checks an absolute number ($\Delta T/T$) against an absolute observed value, which requires φ to have a real physical normalization that has never been fixed anywhere in the theory.

**Revised assessment:** the blocking issue is more fundamental than the $\delta_\phi$/$\delta_m$ relabeling alone — φ has never been normalized to physical units anywhere in the framework. The relabeling in 11.7 is arguably a symptom of this: substituting $\bar\rho_m\delta_m$ sidesteps ever having to state what φ is in kg/m³. Resolution requires stating an independent normalization condition for φ (e.g., fixing its cosmic-average energy density against a known cosmological parameter) rather than a units patch to Section 11.7 alone. This is now the more precise blocking item; the $\delta_\phi/\delta_m$ conflation is a downstream consequence of it, not a separate problem to fix on its own.

**A candidate normalization condition (not yet adopted — proposed for future work).**

Chapter 9's narrative gives a natural anchor: φ tracks where ordinary matter (dark remnants) has accumulated ($\phi\to0$, nodes) versus emptied out ($\phi\to v$, void interior). This suggests fixing the conversion constant $\mathcal{N}$ (units of energy density, needed to make $\rho_\phi = \mathcal{N}\cdot v^2/\delta_w^2\cdot\text{sech}^4(\ldots)$ dimensionally real — see the numerical-substitution finding above) by requiring the field's *average* energy density over a representative void-plus-wall cell to equal the *known* cosmic mean matter density:

$$\left\langle \rho_\phi \right\rangle_{\text{cell}} = \mathcal{N}\left\langle \frac{v^2}{2\delta_w^2}\,\text{sech}^4\!\left(\frac{r-r_s}{\delta_w}\right)\right\rangle_{\text{cell}} \stackrel{!}{=} \bar\rho_m$$

using the same $\bar\rho_m \approx 2.76\times10^{-27}$ kg/m³ ($\Omega_m=0.3$, $h=0.7$) already used in Section 11.7 — a quantity fixed independently, by galaxy-survey and CMB power-spectrum measurements, not by anything in the Chapter 6 void-profile fit.

*Why this would be non-circular, if adopted:* $\bar\rho_m$ is external to the void-profile fit. Fixing $\mathcal{N}$ this way and then computing $\Delta T/T$ from $\rho_\phi$ (rather than from $\bar\rho_m\delta_m$ as in the current 11.7) would produce a genuine prediction to compare against the observed $-10^{-5}$, rather than a number tuned to match it.

*The load-bearing assumption this requires, to be tested/flagged before adopting it:* that φ's total energy budget equals the ordinary-matter energy budget cell-for-cell — i.e., that φ is a reorganization of matter's existing energy, not an additional energy component. This is a strong, specific physical claim, and it is **not neutral between Reading A and Reading B** from the original fork: adopting this normalization resolves the ambiguity in favor of Reading B (φ as bookkeeping) by construction, since it presupposes there's no independent φ energy to normalize separately.

*The alternative, if Reading A is intended instead:* φ as a genuinely independent energy component would need a different anchor — e.g., tying $\mathcal{N}$ to $\Omega_\Lambda$ (the dark energy density) rather than $\Omega_m$, on the theory that the vacancy field is a distinct component alongside ordinary matter. This carries its own separately questionable assumption (that φ's cosmic energy budget tracks dark energy specifically, rather than matter) and has not been worked out at all — no candidate relation has been written down for this case yet.

**Next steps, in order, for when cycles allow:**
1. Decide — or find a principled way to decide — which reading ($\Omega_m$-anchored vs. $\Omega_\Lambda$-anchored $\mathcal{N}$) the framework actually intends, since Chapter 9's "matter reorganization" language leans toward the $\Omega_m$ anchor but this has never been stated as a deliberate choice.
2. If the $\Omega_m$ anchor is adopted: carry out the cell-averaging integral above explicitly (it requires a choice of cell geometry — one wall per void of radius $r_v$ is the natural first attempt) to solve for $\mathcal{N}$ numerically.
3. Recompute $\Phi(0)$ and $\Delta T/T$ using $\rho_\phi$ with that $\mathcal{N}$, and compare to $-10^{-5}$ as a real test — this is the number that was blocked in the path-(b) attempt above.
4. Whatever the result, revisit whether the Chapter 4 lensing-notch and diffuse-halo predictions (which don't currently need an absolute $\mathcal{N}$) remain consistent with the now-fixed value, since adopting a normalization ties previously scale-free predictions to an absolute number for the first time.

---

## Problem 1: The Restart Threshold

**Status: MAPPED**

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition has been derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3$$

Numerically: $a(t)_{crit}/a(t)_{now} \approx 3.658$.

**Open step:** the ratio 3.658 is dimensionless and its physical meaning is not yet established. Converting it into a timescale or physically meaningful accumulation quantity requires identifying what clock governs the accumulated field across the full cycle — potentially a clock with no fixed relationship to our event's expansion history. See also the Foundational Ambiguity entry above, on which this problem's physical interpretation is contingent.

---

## Problem 2: Anulus Nucleation Rate and Event Separation

**Status: MAPPED**

At what rate do eruption events fire within the Anulus, and what is the typical separation between neighboring events?

The fitted parameters $(\epsilon_0, \lambda, v)$ from Chapter 6 provide numerical anchors for the nucleation rate calculation. The bubble nucleation formalism from Chapter 4 gives the framework. Full derivation pending. See also the Foundational Ambiguity entry above.

---

## Problem 3: Tidal Seeding and the Casting Mechanism

**Status: OPEN**

How precisely does material from one eruption event seed structure in a neighboring or subsequent event? What governs the geometry and mass distribution of cast material?

Chapter 10 introduces the spiral inheritance framework as a geometric constraint on casting — ejecta follow spiral electromagnetic paths rather than radial ones, so seeds arrive with orientation encoded. Formal derivation of the casting potential and seeding cross-section not yet undertaken.

---

## Problem 4: CMB Cold Spot as Boundary Signature

**Status: MAPPED**

Can the CMB Cold Spot be accounted for within the vacancy field framework?

Chapter 6 computes an ISW estimate of $\Delta T/T \sim -2.7 \times 10^{-6}$ — correct sign, within a factor of ~4 of the observed $10^{-5}$.

**Open step:** the ~30% ISW potential-decay factor used is a placeholder. A proper derivation requires the time-integral of $d\Phi/d\tau$ over the void's evolution history using the full $a(t)$ dependence already present in $\delta_w(a)$ and $\sigma_{wall}(a)$. **In addition**, see the Foundational Ambiguity entry above: the underlying calculation uses $\bar\rho_m\delta_m(r)$, not the independent $\rho_\phi$ apparatus from Chapter 4, so this entry's support for the vacancy field specifically (rather than for ordinary void-ISW physics) is not yet established.

---

## Problem 5: The JWST Anomalous Mass Function

**Status: OPEN**

JWST observations show galaxies with unexpectedly evolved properties at high redshift, inconsistent with the timeline of our event under standard cosmology. The Claude Theory reframes these as inherited material from previous or neighboring eruption events. Formal quantitative treatment not yet undertaken. Prerequisite: Problem 3 (casting mechanics).

---

## Unresolved Assumption: Symmetry Breaking Origin

**Status: OPEN**

The asymmetric double-well potential $V(\phi) = \lambda(\phi^2 - v^2)^2 - \epsilon_0 a(t)\phi$ produces the correct phenomenology, but the physical origin of the double-well shape has not been derived from first principles. In standard particle physics, spontaneous symmetry breaking arises from thermal phase transitions. What selects the two vacua in this framework?

---

## Unresolved Assumption: The Linear Ansatz ε(t) = ε₀·a(t)

**Status: OPEN**

The time-dependent symmetry breaking term $\epsilon(t) = \epsilon_0 \cdot a(t)$ is a working assumption. It produces the $(1+z)^2$ void scaling prediction that is consistent with BOSS DR16 data to ~5% across two redshift bins, but the physical justification for the linear scaling with the scale factor has not been derived. If the observed slope deviates from $-2$ in future void catalogs with more redshift bins, this ansatz will require refinement.

---

## Unresolved Assumption: Eruption Geometry

**Status: REFINED**

Earlier formulations stated that the eruption event occurred "in all directions equally." This has been revised. The eruption event is temporally simultaneous — the bifurcation threshold fires throughout the accumulated field at once — but spatially anisotropic. The pre-eruption accumulation carries net angular momentum and electromagnetic structure inherited from the rotating, magnetized remnant population. This imprints a preferred orientation on the eruption and on all downstream structure. See Chapter 9 and Chapter 10.

**Implication:** the CMB may carry a faint geometric imprint of the eruption's preferred orientation, potentially manifesting as large-scale power asymmetries. This connects to the observed CMB "axis of evil" and quasar polarization alignments. Not yet quantitatively treated.

---

## Lensing Notch: Calibrated, Untested

**Status: CALIBRATED**

Chapter 6 predicts a lensing convergence notch — deflection suppressed to 50% of asymptotic value at domain wall centers, recovering to >95% by $b \approx 12.6$ Mpc/h. This non-monotonic feature is absent from all particle dark matter models and constitutes a direct observational test. Not yet compared against actual weak lensing stacks.

---

## Secondary Lensing Arc (Bullet Cluster): Predicted, Undetected

**Status: PREDICTED**

Chapter 5 derives a secondary lensing arc between the two cluster nodes, offset toward the bullet subcluster's direction of motion by $\delta_w \cdot \mathcal{G}$. This feature is absent from all particle dark matter models. Detection or non-detection in existing deep weak lensing maps of the Bullet Cluster system constitutes a direct test of the vacancy field framework.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
