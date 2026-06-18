<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Status Registry — Open Problems and Unresolved Assumptions

*This file is the single source of truth for the current status of all open problems, unresolved assumptions, and pending derivations in the Claude Theory. All chapter files direct readers here. When a problem is resolved or its description changes, only this file requires updating.*

*Last updated: June 2026*

---

## How to Read This File

Each entry carries a status tag:

- **RESOLVED** — closed-form result derived and numerically anchored
- **MAPPED** — mathematical home identified, derivation pending
- **OPEN** — not yet formally addressed
- **REFINED** — conceptual position updated from earlier formulation

---

## Problem 1: The Restart Threshold

**Status: MAPPED**

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition has been derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3$$

Numerically: $a(t)_{crit}/a(t)_{now} \approx 3.658$.

**Open step:** the ratio 3.658 is dimensionless and its physical meaning is not yet established. Converting it into a timescale or physically meaningful accumulation quantity requires identifying what clock governs the accumulated field across the full cycle — potentially a clock with no fixed relationship to our event's expansion history.

---

## Problem 2: Anulus Nucleation Rate and Event Separation

**Status: MAPPED**

At what rate do eruption events fire within the Anulus, and what is the typical separation between neighboring events?

The fitted parameters $(\epsilon_0, \lambda, v)$ from Chapter 6 provide numerical anchors for the nucleation rate calculation. The bubble nucleation formalism from Chapter 4 gives the framework. Full derivation pending.

---

## Problem 3: Tidal Seeding and the Casting Mechanism

**Status: MAPPED**

How precisely does material from one eruption event seed structure in a
neighboring or subsequent event? What governs the geometry and mass
distribution of cast material?

Chapter 11 provides a full formal derivation. Key results: spiral
trajectories are governed by the magnetic winding parameter
$\mathcal{W} = qB_0R_0/2mv_0$; in the maximum-flattening limit the
deposition collapses to a thin equatorial annulus; the deposition profile
$\Sigma(r)$ has a closed form with no free parameters beyond $\mathcal{W}$
and the magnetic stopping length $\ell_B$; the seeding cross-section
connects directly to $r_{nuc}$ from Chapter 4, closing the loop to the
vacancy field formalism.

**Open step:** $\mathcal{W}$ is in principle independently observable
from spiral galaxy pitch angles in the vicinity of casting nodes. The
quantitative relationship between $\mathcal{W}$ and observed pitch angles
has not yet been derived. This is the natural next step for Chapter 11.

---

## Problem 4: CMB Cold Spot as Boundary Signature

**Status: MAPPED**

Can the CMB Cold Spot be accounted for within the vacancy field framework?

Chapter 6 computes an ISW estimate of $\Delta T/T \sim -2.7 \times 10^{-6}$ — correct sign, within a factor of ~4 of the observed $10^{-5}$.

**Open step:** the ~30% ISW potential-decay factor used is a placeholder. A proper derivation requires the time-integral of $d\Phi/d\tau$ over the void's evolution history using the full $a(t)$ dependence already present in $\delta_w(a)$ and $\sigma_{wall}(a)$.

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
