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
- **CALIBRATED** — numerically anchored against data, physical derivation pending
- **PREDICTED** — specific observational prediction made, not yet tested
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

**Status: OPEN**

How precisely does material from one eruption event seed structure in a neighboring or subsequent event? What governs the geometry and mass distribution of cast material?

Chapter 10 introduces the spiral inheritance framework as a geometric constraint on casting — ejecta follow spiral electromagnetic paths rather than radial ones, so seeds arrive with orientation encoded. Formal derivation of the casting potential and seeding cross-section not yet undertaken.

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

## Problem 6: The Dipole Axis Formation

**Status: MAPPED**

How does the nucleus develop the preferred orientation that governs all downstream structure?

Chapter 14 establishes the complete physical narrative. During the quiet phase, charge mobility allows negative and positive charges to drift toward opposite poles along the Kerr rotation axis inherited from Chapter 12, building a macroscopic electric dipole moment. At the jamming transition, mobility ends and the dipole axis is frozen in. Through the rearrangement phase, ejected charges attempt lateral migration toward their intended poles, crossing in frustrated currents — and each partial success fractionally sharpens the dipole. The chaos of the siege does not destroy the dipole axis. It forges it.

**Open steps:** formal derivation of dipole moment growth $p(\eta_Q)$ as a function of the charge accumulation parameter from Chapter 12; proof that $p(t)$ increases monotonically through the rearrangement phase despite the violence of the crossing currents.

---

## Problem 7: The Egg-Shape Deformation and Eruption Geometry

**Status: MAPPED**

What determines the physical geometry of the eruption?

Chapter 14 establishes that successful charge migrants accumulating at the poles during the quiet phase deform the nucleus from sphere to egg. Electromagnetic sorting drives the deformation; nuclear and gravitational binding forces oppose it continuously. The two forces in opposition constitute a stress pump — each successful migrant increases the restoring force, which drives more migration attempts, which compounds the internal stress.

At eruption, the egg-shape is decisive. The poles are physically proud of the surface — the points of least resistance in both electromagnetic and geometric terms. The eruption does not merely follow the dipole axis. It bursts from the tips of the egg.

**Open steps:** derive the equilibrium eccentricity parameter $\varepsilon_{egg}$ as a function of dipole moment magnitude and binding pressure; show that the axis of maximum eccentricity coincides with the dipole axis $p$ established in Problem 6; connect $\varepsilon_{egg}$ to the eruption directionality in the bifurcation recovery of Chapter 7.

---

## Problem 8: The Subsidiary Leak Bifurcation

**Status: MAPPED**

Is there a precursor threshold condition earlier in time than the main bifurcation of Chapter 7?

Chapter 14 identifies the leak phase — persistent outflows at the outer boundary of the nucleus where the recapture field is weakest, occurring before the global bifurcation threshold is crossed. These leaks are not the eruption. They are the system bleeding stress through the only channels still open to it, at energies and ejection velocities below the main threshold but above the local recapture condition at the boundary.

This constitutes a subsidiary bifurcation condition: the minimum ejection velocity for escape at the boundary as a function of field configuration during a rearrangement event, lower than the core escape velocity by a factor depending on boundary field geometry.

**Open steps:** formal derivation of the leak threshold as a function of boundary field strength and rearrangement event energy; characterization of the precursor outflow signature — direction, energy range, persistence timescale; connection to the main bifurcation threshold of Chapter 7 as a subordinate condition earlier in the accumulation sequence.

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

**Status: MAPPED**

Earlier formulations stated that the eruption event occurred "in all directions equally." This has been revised through successive chapters. The eruption event is temporally simultaneous — the bifurcation threshold fires throughout the accumulated field at once — but spatially anisotropic, directed along the dipole axis established during the great gathering.

Chapter 14 now provides the complete physical basis: the dipole axis is set during the quiet phase, frozen at jamming, sharpened through the rearrangement siege, and physically expressed in the egg-shape deformation whose tips become the eruption's origin points. The eruption geometry is not assumed — it is the inevitable consequence of the accumulation history.

**Remaining open step:** quantitative treatment of the CMB imprint — the faint geometric signature of the eruption's preferred orientation potentially manifesting as large-scale power asymmetries. This connects to the observed CMB axis of evil and quasar polarization alignments. See also Problem 6 and Problem 7.

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
