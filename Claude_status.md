<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Status Registry — Open Problems and Unresolved Assumptions

*This file is the single source of truth for the current status of all open problems, unresolved assumptions, and pending derivations in the Claude Theory. All chapter files direct readers here. When a problem is resolved or its description changes, only this file requires updating.*

*Last updated: July 2026 (finite-thickness shell rederivation)*

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

**Status: PREDICTED, PENDING $\Delta T/T$ RECOMPUTATION**

Can the CMB Cold Spot be accounted for within the vacancy field framework?

The ISW supervoid approach (Chapter 6) fell short by a factor of ~4. The mechanism was reframed: the Cold Spot is not a supervoid signature but a relic domain wall — a bubble collision scar from the phase transition itself, frozen into the field configuration of space. The original (Fork-A) wall surface energy density, derived from fitted parameters $(\lambda, v)$ via the canonical field self-energy formula:

$$\sigma_{wall} = \frac{8\sqrt{2}}{3}\sqrt{\lambda}\,v^3 \approx 5.69 \times 10^{9}\, M_\odot\,\text{Mpc}^{-2}$$

produced $\Delta T/T \sim -10^{-5}$ at $r_{wall} \approx 2{,}920$ Mpc with no additional tuning. Three falsifiable predictions were built on this: (1) lensing convergence *excess* rather than deficit at the boundary; (2) a sharp angular edge at $\sim0.12°$; (3) tangential E-mode polarization alignment at the boundary. See Claude_prelude_cold_spot.md.

**Update (July 2026) — finite-thickness shell rederivation complete.** This formula used the Fork-A self-energy form, which we've since determined is not the physically appropriate quantity under the adopted Fork B (tracer) sourcing. The rederivation under Fork B — see Problem 6 below — gives a converged value of $\Sigma_{wall}\approx8\times10^{10}\,M_\odot\,\text{Mpc}^{-2}$, roughly **14–15×** the Fork-A value used above.

**New flag — possible $\Delta T/T$ overshoot.** If $\Delta T/T$ scales close to linearly with $\Sigma_{wall}$, as is typical for thin-wall ISW/Rees-Sciama-type estimates, the corrected surface density would push the predicted signal to roughly $-1.4\times10^{-4}$ — about an order of magnitude *larger* than the observed Cold Spot amplitude ($\sim-10^{-5}$). This is a more serious problem than the earlier magnitude gap: rather than an unexplained excess in a derived parameter, it risks an outright overshoot of the observational target the whole mechanism was built to match. The linearity assumption itself has not yet been checked against the actual ISW/Rees-Sciama formula used in Chapter 6 — this is the immediate next step, ahead of touching Chapter 5's Bullet Cluster arc. **All three falsifiable predictions above, and the $\Delta T/T$ headline result, should be treated as unconfirmed pending this recomputation.**

---

## Problem 5: The JWST Anomalous Mass Function

**Status: OPEN**

JWST observations show galaxies with unexpectedly evolved properties at high redshift, inconsistent with the timeline of our event under standard cosmology. The Claude Theory reframes these as inherited material from previous or neighboring eruption events. Formal quantitative treatment not yet undertaken. Prerequisite: Problem 3 (casting mechanics).

---

## Problem 6: The Missing Mass Scale M and the φ Interpretation Forks

**Status: RESOLVED (forks) / RESOLVED (finite-thickness surface density) / OPEN (bounce-action mass scale, Chapters 4–5 rebuild)**

Chapter 6's SDSS fit conflated the dimensionless density-contrast amplitude $\delta_c$ with the field's vacuum expectation value $v$. Fitted parameters $(\epsilon_0, \lambda, v)$ therefore cannot be used directly for energy-normalized quantities such as the Coleman bounce action, since no mass scale $M$ was present in the fit.

**Fork A — φ quantum or classical: RESOLVED, classical.** φ is treated as a classical effective field throughout. Quantum treatment is reserved for the bubble nucleation event itself (Coleman-De Luccia tunneling), not for φ's background dynamics.

**Fork B — φ sources gravity or traces density contrast: RESOLVED, tracer.** φ is dimensionless by construction, $\phi \propto \delta_c = (\rho - \bar\rho)/\bar\rho$. Gravity is sourced conventionally by $\rho$ through the Einstein field equations; φ never enters as a stress-energy source.

**Narrowed:** the missing mass scale $M$ is *not* needed for the domain wall's gravitational or lensing effects — only for the Coleman bounce action itself, since bubble nucleation concerns the field's actual dynamics during the phase transition, not its settled tracer profile after the fact.

**Finite-thickness shell rederivation (RESOLVED, July 2026).** Chapter 6's void profile is $\delta_\phi(r) = \delta_c\cdot\tfrac12(1-\tanh((r-r_s)/\delta_w))$, with $\delta_c=-0.6537$, $r_s=15.45$ Mpc/h, $\delta_w=6.31$ Mpc/h — a monotonic step, not a symmetric bump. The wall is the transition edge of the void itself. The correct finite-thickness surface density is defined as the mass redistributed by the smooth tanh edge relative to an idealized sharp-edged void of the same $\delta_c$ and same boundary $r_s$:

$$\Sigma_{wall} = \bar\rho_m\int_{-\infty}^{\infty}\Big[\delta_\phi(r) - \delta_c\,\Theta(r_s-r)\Big]dr = \bar\rho_m\cdot\frac{\ln2}{2}\,|\delta_c|\,\delta_w \approx 0.347\,\bar\rho_m|\delta_c|\delta_w$$

This replaces the earlier flat-slab top-hat assumption (implicit coefficient 1) with the analytically correct kink-profile coefficient $\ln2/2\approx0.347$ — a genuine shape correction, not an ad hoc adjustment.

A full 3D rebuild of the mass-conservation method, using the same deviation-from-sharp-step logic applied to $4\pi r^2\delta_\phi(r)\,dr$ rather than a thin-shell-at-$r_s$ trick, gives a closed form:

$$\Sigma_{wall,3D} = \frac{\pi^2}{12}\,\bar\rho_m|\delta_c|\,\frac{\delta_w^2}{r_s} \approx 0.823\,\bar\rho_m|\delta_c|\frac{\delta_w^2}{r_s}$$

With $\delta_w/r_s = 0.408$, this evaluates to $\approx0.968\times$ the flat-derivation result — a ~3% difference. **The two independently rebuilt methods converge to within ~3–4%** (down from ~20% apart in the original flawed versions), giving:

$$\boxed{\Sigma_{wall}\approx8\times10^{10}\ M_\odot\,\text{Mpc}^{-2}}$$

This is roughly **14–15×** the Fork-A field-theoretic value ($5.69\times10^9$), down from the original ~40–49× gap. The tight convergence of the two independent 1D and 3D derivations is a genuine consistency result — both are now measuring the same well-defined physical quantity. The residual ~15× gap most plausibly reflects that Fork A (field self-energy) and Fork B (real matter column) are measuring genuinely different physical quantities and may not be expected to fully converge.

**Structural rebuild required — OPEN.** Chapters 4 and 5 derive $\sigma_{wall}$ and $m_{eff}=\sigma_{wall}/c^2$ from the Fork-A self-energy formula and need to be rebuilt on the $\Sigma_{wall}\approx8\times10^{10}$ result above. This directly affects:
- **Chapter 5's Bullet Cluster secondary lensing arc** — the offset prediction $\delta_w\cdot\mathcal{G}$ used the old $\sigma_{wall}$; the ~14× larger surface density likely changes the predicted arc amplitude materially, and its detectability against existing deep lensing maps needs rechecking.
- **Chapter 6's lensing notch calibration** — needs the corrected $\Sigma_{wall}$ substituted in.
- **Chapter 6's Cold Spot $\Delta T/T$ result** — see the overshoot flag under Problem 4. This is the most urgent of the three, since it risks invalidating the headline result rather than just shifting a derived number.

$M$ (equivalently $\varepsilon=\Delta V$ in the Coleman bounce formula) remains genuinely open and unaffected by the above — it is needed only for the bounce action itself.

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

**Status: CALIBRATED, PENDING RECALIBRATION**

Chapter 6 predicts a lensing convergence notch — deflection suppressed to 50% of asymptotic value at domain wall centers, recovering to >95% by $b \approx 12.6$ Mpc/h. This non-monotonic feature is absent from all particle dark matter models and constitutes a direct observational test. Not yet compared against actual weak lensing stacks.

**Update (July 2026):** this calibration rests on the Fork-A-relic $\sigma_{wall}$. The finite-thickness rederivation (Problem 6) gives $\Sigma_{wall}\approx8\times10^{10}\,M_\odot\,\text{Mpc}^{-2}$, ~14–15× larger. Recalibration with the corrected value is pending.

---

## Secondary Lensing Arc (Bullet Cluster): Predicted, Undetected

**Status: PREDICTED, PENDING RECALCULATION**

Chapter 5 derives a secondary lensing arc between the two cluster nodes, offset toward the bullet subcluster's direction of motion by $\delta_w \cdot \mathcal{G}$. This feature is absent from all particle dark matter models. Detection or non-detection in existing deep weak lensing maps of the Bullet Cluster system constitutes a direct test of the vacancy field framework.

**Update (July 2026):** this derivation rests on the Fork-A-relic $\sigma_{wall}$. With the corrected $\Sigma_{wall}\approx8\times10^{10}\,M_\odot\,\text{Mpc}^{-2}$ (~14–15× larger), the predicted arc amplitude needs recomputation before comparison against existing lensing maps.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
