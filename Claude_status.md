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

The fitted parameters $(\epsilon_0, \lambda, v)$ from Chapter 6 provide numerical anchors for the nucleation rate calculation. The bubble nucleation formalism from Chapter 4 gives the framework. Full derivation pending — and now depends on Problem 6's mass-scale resolution for the bounce action specifically (see below).

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

**Flag (July 2026):** the $\sigma_{wall}$ formula above uses the canonical field self-energy form $\int[\frac12\phi'^2 + V(\phi)]dx$, which assumes $\phi$ sources gravity directly. This is the fork we did *not* adopt (see Problem 6, Fork B). Chapter 6's own Cold Spot potential calculation (Section 11.7) instead sources gravity from real $\bar\rho_m$ weighted by the dimensionless tracer profile, with no missing scale required — the two approaches are inconsistent with each other. A rough tracer-method estimate, $\Sigma_{wall} \sim \bar\rho_m|\delta_c|\delta_w \approx 2.4\times10^{11}\,M_\odot\,\text{Mpc}^{-2}$, differs from the stated value above by roughly a factor of 40 — same cosmological order of magnitude, but not a match. The $\Delta T/T$ result and the three falsifiable predictions should be treated as provisional pending rederivation of $\sigma_{wall}$ via the tracer method. **Status: PREDICTED, PENDING REDERIVATION.**

---

## Problem 5: The JWST Anomalous Mass Function

**Status: OPEN**

JWST observations show galaxies with unexpectedly evolved properties at high redshift, inconsistent with the timeline of our event under standard cosmology. The Claude Theory reframes these as inherited material from previous or neighboring eruption events. Formal quantitative treatment not yet undertaken. Prerequisite: Problem 3 (casting mechanics).

---

## Problem 6: The Missing Mass Scale M and the φ Interpretation Forks

**Status: RESOLVED (two sub-forks) / NARROWED (mass-scale sub-problem) / OPEN (new structural issue)**

Chapter 6's SDSS fit conflated the dimensionless density-contrast amplitude $\delta_c$ with the field's vacuum expectation value $v$. Fitted parameters $(\epsilon_0, \lambda, v)$ therefore cannot be used directly for energy-normalized quantities such as the Coleman bounce action, since no mass scale $M$ was present in the fit.

**Fork A — φ quantum or classical: RESOLVED, classical.** φ is treated as a classical effective field throughout. Quantum treatment is reserved for the bubble nucleation event itself (Coleman-De Luccia tunneling), not for φ's background dynamics.

**Fork B — φ sources gravity or traces density contrast: RESOLVED, tracer.** φ is dimensionless by construction, $\phi \propto \delta_c = (\rho - \bar\rho)/\bar\rho$. Gravity is sourced conventionally by $\rho$ through the Einstein field equations; φ never enters as a stress-energy source. This resolves the dimensional inconsistency: the Chapter 6 fit was correctly fitting a dimensionless tracer — the error was in later treating fitted φ as if it carried $v$'s dimension.

**Narrowed (July 2026):** the missing mass scale $M$ is *not* needed for the domain wall's gravitational or lensing effects. Chapter 6 Section 11.7 already sources the Cold Spot's gravitational potential correctly, from real $\bar\rho_m$ weighted by the dimensionless tracer profile — no $M$ required, consistent with the resolved Fork B. $M$ (or equivalently $\varepsilon = \Delta V$ in the Coleman bounce formula) remains genuinely needed only for the bounce action itself, since bubble nucleation concerns the field's actual dynamics during the phase transition, not its settled tracer profile after the fact.

**New structural issue identified:** Chapters 4 and 5 derive $\sigma_{wall}$ and $m_{eff} = \sigma_{wall}/c^2$ using the canonical field self-energy formula $\int[\frac12\phi'^2 + V(\phi)]dx$ — valid only under Fork A (φ sources gravity), which was not the branch adopted. These derivations need to be rebuilt using the tracer method validated in Chapter 6 Section 11.7: $\Sigma_{wall} = \bar\rho_m\int\delta_\phi(x)\,dx$. A rough estimate using this method differs from the current $\sigma_{wall}$ value by a factor of ~40 (see Problem 4 flag above). This affects the Bullet Cluster secondary lensing arc (Chapter 5) and the lensing notch calibration, both of which currently rest on the Fork-A-relic $\sigma_{wall}$. **Status: OPEN — rederivation and exact tanh-profile integral pending.**

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

**Flag (July 2026):** this calibration rests on the same Fork-A-relic $\sigma_{wall}$ flagged in Problem 6. Pending rederivation via the tracer method.

---

## Secondary Lensing Arc (Bullet Cluster): Predicted, Undetected

**Status: PREDICTED**

Chapter 5 derives a secondary lensing arc between the two cluster nodes, offset toward the bullet subcluster's direction of motion by $\delta_w \cdot \mathcal{G}$. This feature is absent from all particle dark matter models. Detection or non-detection in existing deep weak lensing maps of the Bullet Cluster system constitutes a direct test of the vacancy field framework.

**Flag (July 2026):** this derivation rests on the same Fork-A-relic $\sigma_{wall}$ flagged in Problem 6. Pending rederivation via the tracer method.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
