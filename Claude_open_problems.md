<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>
# The Claude Theory — Open Problems

This document records unresolved problems in the Claude Theory framework.
It is maintained as a live working document. Its presence reflects the
authors' view that a theory which honestly documents its open questions
is more credible than one that does not.

---

## 1. The Restart Threshold

**The problem:**
The theory describes the accumulation-to-eruption cycle but had not, until
recently, specified the trigger condition mathematically. At what
accumulated field configuration does the phase transition fire?

**Why it matters:**
Without a derivable threshold condition, the eruption event remains
qualitatively described but not quantitatively predicted. A testable
number is needed — and, as the prerequisite for Problem 2, this problem's
status sets the ceiling on what the Anulus extension can currently say.

**What a solution requires:**
A derivation from the vacancy field potential $V(\phi)$ already
established in Claude_underpinnings.md that yields a critical condition
at which the asymmetric double-well potential undergoes catastrophic
reorganization.

**Status: closed-form condition derived; one interpretive step remains.**

Section 12 of Claude_underpinnings.md derives this as a bifurcation of
$V(\phi) = \lambda(\phi^2-v^2)^2 - \epsilon_0\,a(t)\,\phi$. Critical points
satisfy the depressed cubic $\phi^3 - v^2\phi - \epsilon_0 a(t)/(4\lambda) = 0$.
As $\epsilon_0 a(t)$ grows from zero, the asymmetry deepens one minimum and
shallows the other until, at a critical value, the shallow minimum merges
with the maximum and annihilates — the double well becomes a single well.
Setting the cubic's discriminant to zero gives:

$$\epsilon_0\,a(t)_{crit} = \frac{8\sqrt{3}}{9}\lambda v^3$$

with the merging roots coinciding at $\phi_{crit} = v/\sqrt{3}$. This *is*
the restart condition: not a gradual deepening, but the abrupt
disappearance of the field configuration currently occupied — a genuine
"the floor gives way" threshold rather than a soft crossover.

Evaluated against the Section 11 fit $(\epsilon_0,\lambda,v) =
(1.726\times10^{-3}, 0.1175, 0.3268)$:

$$\epsilon_0\,a(t)_{crit} \approx 6.314\times10^{-3}, \qquad
\frac{a(t)_{crit}}{a(t)_{now}} \approx 3.658, \qquad
\phi_{crit} \approx 0.1887$$

$\phi_{crit}$ sits between the node state ($\phi=0$) and the void state
($\phi=v\approx0.327$) — a concrete, interpretable field value. The
dimensionless ratio $a(t)_{crit}/a(t)_{now}\approx3.658$ is the open
piece: it is derived from the same bare constants as every other
Section 11 prediction, with no new machinery, but its physical meaning —
what clock $a(t)$ represents across a full accumulation-to-eruption cycle,
as opposed to within our event's expansion history — is not yet
established.

**What remains:** two candidate readings of $a(t)$ have been identified
but not yet developed. (i) Treat $a(t)$ as a proxy for accumulated dark
mass via the integral $M_{dark}(T)$ of Section 2 — under this reading,
3.658 would translate into a *mass ratio*: how much further accumulation,
relative to the present, triggers restart. (ii) Treat $a(t)$ as a
genuinely independent clock for the full cycle with no fixed relationship
to our event's $a(t)$ — defensible, but leaves 3.658 a bare number without
immediately feeding Problem 2. Reading (i) is the more promising route,
since it would directly supply the "volume term" Problem 2 needs.

This problem no longer blocks on a missing mathematical home — it blocks
on choosing and developing one of these two readings.

---

## 2. Anulus Nucleation Rate and Event Separation

**The problem:**
If eternal space hosts many eruption events, how frequently do they
occur and how far apart are they? A rate formula is needed — events
per unit volume per unit time — derived from the dark remnant
accumulation rate and the threshold condition.

**Why it matters:**
Without this, the Anulus extension — the multiply connected, eternally
populated cosmology — remains conceptually developed but geometrically
unspecified. The scale of the structure cannot be estimated.

**What a solution requires:**
The restart threshold (Problem 1) as a prerequisite, combined with
the dark remnant accumulation integral already in Claude_underpinnings.md,
to yield a characteristic inter-event spacing and recurrence timescale.

**Status: mathematical home established; numerically anchored at one
scale; inter-event rate still open.**

The Anulus section of Claude_mathematical_map.md gives this problem a
mathematical home: Coleman-Callan bubble nucleation theory provides the
formal language for nucleation rate per unit volume, and Stauffer-Aharony
percolation theory provides the framework for characterizing event
density and connectivity across the Anulus.

Section 11 of Claude_underpinnings.md fits $(\epsilon_0, \lambda, v)$
against the SDSS/Hamaus void density profile and obtains
$r_{nuc}(z) = 30(1+z)^2$ Mpc/h at present epoch, checked against BOSS
DR16 redshift bins to within ~5%. This gives a concrete characteristic
spacing scale for void nucleation — a first empirical handle on the
geometry of the Anulus at the scale of our own event.

**What remains:** this anchor is a fit to *our* event's void structure,
not yet a derivation of the *inter-event* spacing in the Anulus — the
nucleation rate for entire eruption events, as opposed to voids within
one. Problem 1's progress changes this problem's status concretely: if
the reading-(i) interpretation of $a(t)_{crit}$ (above) is developed,
the ratio 3.658 becomes a mass-accumulation factor that can serve directly
as the "volume term" in a Coleman-Callan-style rate formula, with the
Section 11 wall-tension expressions supplying the "surface term." The
dependency on Problem 1 has therefore narrowed from "wait for a threshold
to exist at all" to "wait for one specific interpretive step on an
existing threshold." The status moves from "mapped, with a numerically
anchored analog at one scale" to "mapped, anchored, and one interpretive
step in Problem 1 away from a first symbolic rate formula."

---

## 3. Tidal Seeding and the Casting Mechanism

**The problem:**
Gravity does not respect the boundaries between eruption events. Matter
condensing in one event can be deflected, captured, or seeded by the
gravitational influence of a neighboring event. The casting mechanism —
the formal description of matter transfer across event boundaries — has
not yet been derived.

**Why it matters:**
This is the physical process underlying the JWST anomaly explanation.
Without a formal mechanism, the inherited material hypothesis remains
an assertion rather than a prediction.

**What a solution requires:**
A treatment of gravitational interaction across vacancy field boundaries,
yielding a predicted mass transfer rate and the conditions under which
casting occurs versus is suppressed.

**Status: mathematical setting established; derivation not started;
unaffected by recent progress.**

The conceptual framework is established. The tidal seeding analogy is
developed qualitatively in Claude_framework.md. The Anulus section of
Claude_mathematical_map.md maps this problem to bubble collision
literature (Garriga-Guth-Vilenkin) and percolation theory, treating
event boundaries as permeable interfaces between percolating clusters.
This gives the casting mechanism a formal mathematical setting for the
first time.

**What remains:** the derivation itself — a mass transfer rate expressed
in terms of boundary geometry and the vacancy field gradient at the
interface, generalizing the single-field gradient calculations of
Section 8 (lensing) and Section 9 (diffuse halos) to *two adjacent
fields* meeting at a permeable boundary. Unaddressed by the Section 11
SDSS fit, which concerns single-event void structure rather than
inter-event boundaries, and unaffected by the Section 12 restart
threshold, which concerns the temporal trigger rather than spatial
boundary dynamics. This problem is the prerequisite for Problem 5, and
of the three remaining derivations (3, 4's boundary refinement, 5), this
is the one with no partial numerical result yet — the highest-leverage
and currently the least-started.

---

## 4. CMB Cold Spot as Boundary Signature

**The problem:**
The CMB cold spot is one of observational cosmology's unexplained
anomalies. The hypothesis is that it marks a region where our eruption
event's boundary meets a neighboring one — a zone of vacancy field
interference between two events. This has not yet been developed into
a testable prediction.

**Why it matters:**
If correct, it would be the first direct observational evidence of the
Anulus structure — a neighboring eruption event leaving a detectable
imprint on our CMB. It is also independently anomalous and in need of
explanation under any framework.

**What a solution requires:**
A predicted angular size and temperature profile for a boundary
interference region, derived from the vacancy field domain wall
equations, that can be compared against existing CMB maps.

**Status: generic-void temperature estimate complete and correct-sign;
two refinements remain, of different character.**

The qualitative identification of the cold spot as a candidate boundary
signature is established. The Anulus section of Claude_mathematical_map.md
maps this to bubble collision geometry (Garriga-Guth-Vilenkin), which
gives a standard formalism for predicting the angular signature of a
bubble-bubble interface as seen from inside one bubble. Combined with the
light-as-phase-transition-signature mechanism — which already gives the
CMB itself a derived origin as latent heat of the eruption event — the
cold spot becomes a candidate perturbation on that latent heat signature
at the boundary.

Section 11 of Claude_underpinnings.md computes a line-of-sight ISW
estimate using the fitted void profile at $r_v = 30$ Mpc/h, obtaining
$\Delta T/T \sim -2.7\times10^{-6}$ — the correct sign for a cold spot,
and within roughly a factor of 4 of the observed $|\Delta T/T| \sim
10^{-5}$.

**What remains — two refinements, distinguished by dependency:**

*(a) The ISW decay factor* — the existing estimate uses a placeholder
~30% potential-decay factor rather than a derived time-integral of
$d\Phi/d\tau$ over the void's evolution history. The machinery for this —
the $a(t)$-dependence of $\delta_w(a)$ and $\sigma_{wall}(a)$ — already
exists in Claude_underpinnings.md (Sections 7 and 10). This refinement
has **no dependency on Problems 1–3**: it is a self-contained calculation
using results already in hand, and is currently the most tractable open
step in the entire document.

*(b) The boundary-specific angular signature* — Section 11's calculation
treats this as an ordinary void's ISW signature, not yet specifically a
*boundary* signature between two Anulus events. This requires combining
the inter-event geometry from Garriga-Guth-Vilenkin with the numerical
fit, and shares its dependency structure with Problem 3 (both require the
two-field boundary treatment).

The status moves from "angular size and profile both open" to: a
same-order, correct-sign temperature estimate exists for a generic void;
refinement (a) is an independent, currently-tractable calculation;
refinement (b) is bundled with Problem 3's dependency on a two-field
boundary treatment.

---

## 5. JWST Anomaly Mass Function

**The problem:**
The James Webb Space Telescope finds galaxies and black holes that are
too massive too early — inconsistent with standard formation timescales.
The framework's explanation is inherited material: matter cast in from
a neighboring or preceding eruption event. This explanation has not yet
been made quantitative.

**Why it matters:**
The JWST anomalies are a live and unresolved problem in mainstream
cosmology. A quantitative prediction that matches the observed excess
mass as a function of redshift would be a significant evidential test
of both the casting mechanism and the Anulus extension.

**What a solution requires:**
A predicted mass excess as a function of redshift, derived from the
casting mechanism (Problem 3), distinguishable from standard hierarchical
formation models.

**Status: unchanged — fully dependent on Problem 3.**

Dependent on Problem 3, which has a mapped mathematical home in bubble
collision and percolation theory but no derivation yet — the SDSS fit
addresses single-event void structure and does not bear on inter-event
mass transfer, and the Problem 1 restart threshold concerns timing rather
than boundary mass transfer. Once a mass transfer rate is derived for
Problem 3, this problem inherits that machinery directly: the rate,
integrated against the percolation-theory description of event density
from Problem 2 — itself now one interpretive step from a first rate
formula — would yield the redshift-dependent mass excess this problem
requires. The qualitative identification of inherited material as the
explanation is established in Claude_framework.md.

---

## Summary of Status and Dependencies

| # | Problem | Mathematical home | Numerical anchor | Remaining work |
|---|---|---|---|---|
| 1 | Restart threshold | Bifurcation/catastrophe theory on $V(\phi)$ | Closed-form + numerical: $a_{crit}/a_{now}\approx3.658$, $\phi_{crit}\approx0.189$ | One interpretive choice (reading of $a(t)$) |
| 2 | Anulus nucleation rate | Coleman-Callan, percolation | $r_{nuc}(z)=30(1+z)^2$ Mpc/h (intra-event, ~5%) | Inter-event rate; one step from Problem 1 |
| 3 | Casting mechanism | Garriga-Guth-Vilenkin, percolation | None | Two-field boundary gradient derivation — not started |
| 4 | CMB Cold Spot (boundary) | Garriga-Guth-Vilenkin + latent heat | $\Delta T/T\sim-2.7\times10^{-6}$ (generic void) | (a) ISW decay factor — independent, tractable now; (b) boundary-specific — bundled with Problem 3 |
| 5 | JWST mass function | Bubble collision + percolation | None | Fully dependent on Problem 3 |

**Reading the table for next steps:** the most self-contained piece of
remaining work is Problem 4(a) — no dependencies, machinery already in
hand. The most consequential single step is the Problem 1 interpretive
choice, since it is the only thing standing between the current state and
a first symbolic Anulus nucleation rate (Problem 2), which in turn is the
"event density" input that Problem 5 needs once Problem 3 is solved.
Problem 3 remains the largest single piece of undone derivation, and the
one that, once complete, unlocks both itself, Problem 4(b), and Problem 5.

---

*Last updated: June 2026*
*Cristóbal Eduardo Kendris García and Claude*
