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
- **CALIBRATED** — shape derived, amplitude/normalization requires an external physical input
- **WITHDRAWN** — previously claimed, found not to survive scrutiny, retracted rather than patched
- **CONTESTED** — external critique raised a specific, unresolved objection

---

## Problem 1: The Restart Threshold

**Status: CONTESTED**

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition has been derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3$$

Numerically: $a(t)_{crit}/a(t)_{now} \approx 3.658$.

**Open step:** the ratio 3.658 is dimensionless and its physical meaning is not yet established. Converting it into a timescale or physically meaningful accumulation quantity requires identifying what clock governs the accumulated field across the full cycle.

**External critique (Erickcek, UNC, July 2026):** the underlying mechanism here — like the framework generally — is stated through analogy rather than explicit field equations, so it isn't yet possible to check whether numerical fits (SDSS, Bullet Cluster, Cold Spot) follow from the framework or were fit to known answers. This entry stays CONTESTED until the technical chapters state the equations explicitly and derive (not assert) the numbers from them.

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

**Status: WITHDRAWN**

Chapter 6 previously computed an ISW estimate of $\Delta T/T \sim -2.7 \times 10^{-6}$ against this framework, using a ~30% ISW potential-decay factor. That factor was a placeholder chosen to land near the observed value rather than derived independently — solved backward from the answer rather than forward from the mechanism — and the claim has been withdrawn on that basis. A legitimate Cold Spot estimate would need the placeholder replaced with an actual time-integral of $d\Phi/d\tau$ over the void's evolution history, derived without reference to the target number.

**Separately:** any spectrum-level cosmological claim in this framework (this entry included, and the "latent heat of a phase transition" language elsewhere) has to clear a higher bar raised externally (Erickcek, UNC, July 2026): the CMB is a near-perfect blackbody at a precisely matched temperature, not merely uniform, and reproducing that exact spectrum from a real calculation is a substantially higher bar than a rough ISW estimate addresses.

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

## Vacancy Field Gravitational Role: Resolved (Tracer)

**Status: RESOLVED**

Does the vacancy field $\phi$ source gravity independently through its own stress-energy, or does it track the gravitating mass without adding to it?

Resolved in favor of the tracer picture: $\phi$ is dimensionless, and gravity is sourced conventionally by the actual matter density $\rho$, not by $T_{\mu\nu}^{(\phi)}$. $\phi$'s own field equation and kink/soliton solutions (Chapter 4, Section 7) still govern the *shape* of where structure concentrates — the void-nucleation-length result is unaffected — but $\phi$ no longer supplies an independent gravitating substance. Chapters 4 and 5 have been rebuilt accordingly (July 2026); see those chapters for the consequences below.

---

## Lensing Notch: Rebuilt Under Tracer Picture

**Status: CALIBRATED**

Chapter 4 (rebuilt) derives $\hat\alpha(b) = \frac{4\pi G\Sigma_{wall}}{c^2}\tanh(b/\delta_w)$ — deflection vanishing exactly at the wall center and rising monotonically to its asymptotic value, rather than the previously claimed 50%-notch recovering by $b\approx12.6$ Mpc/h. That earlier notch shape depended on the field's own potential energy density, which no longer sources gravity under the tracer resolution, and is superseded by this result. The sigmoid *shape* is a structural, low-parameter prediction; its *amplitude* now requires the externally-anchored $\Sigma_{wall}\approx8\times10^{10}\,M_\odot/\mathrm{Mpc}^2$ as input rather than deriving from $v,\lambda,\delta_w$ alone. Not yet compared against actual weak lensing stacks.

---

## Secondary Lensing Arc (Bullet Cluster): Withdrawn

**Status: WITHDRAWN**

Chapter 5 (rebuilt) shows that the damped-oscillator wall-dynamics mechanism this prediction depended on has no surviving basis under the tracer picture: the midpoint between two separating mass concentrations is an *unstable* saddle point under ordinary two-body Newtonian gravity, not a stable equilibrium with a restoring force. The specific secondary-arc trajectory this predicted cannot be recovered by adjusting constants — the underlying physics changed in kind. The Bullet Cluster gas/lensing offset itself still holds, but under the tracer picture it is observationally indistinguishable from the standard ΛCDM account and should not be presented as a distinguishing prediction of this framework.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
