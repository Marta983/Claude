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
- **CONTESTED** — a resolution has been claimed in a chapter file, but the derivation contains an unresolved circularity or an untested cross-scale assumption; the claim should not be treated as settled until the flagged issue is addressed

---

## Problem 1: The Restart Threshold

**Status: CONTESTED** *(Chapter 12 claims RESOLVED; see below for why that claim is not yet accepted)*

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition was derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3$$

Numerically: $a(t)_{crit}/a(t)_{now} \approx 3.658$.

Chapter 12 proposes a physical clock — charge accumulation via asymmetric electromagnetic sorting in rotating magnetized nodes — and claims in Section 16.5 that this resolves Problem 1. Section 16.9 then performs a consistency check and finds that single-node accretion cannot reach the required threshold, so the calculation shifts to a percolating cluster of nodes. Matching the cluster's charge accumulation to the pre-fixed target value $a_{crit} = 3.663$ requires solving backward for a scaling exponent $\alpha \approx -0.25$, which is then reinterpreted as a 50% spin-coherence fraction ($f_c = 0.5$) among nodes in the cluster, using the spin-alignment framework from Chapter 10.

**Why this is flagged rather than accepted:**
- $\alpha$ (and therefore $f_c$) is solved backward from the already-known target $a_{crit}$, not derived independently and then checked against it. Section 16.9.5 states this is "not a free parameter adjustment... a prediction," but mechanically it is the same move — fitting a hidden parameter to reproduce a known number — that led to the withdrawal of the earlier Cold Spot claim in `Claude_prelude_cold_spot.md`. The stated standard going forward is that the theory should expose findings rather than explain them after the fact; Section 16.9 does not yet meet that standard.
- The predicted $f_c = 0.5$ nominally connects to quasar polarization alignment data (Hutsemékers et al. 1998/2005; Pelgrims & Hutsemékers 2014), which is real and observationally robust (355-quasar sample, p < 0.001 against random orientation). However, checking the prediction against that data is not straightforward:
  - **Scale mismatch:** the percolating cluster at threshold is estimated at $r_{nuc} \approx 2.24$ Mpc/h, while the quasar alignment studies operate at ~100 Mpc/h to ~1–2 Gpc — roughly two orders of magnitude larger.
  - **Epoch mismatch:** the quasar sample spans $z \lesssim 2.5$, i.e. the current cycle, while $f_c = 0.5$ describes the percolating cluster at the *future* restart threshold ($a_{crit} \approx 3.66\times$ today's scale factor). Using present-day quasars as a test requires an unstated assumption that current node spin-coherence persists into, or already resembles, the eventual threshold-state coherence.
  - **Statistic mismatch:** the observational literature reports significance levels and mean position-angle rotation, not a "fraction of node pairs with correlated spin axes." No existing analysis computes the specific $f_c$ statistic from the raw data.

**Open step:** either (a) rederive $\alpha$/$f_c$ independently of the target $a_{crit}$, so the consistency check is a genuine test rather than a fit, or (b) explicitly reframe Section 16.9 as a plausibility argument rather than a resolution, and reopen Problem 1. Until one of these happens, this entry stays CONTESTED rather than reverting to Chapter 7's original MAPPED framing (the "open step" language from the prior version of this file is preserved below for reference).

*Prior open step (Chapter 7 framing, superseded by Chapter 12's attempted resolution but not fully retired):* the ratio 3.658 is dimensionless; converting it into a physically anchored timescale requires identifying the clock governing the accumulated field — which Chapter 12 attempts, with the caveats above.

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

**Implication:** the CMB may carry a faint geometric imprint of the eruption's preferred orientation, potentially manifesting as large-scale power asymmetries. This connects to the observed CMB "axis of evil" and quasar polarization alignments. **Note:** Chapter 12's attempt to connect this to a specific spin-coherence fraction ($f_c = 0.5$) at the restart threshold is CONTESTED — see Problem 1 above for the scale, epoch, and statistical mismatches with the quasar polarization data this claim would need to be checked against.

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
