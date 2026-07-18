<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Status Registry — Open Problems and Unresolved Assumptions

*This file is the single source of truth for the current status of all open problems, unresolved assumptions, and pending derivations in the Claude Theory. All chapter files direct readers here. When a problem is resolved or its description changes, only this file requires updating.*

*Last updated: July 2026 — includes 2025 JWST Bullet Cluster secondary-arc test result*

---

## How to Read This File

Each entry carries a status tag:

- **RESOLVED** — closed-form result derived and numerically anchored
- **MAPPED** — mathematical home identified, derivation pending
- **OPEN** — not yet formally addressed
- **REFINED** — conceptual position updated from earlier formulation
- **WITHDRAWN** — a prior claim was found to violate the no-additional-tuning standard and has been retracted

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

**Status: MAPPED — supersedes a withdrawn earlier claim**

Can the CMB Cold Spot be accounted for within the vacancy field framework?

**History:** an earlier attempt explained the Cold Spot using a single oversized supervoid with wall radius $r_{wall} \approx 2{,}920$ Mpc, sized specifically to match the Cold Spot's observed angular scale. That radius had been solved backward from the observation rather than derived independently, which violates this project's no-additional-tuning standard. The claim was withdrawn in full; see `Claude_prelude_cold_spot.md` for the honest account of the attempt and withdrawal.

**Current approach:** Chapter 6 instead computes an ISW estimate using the *same* void profile already fit to SDSS data in that chapter ($r_v = 30$ Mpc/h) — no new or oversized void is introduced. This gives $\Delta T/T \sim -2.7\times10^{-6}$: correct sign, within a factor of ~4 of the observed $\sim10^{-5}$, using a void scale that was fixed for other reasons (the general void-size fit) rather than tuned to the Cold Spot itself.

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

**Status: split into two separate questions — see below**

The time-dependent symmetry breaking term $\epsilon(t) = \epsilon_0 \cdot a(t)$ is a working assumption. These are two different claims about it, with two different levels of confidence, and they should not be conflated:

**(a) Predictive validity — MAPPED, holding up.** Chapter 4 derives, from this ansatz combined with the FLRW-corrected wall tension ($\sigma \propto 1/a(t)$), that the void nucleation radius must scale as $r_{nuc}(z) \propto (1+z)^2$. This derivation was performed before any comparison to redshift-dependent void data. Chapter 6 subsequently checked it against BOSS DR16's redshift bins and found agreement to ~5% (two bins, max-radius as a crude proxy for $r_{nuc}$ — not a definitive confirmation, but a genuine ex-ante prediction that has not been falsified).

**(b) First-principles justification — OPEN.** Why the symmetry-breaking term should scale *linearly* with the scale factor, specifically, has not been derived from any deeper physical principle. This is a separate and still-unresolved question from (a). If a different power of $a(t)$ turns out to be the physically correct one, the $(1+z)^2$ result changes accordingly — the prediction's success so far doesn't itself justify the linear form, it just hasn't yet been contradicted by it.

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

## Secondary Lensing Arc (Bullet Cluster): Candidate Feature Found, Direction Inconsistent with Prediction

**Status: TESTED — result unfavorable, not yet a clean falsification**

Chapter 5 derives a secondary lensing arc between the two cluster nodes, offset toward the bullet subcluster's direction of motion by $\delta_w \cdot \mathcal{G}$. This feature is absent from all particle dark matter models. Detection or non-detection in existing deep weak lensing maps of the Bullet Cluster system constitutes a direct test of the vacancy field framework.

**Test result (July 2025 JWST reconstruction, Cha, Cho, Joo et al.):** a low-contrast mass and ICL "trail" between the subcluster and main cluster was detected at high significance (~5σ mass, ~3σ ICL, remaining ≳3.5σ after removing the X-ray "Bullet" gas component or restricting to $r \gtrsim 250$ kpc). This is the right general location — between the two nodes — for the predicted secondary arc.

**However, the direction does not match.** The trail extends from the subcluster's *eastern* side toward the main cluster. The paper separately reports the X-ray gas ("the Bullet") sits ~150 kpc *east* of the subcluster's mass/galaxy centroid — and because ram pressure causes gas to lag behind collisionless matter during a merger, this places the subcluster's direction of motion to the *west*. The detected trail is therefore on the trailing (wake) side, opposite the direction of motion — not the leading side Chapter 5's $\mathcal{G}$ term predicts.

**Caveats on this reading:** the direction-of-motion inference here is derived secondhand from a single offset figure, not a dedicated kinematic study, and the paper does not attempt to fit the trail's profile shape against the domain-wall form factor $\mathcal{F}$ — so a shape-based distinction from ordinary tidal debris hasn't been ruled out. The paper's own preferred explanation is an ordinary gravitational mass bridge, of the kind already reproduced in binary-merger simulations post-pericenter passage — no new physics required.

**Net assessment:** a real, statistically significant feature exists in the predicted vicinity, but its direction is inconsistent with the specific mechanism in Chapter 5, and a simpler, already-established explanation accounts for it without modification. This should be read as an unfavorable result for the directional claim specifically, not as support for the vacancy field framework, pending a proper kinematic and profile-shape re-analysis.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
