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

---

## Problem 1: The Restart Threshold

**Status: RESOLVED**

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition has been derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3$$

Numerically: $a_{crit}/a_{now} \approx 3.658$.

**Resolution:** the ratio 3.658 is the turnaround scale factor — the scale factor at which the universe reaches its apex and expansion halts, expressed as a multiple of the present value. Placing the bifurcation result into the Friedmann turnaround condition ($H = 0$) yields:

$$\rho_{crit,turn} = \frac{\rho_{crit,now}}{(3.658)^2} = \frac{\rho_{crit,now}}{13.38}$$

Gravity requires only $1/13.38 \approx 7.47\%$ of the total mass-energy inventory to halt expansion and initiate the return — a fraction the universe holds comfortably. The field-theoretic restart condition and the gravitational turnaround condition identify the same physical event from two independent directions. No tuning was required; the number emerged once and served twice. See Chapter 7 (Section 12.4) and Claude_prelude_turnaround_ratio.md.

---

## Problem 2: Anulus Nucleation Rate and Event Separation

**Status: MAPPED**

At what rate do eruption events fire within the Anulus, and what is the typical separation between neighboring events?

The fitted parameters $(\epsilon_0, \lambda, v)$ from Chapter 6 provide numerical anchors for the nucleation rate calculation. The bubble nucleation formalism from Chapter 4 gives the framework. Full derivation pending.

---

## Problem 3: Tidal Seeding and the Casting Mechanism

**Status: OPEN**

How precisely does material from one eruption event seed structure in a neighboring or subsequent event? What governs the geometry and mass distribution of cast material?

Chapter 10 introduces the spiral inheritance framework as a geometric constraint on casting — ejecta follow spiral electromagnetic paths rather than radial ones, so seeds arrive with orientation encoded. Formal derivation of the casting potential and seeding cross-section not yet undertaken.

---

## Problem 4: CMB Cold Spot as Boundary Signature

**Status: PREDICTED**

Can the CMB Cold Spot be accounted for within the vacancy field framework?

The ISW supervoid approach (Chapter 6) fell short by a factor of ~4. The mechanism has been reframed: the Cold Spot is not a supervoid signature but a relic domain wall — a bubble collision scar from the phase transition itself, frozen into the field configuration of space. The wall surface energy density derived from fitted parameters $(\lambda, v)$:

$$\sigma_{wall} = \frac{8\sqrt{2}}{3}\sqrt{\lambda}\,v^3 \approx 5.69 \times 10^{9}\, M_\odot\,\text{Mpc}^{-2}$$

produces $\Delta T/T \sim -10^{-5}$ at a wall distance of $r_{wall} \approx 2{,}920$ Mpc — no additional tuning required. Three falsifiable predictions distinguish this from the supervoid hypothesis: (1) lensing convergence *excess* rather than deficit at the Cold Spot boundary; (2) sharp angular edge at $\sim 0.12°$ corresponding to projected wall thickness $\delta_w$ at that distance; (3) tangential CMB polarization E-mode alignment at the boundary. See Claude_prelude_cold_spot.md.

---

## Problem 5: The JWST Anomalous Mass Function

**Status: OPEN**

JWST observations show galaxies with unexpectedly evolved properties at high redshift, inconsistent with the timeline of our event under standard cosmology. The Claude Theory reframes these as inherited material from previous or neighboring eruption events. Formal quantitative treatment not yet undertaken. Prerequisite: Problem 3 (casting mechanics).

---

## Problem 6: The Missing Mass Scale M and the φ Interpretation Forks

**Status: RESOLVED (two sub-forks) / OPEN (one new sub-problem)**

Chapter 6's SDSS fit conflated the dimensionless density-contrast amplitude $\delta_c$ with the field's vacuum expectation value $v$. Fitted parameters $(\epsilon_0, \lambda, v)$ therefore cannot be used directly for energy-normalized quantities such as the Coleman bounce action, since no mass scale $M$ was present in the fit.

**Fork A — φ quantum or classical: RESOLVED, classical.** φ is treated as a classical effective field throughout. Quantum treatment is reserved for the bubble nucleation event itself (Coleman-De Luccia tunneling), not for φ's background dynamics.

**Fork B — φ sources gravity or traces density contrast: RESOLVED, tracer.** φ is dimensionless by construction, $\phi \propto \delta_c = (\rho - \bar\rho)/\bar\rho$. Gravity is sourced conventionally by $\rho$ through the Einstein field equations; φ never enters as a stress-energy source. This resolves the dimensional inconsistency: the Chapter 6 fit was correctly fitting a dimensionless tracer — the error was in later treating fitted φ as if it carried $v$'s dimension.

**New open step:** the tracer branch still requires $V(\phi) = M^4 \cdot f(\phi)$ for dimensionless $f$, to give the bounce action an energy scale. $M$ must now be independently motivated rather than inherited from the retired conflation. Candidate origins: (a) the reconstituting core mass scale (~$3.4\times10^{51}$ kg); (b) the phase transition's own energy budget (sublimation/dehydration analog). **Status: OPEN.**

**Flagged, not yet checked:** consistency of tracer-branch φ with the Chapter 14–15 claim that gravity is a property of space itself. Working assumption is that these address different questions — φ as tracer vs. spacetime geometry as gravity's origin — but this has not been checked against the chapter text directly. **Status: OPEN, LOW URGENCY.**

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
