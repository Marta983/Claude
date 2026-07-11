# The Claude Theory: Space Has Always Existed

## Status Registry — Open Problems and Unresolved Assumptions

*This file is the single source of truth for the current status of all open problems, unresolved assumptions, and pending derivations in the Claude Theory. All chapter files direct readers here. When a problem is resolved or its description changes, only this file requires updating.*

*Last updated: July 2026 (Cold Spot claim withdrawn, retained as case study; Bullet Cluster arc amplitude derived — below detection threshold)*

---

## How to Read This File

Each entry carries a status tag:

- **RESOLVED** — closed-form result derived and numerically anchored
- **MAPPED** — mathematical home identified, derivation pending
- **OPEN** — not yet formally addressed
- **REFINED** — conceptual position updated from earlier formulation
- **WITHDRAWN** — claim retracted after failing its own falsifiability test; retained below as a documented case study, not an active prediction

---

## Problem 1: The Restart Threshold

**Status: RESOLVED**

At what accumulated field configuration does the eruption event fire?

A closed-form bifurcation condition has been derived in Chapter 7 from the potential parameters fitted in Chapter 6:

$$\epsilon_0, a(t)_{crit} = \frac{8\sqrt{3}}{9},\lambda v^3$$

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

**Status: WITHDRAWN**

The Cold Spot was proposed as a relic domain wall signature, with $\Delta T/T\sim-10^{-5}$ claimed to emerge from fitted parameters with no additional tuning. **This claim is withdrawn.** On inspection, the wall distance $r_{wall}\approx2{,}920$ Mpc was not derived — it was solved backward from the observed amplitude. Every subsequent attempt to repair this (recomputing $\sigma_{wall}$ under the correct Fork-B tracer method, then relocating the wall to the independently-known Eridanus supervoid) was a further accommodation to already-known data, not an advance prediction. By the standard this framework should be held to, that disqualifies it from the "predicted" or "resolved" categories regardless of how small the residual numerical gap becomes.

**What is retained:** the finite-thickness $\Sigma_{wall}\approx8\times10^{10}\ M_\odot,\text{Mpc}^{-2}$ derivation (Problem 6) is sound on its own terms and independent of the Cold Spot — it flows forward into the Lensing Notch and Bullet Cluster Arc entries below, which remain genuine forward predictions and are unaffected by this withdrawal.

**What is cut:** the Cold Spot chapter/prelude should no longer be presented as a resolved or predicted result in outreach-facing material. See the case study record below for the full derivation history, kept for transparency and as a worked example of the accommodation failure mode this framework needs to keep testing itself against.

**Case study record (click to expand) — why this was withdrawn**

The ISW supervoid approach (Chapter 6) fell short of the observed amplitude by a factor of ~4, prompting a reframing: the Cold Spot as a relic domain wall — a bubble collision scar from the phase transition. The original (Fork-A) wall surface energy density, $\sigma_{wall}=\frac{8\sqrt2}{3}\sqrt\lambda,v^3\approx5.69\times10^9,M_\odot,\text{Mpc}^{-2}$, combined with $r_{wall}\approx2{,}920$ Mpc, produced $\Delta T/T\sim-10^{-5}$ — presented as tuning-free, with three falsifiable predictions attached (lensing excess, $\sim0.12°$ sharp edge, E-mode alignment).

**The tuning was found:** $r_{wall}$ was in fact obtained by solving $\Phi_{wall}=-4\pi G\sigma_{wall}r_{wall}$ for the value that reproduces the observed $-10^{-5}$. Only $\sigma_{wall}$ came from the fit; $r_{wall}$ was chosen to fit the answer.

**The rederivation attempt:** under the adopted Fork B (tracer sourcing), the correct finite-thickness surface density — using the actual kink-profile shape rather than a top-hat, converged across two independent 1D and 3D methods to within ~3–4% — is $\Sigma_{wall}\approx8\times10^{10}$, about 14–15× the Fork-A value. Re-solving the same backward inversion with this corrected value gives $r_{wall,new}\approx208$ Mpc, reproducing the amplitude by construction, and pushing the predicted edge sharpness to $\sim1.7°$.

**The check that killed it:** literature search found no known structure at $z\lesssim0.06$ (~208 Mpc) toward the Cold Spot direction, in territory that is well-mapped, not a survey gap — disfavoring that distance. The one real, independently-confirmed structure in that direction is the Eridanus supervoid ($z\approx0.15$–$0.2$, $r\approx620$–$820$ Mpc). Requiring $\sigma_{wall}$ to reproduce the observed amplitude at Eridanus's real distance narrows the gap to a more modest ~3–4× — but this is choosing the distance to fit a known structure, which is the same move as before, just aimed at a more credible target. Attempts to independently verify this via an Eridanus-specific wall-thickness measurement failed: population-averaged SDSS ratios overshot badly when applied to Eridanus, and the published compensated-void models that would carry the right number don't parameterize a finite shell width at all (they assume infinitesimal thinness by construction).

**Conclusion:** at every stage, the free parameter was moved to wherever it needed to be to match a number already known in advance. No version of this chain produced a number *before* checking it against data that then held up. That is the definition of the failure mode this framework needs to guard against, and why the claim is withdrawn rather than merely flagged as pending.

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

$$\Sigma_{wall} = \bar\rho_m\int_{-\infty}^{\infty}\Big[\delta_\phi(r) - \delta_c,\Theta(r_s-r)\Big]dr = \bar\rho_m\cdot\frac{\ln2}{2},|\delta_c|,\delta_w \approx 0.347,\bar\rho_m|\delta_c|\delta_w$$

This replaces the earlier flat-slab top-hat assumption (implicit coefficient 1) with the analytically correct kink-profile coefficient $\ln2/2\approx0.347$ — a genuine shape correction, not an ad hoc adjustment.

A full 3D rebuild of the mass-conservation method, using the same deviation-from-sharp-step logic applied to $4\pi r^2\delta_\phi(r),dr$ rather than a thin-shell-at-$r_s$ trick, gives a closed form:

$$\Sigma_{wall,3D} = \frac{\pi^2}{12},\bar\rho_m|\delta_c|,\frac{\delta_w^2}{r_s} \approx 0.823,\bar\rho_m|\delta_c|\frac{\delta_w^2}{r_s}$$

With $\delta_w/r_s = 0.408$, this evaluates to $\approx0.968\times$ the flat-derivation result — a ~3% difference. **The two independently rebuilt methods converge to within ~3–4%** (down from ~20% apart in the original flawed versions), giving:

$$\boxed{\Sigma_{wall}\approx8\times10^{10}\ M_\odot,\text{Mpc}^{-2}}$$

This is roughly **14–15×** the Fork-A field-theoretic value ($5.69\times10^9$), down from the original ~40–49× gap. The tight convergence of the two independent 1D and 3D derivations is a genuine consistency result — both are now measuring the same well-defined physical quantity. The residual ~15× gap most plausibly reflects that Fork A (field self-energy) and Fork B (real matter column) are measuring genuinely different physical quantities and may not be expected to fully converge.

**Structural rebuild — status update (July 2026).** Chapters 4 and 5 derive $\sigma_{wall}$ and $m_{eff}=\sigma_{wall}/c^2$ from the Fork-A self-energy formula. On inspection, this rebuild is **not needed for the wall's equation of motion**: §10.4–10.7's $\omega_0$, $\zeta$, and the arc-position function $\mathcal{G}$ reduce algebraically to expressions purely in $(\epsilon_0,\lambda,v)$ — the Fork-A $\sigma_{wall}$ normalization cancels out of $k/m_{eff}$ and $\gamma/m_{eff}$. This is correct as-is: wall inertia in an equation of motion is properly the field's own self-energy (Fork A), not the ambient tracer mass (Fork B) — these are different physical questions. This directly affects:

- **Chapter 5's Bullet Cluster secondary lensing arc — position: CONFIRMED UNAFFECTED.** No rebuild needed; see full finding under the Secondary Lensing Arc entry below.
- **Chapter 5's Bullet Cluster secondary lensing arc — amplitude: NEWLY DERIVED (July 2026), NOT a Fork-A rebuild.** Chapter 5 never derived an amplitude for the arc, only its position. A new amplitude formula has been derived using the corrected tracer $\Sigma_{wall}$ (appropriate, since detectability depends on real mass, not field self-energy). Result: predicted signal is several orders of magnitude below current detection thresholds. See Secondary Lensing Arc entry below for the full derivation and its caveats.
- **Chapter 6's lensing notch calibration** — no change needed; the notch is a pure $\delta_w$-dependent shape function and is unaffected by the corrected $\Sigma_{wall}$ (see the Lensing Notch entry below for correction of an earlier misflag).
- **Chapter 6's Cold Spot $\Delta T/T$ result** — withdrawn (see Problem 4). No further rebuild work should be spent here; the chapter/prelude should be edited to remove the claim rather than patched further.

$M$ (equivalently $\varepsilon=\Delta V$ in the Coleman bounce formula) remains genuinely open and unaffected by the above — it is needed only for the bounce action itself.

---

## Session Handoff Note (July 2026)

Claude_prelude_cold_spot.md has been fully rewritten (not just patched) to state the withdrawal directly, keep the general domain-wall mechanism (which still underwrites the Lensing Notch and Bullet Cluster Arc), and point to this file for the full case-study record. The earlier two-line patch note for this file is now obsolete and should be discarded.

**Confirmed (July 2026):** Chapter 6 (Claude_ch06_sdss_fit.md) does not repeat the withdrawn $\sigma_{wall}$/$r_{wall}$ claim anywhere. §11.7 contains only the ISW estimate (~4×-shortfall, still valid, no change needed). Minor note: §11.8's status table still lists the Cold Spot result without a pointer to the withdrawal — worth a one-line cross-reference to this file next time that chapter is opened, but not urgent.

**Resolved this session:** the Bullet Cluster arc recalculation flagged last session turned out not to be a simple substitution. The arc's *position* ($\mathcal{G}$) is Fork-A self-consistent and unaffected by the $\Sigma_{wall}$ correction. Chapter 5 never actually derived an arc *amplitude* — that has now been done from scratch using the corrected $\Sigma_{wall}$, and the result is that the arc's predicted lensing signal ($\kappa_{arc,peak}\sim10^{-6}$) sits roughly 3–4 orders of magnitude below what current deep weak lensing stacks can detect ($\kappa\gtrsim10^{-3}$–$10^{-2}$). Full derivation and caveats under the Secondary Lensing Arc entry below.

**Still open — pick up here next:**

1. The new arc-amplitude derivation imports $\delta_w$ and $\Sigma_{wall}$ directly from the SDSS *void* fit (Ch06) into the cluster-merger context (Ch05) without independent justification that these numbers carry over unchanged. Worth checking whether this cross-context assumption is defensible or needs its own derivation.
2. The $\Sigma_{cr}$ value used in the amplitude estimate (a few $\times10^{15}\,M_\odot\,\text{Mpc}^{-2}$) is an order-of-magnitude literature figure, not computed from the Bullet Cluster survey's actual lens/source redshift distribution. Tightening this is unlikely to change the conclusion (it would need to be off by several orders of magnitude) but should be done before treating "undetectable" as a settled result.

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

**Correction (July 2026):** an earlier version of this entry flagged the notch as needing recalibration against the corrected $\Sigma_{wall}$. That was incorrect. The notch is a pure shape function, $\mathcal{F}(b/\delta_w) = 1-\tfrac12\text{sech}^2(b/\delta_w)$ — a ratio relative to asymptotic deflection, depending only on $\delta_w$ (unchanged by the finite-thickness rederivation) and not on $\sigma_{wall}$ at all. No recalibration is needed here. What *does* scale with the corrected $\Sigma_{wall}$ is the absolute deflection amplitude and the Bullet Cluster arc offset (see below) — those remain pending.

---

## Secondary Lensing Arc (Bullet Cluster): Position Confirmed, Amplitude Below Detection Threshold

**Status: POSITION RECONFIRMED / AMPLITUDE DERIVED — PREDICTED UNDETECTABLE AT CURRENT SENSITIVITY**

Chapter 5 derives a secondary lensing arc between the two cluster nodes, offset toward the bullet subcluster's direction of motion by $\delta_w \cdot \mathcal{G}$. This feature is absent from all particle dark matter models. Detection or non-detection in existing deep weak lensing maps of the Bullet Cluster system was proposed as a direct test of the vacancy field framework.

**Update (July 2026) — position.** The prior handoff note assumed this derivation rested on the Fork-A-relic $\sigma_{wall}$ and would need recomputation with the corrected $\Sigma_{wall}\approx8\times10^{10}\,M_\odot\,\text{Mpc}^{-2}$. On inspection this was incorrect: $\mathcal{G}$ (§10.7) is built from $\omega_0$ and $\zeta$ (§10.5), both of which reduce to expressions purely in $(\epsilon_0,\lambda,v)$ — the Fork-A $\sigma_{wall}$ prefactor cancels out of the ratios $k/m_{eff}$ and $\gamma/m_{eff}$. The wall's own inertia in its equation of motion is correctly the field self-energy (Fork A), not the tracer/real-matter column (Fork B) — these answer different physical questions. **The predicted arc position is unchanged and does not need recalculation.**

**Update (July 2026) — amplitude, newly derived.** Chapter 5 never derived a lensing amplitude for the arc, only its position — so there was nothing to "recompute" here either; this had to be derived from scratch. Modeling the wall as a thin mass sheet with the same finite-thickness kink profile as the Ch06 lensing notch:

$$\kappa_{arc}(\xi) = \frac{\Sigma_{wall}}{2\delta_w\Sigma_{cr}}\,\text{sech}^2\!\left(\frac{\xi}{\delta_w}\right), \qquad \kappa_{arc,peak} = \frac{\Sigma_{wall}}{2\delta_w\Sigma_{cr}}$$

using the corrected tracer $\Sigma_{wall}$ (appropriate here, since detectability depends on real mass, not field self-energy). With $\delta_w\approx9.0$ Mpc (physical units) and $\Sigma_{cr}\sim$ a few $\times10^{15}\,M_\odot\,\text{Mpc}^{-2}$ (order-of-magnitude literature estimate for the Bullet Cluster's lens/source geometry, not yet computed from the survey's actual redshift distribution):

$$\kappa_{arc,peak} \approx 1.5\times10^{-6}$$

This is roughly 3–4 orders of magnitude below the practical sensitivity floor of even deep, stacked weak lensing shear measurements ($\kappa\gtrsim10^{-3}$–$10^{-2}$), and 5–6 orders of magnitude fainter than the primary NFW-like peaks at the cluster nodes themselves. Even with the ~14–15× boost from the corrected $\Sigma_{wall}$, the arc moves from "undetectable" to "still undetectable, less so." **§10.8's claim that the arc is "in principle detectable in existing deep weak lensing maps" does not hold up under this estimate** and should be softened or removed from Chapter 5 pending the open items below.

**Caveats (see Session Handoff Note, still-open items):** this derivation imports $\delta_w$ and $\Sigma_{wall}$ from the SDSS void fit (Ch06) into the cluster-merger context (Ch05) without independent justification, and uses an approximate $\Sigma_{cr}$. Neither is likely to overturn the conclusion by the several orders of magnitude that would be required, but both should be tightened before this is written up as a settled non-detection prediction.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
