<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 5 — The Bullet Cluster (Rebuilt)

*Revision note: rebuilt under the Fork B tracer resolution (φ demoted to a tracer of density contrast; gravity sourced conventionally by ρ). This rebuild does not fully preserve the chapter's original claims — see Section 10.4 below, where the wall-dynamics mechanism is retracted rather than patched.*

---

## Section 10.1–10.3: Setup and the Primary Offset (Survives, but Reinterpreted)

The observational core of the Bullet Cluster is unchanged: the X-ray-emitting gas (collisional, electromagnetically coupled) lags behind the lensing mass peaks (collisionless) during the collision, producing the signature offset between the two.

Under the old picture, this was explained by $\phi$ — an independent field passing through the collision unimpeded, like the gas's collisionless counterpart, with its own gravitating stress-energy standing in for "dark matter." Under the tracer picture, this explanation **changes in kind, not just in derivation**: $\phi$ no longer supplies a new gravitating substance. It only labels where the actual collisionless mass (dark remnants, per the framework's own account of what constitutes that mass) already is. The lensing peak coincides with the collisionless mass because the collisionless mass is collisionless — full stop. $\phi$ is a bookkeeping device tracking that mass's location, not an explanation for why the offset exists.

**This needs to be stated plainly, not softened**: on this point, the tracer-picture Claude Theory is now observationally indistinguishable from the standard ΛCDM account of the Bullet Cluster. Both say "collisionless mass separates from collisional gas during the collision, hence the offset." The framework's distinctive claim was never really *that* the offset exists — every viable theory explains that — but *what* the collisionless mass is and how it got there (frozen vacuum domains / relic asymmetry rather than a new particle species). That deeper claim survives. The offset itself is not, on its own, evidence for one picture over the other.

---

## Section 10.4: Wall Dynamics and the Secondary Arc (Retracted)

This is the chapter's harder finding, and it should be stated as a finding rather than patched around.

**The old mechanism.** The original chapter modeled the re-forming domain wall (the density ridge that reappears between the two separating cluster cores after collision) as a damped harmonic oscillator, settling toward a new equilibrium position with restoring constant $k = 2\epsilon_0 a(t)v/\delta_w^2$ and effective mass $m_{eff} = \sigma_{wall}/c^2$ — both quantities coming from the field's *own* potential curvature and self-energy. That restoring force was legitimate in the old picture: it's the stiffness of the domain wall as a genuine physical membrane, trying to sit at its own potential minimum. It had nothing to do with two-body gravity between the cluster cores; it was intrinsic to the field.

**Why it doesn't survive.** Under the tracer picture, $\phi$ no longer has a gravitationally-relevant potential of its own — its dynamics govern *shape*, not *force*. So if the wall is going to have any restoring dynamics at all, that restoring force now has to come from somewhere physical: the actual gravity of the two cluster cores acting on the actual mass sitting between them.

Work this out directly. Model the two cores as point masses $M$ at $x=\pm D/2$, and ask about the net gravitational force on a test mass at position $X$ along the line joining them:

$$F(X) = GM\left[\frac{1}{(D/2-X)^2} - \frac{1}{(D/2+X)^2}\right]$$

$F(0)=0$ by symmetry — the midpoint is an equilibrium. But:

$$\left.\frac{dF}{dX}\right|_{X=0} = GM\left[\frac{2}{(D/2)^3}+\frac{2}{(D/2)^3}\right] = \frac{32GM}{D^3} > 0$$

A positive slope at a zero means the midpoint is an **unstable** equilibrium — this is the familiar tidal-saddle-point result for two point masses. A small displacement toward one core is amplified, not damped. There is no stable restoring force along the axis connecting two point masses under ordinary Newtonian gravity.

**This directly contradicts the requirement of the old model.** The damped-oscillator picture — and with it, the specific secondary-lensing-arc prediction that depended on the wall oscillating back through a predictable trajectory — has no surviving mechanism under strict tracer physics. It cannot simply be re-derived with new constants; the qualitative physics (stable restoring force) that the old derivation depended on is gone.

**What (if anything) replaces it.** The re-formation of a density ridge between two separating mass concentrations is a real phenomenon in a collisional system — but its physical origin, under the tracer picture, would have to be something like gravitational relaxation or dynamical friction acting on a free-fall/crossing timescale,

$$\tau_{dyn} \sim \frac{1}{\sqrt{G\bar\rho}}$$

rather than a harmonic restoring force with a definite oscillation period. That gives a rough *timescale* for the ridge to re-establish itself, but not a predictive trajectory, and not the specific secondary arc position the original chapter predicted. Deriving an actual predictive replacement would require proper collisional/N-body treatment (dynamical friction, gas drag, violent relaxation) — it is not a small patch on the existing derivation.

**Status: this sub-result is retracted, not rebuilt.** Following the same standard that led to withdrawing the Cold Spot claim: the honest move is to mark the secondary-arc prediction as OPEN / RETRACTED, not to force a substitute constant into the old damped-oscillator form. The flagship falsifiable claim that most sharply distinguished this framework from ΛCDM in the Bullet Cluster context does not currently survive the tracer resolution.

---

## κ(r) Under the Tracer Picture

Since the primary lensing profile now inherits directly from Chapter 4's rebuilt $\Sigma_{node}(r)$:

$$\kappa(r) = \frac{\Sigma_{node}(r)}{\Sigma_{cr}} = \frac{M_{node}}{2\pi r_{node}^2 \Sigma_{cr}}\cdot\frac{1}{1+(r/r_{node})^2}$$

with $M_{node}$, $r_{node}$ now external, independently-fit quantities per core (gas-stripped remnant on one side, less-stripped on the other), rather than parameters derived from $v,\lambda,\delta_w$. This reproduces the qualitative shape of the observed convergence maps (two offset peaks), but — consistent with the Section 10.1–10.3 finding above — does so in a way that is not distinguishable from a standard two-halo NFW fit. The distinguishing power the framework once claimed here has moved entirely into the *interpretation* of what $M_{node}$ physically is, not into the shape of $\kappa(r)$ itself.

---

## Updated Summary

| Claim | Status after tracer rebuild |
|---|---|
| Lensing/gas offset exists | Survives — but now observationally identical to ΛCDM's own account |
| $\kappa(r)$ two-peak structure | Survives in shape; normalization now external, same as any NFW fit |
| Wall restoring dynamics (damped oscillator) | **Retracted** — no stable mechanism under ordinary two-body gravity |
| Secondary arc prediction | **Retracted**, pending a genuine collisional/dynamical-friction derivation |

---
## A Living Document
The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.
---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
