<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>
# The Claude Theory — Open Problems

This document records unresolved problems in the Claude Theory framework.
It is maintained as a live working document. Its presence reflects the
authors' view that a theory which honestly documents its open questions
is more credible than one that does not.

---

## 1. The Restart Threshold

**The problem:**
The theory describes the accumulation-to-eruption cycle but has not yet
specified the trigger condition mathematically. At what accumulated mass,
density, or vacancy field energy does the phase transition fire?

**Why it matters:**
Without a derivable threshold condition, the eruption event remains
qualitatively described but not quantitatively predicted. A testable
number is needed.

**What a solution requires:**
A derivation from the vacancy field parameters already established in
Claude_underpinnings.md that yields a critical field energy or mass
density at which the asymmetric double-well potential undergoes
catastrophic reorganization.

**Partial progress:**
Section 12 of Claude_underpinnings.md derives this threshold directly
from the potential $V(\phi) = \lambda(\phi^2-v^2)^2 - \epsilon_0 a(t)\phi$
as a bifurcation condition: the point at which the cubic
$dV/d\phi = 0$ transitions from three real roots to one, and the shallow
minimum the field currently occupies merges with the local maximum and
annihilates. The discriminant condition gives a closed form,

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\lambda v^3, \qquad
\phi_{crit} = \frac{v}{\sqrt{3}}$$

Evaluated against the Section 11 fit
$(\epsilon_0, \lambda, v) = (1.726\times10^{-3}, 0.1175, 0.3268)$, this
gives $a(t)_{crit}/a(t)_{now} \approx 3.658$.

This problem now has a mapped mathematical home and a numerical value,
where previously it had neither. It is no longer the only problem in this
document without a mapped mathematical home.

**What remains:**
The ratio $3.658$ is dimensionless. Its physical meaning is not yet
established — specifically, what clock $a(t)$ represents across the full
accumulation-eruption cycle, as distinct from the $a=1$ normalization used
in Section 11 for *our* event's present-epoch void structure. Converting
the ratio into a physical timescale, or into a meaningful "how much further
accumulation remains," is the open step. This is now the focus of ongoing
work and remains the most consequential open problem in the framework:
every other open problem either depends on it directly (Problem 2) or is
independently tractable without it (Problems 3–5) — though Problem 1 has
moved from "no mathematical home" to "mathematical home and numerical
value established, physical interpretation of that value open."

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

**Partial progress:**
The Anulus section of Claude_mathematical_map.md gives this problem a
mathematical home: Coleman-Callan bubble nucleation theory provides the
formal language for nucleation rate per unit volume, and Stauffer-Aharony
percolation theory provides the framework for characterizing event
density and connectivity across the Anulus.

This problem now carries a numerical anchor as well. Section 11 of
Claude_underpinnings.md fits $(\epsilon_0, \lambda, v)$ against the
SDSS/Hamaus void density profile and obtains $r_{nuc}(z) = 30(1+z)^2$
Mpc/h at present epoch, checked against BOSS DR16 redshift bins to
within ~5%. This gives a concrete characteristic spacing scale for void
nucleation — a first empirical handle on the geometry of the Anulus at
the scale of our own event.

What remains: this anchor is a fit to *our* event's void structure, not
yet a derivation of the *inter-event* spacing in the Anulus — the
nucleation rate for entire eruption events, as opposed to voids within
one. The dependency on Problem 1 for a first-principles threshold remains,
though Problem 1 itself now has a numerical value (Section 12) whose
physical interpretation, once established, would feed directly into this
problem's recurrence timescale. The status moves from "mapped but not yet
derivable" to "mapped, with a numerically anchored analog at one scale, and
a candidate threshold value from Problem 1 awaiting physical interpretation."

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

**Partial progress:**
The conceptual framework is established. The tidal seeding analogy is
developed qualitatively in Claude_framework.md. The Anulus section of
Claude_mathematical_map.md maps this problem to bubble collision
literature (Garriga-Guth-Vilenkin) and percolation theory, treating
event boundaries as permeable interfaces between percolating clusters.
This gives the casting mechanism a formal mathematical setting for the
first time. The remaining step is the derivation itself: a mass transfer
rate expressed in terms of the boundary geometry and the vacancy field
gradient at the interface. Unaddressed by the Section 11 SDSS fit or by
Section 12's restart threshold, both of which concern single-event
structure rather than inter-event boundaries. This problem is the
prerequisite for Problem 5.

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

**Partial progress:**
The qualitative identification of the cold spot as a candidate boundary
signature is established. The Anulus section of Claude_mathematical_map.md
maps this to bubble collision geometry (Garriga-Guth-Vilenkin), which
gives a standard formalism for predicting the angular signature of a
bubble-bubble interface as seen from inside one bubble. Combined with the
light-as-phase-transition-signature mechanism — which already gives the
CMB itself a derived origin as latent heat of the eruption event — the
cold spot becomes a candidate perturbation on that latent heat signature
at the boundary.

This problem now carries a numerical result as well. Section 11 of
Claude_underpinnings.md computes a line-of-sight ISW estimate using the
fitted void profile at $r_v = 30$ Mpc/h, obtaining $\Delta T/T \sim
-2.7\times10^{-6}$ — the correct sign for a cold spot, and within roughly
a factor of 4 of the observed $|\Delta T/T| \sim 10^{-5}$.

What remains: the ISW estimate uses a placeholder ~30% potential-decay
factor rather than a derived time-integral of $d\Phi/d\tau$ over the
void's evolution history (the machinery for which — $a(t)$-dependence of
$\delta_w$ and $\sigma_{wall}$ — already exists in Claude_underpinnings.md).
The angular size prediction for the cold spot, as distinct from its
temperature depth, has not been derived. And critically: Section 11's
calculation treats this as an ordinary void's ISW signature, not yet as
specifically a *boundary* signature between two Anulus events — the
inter-event geometry from Garriga-Guth-Vilenkin has not yet been combined
with the numerical fit. The status moves from "angular size and profile
both open" to "a same-order, correct-sign temperature estimate exists for
a generic void; the boundary-specific angular and refined profile
derivation remains open."

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

**Partial progress:**
Dependent on Problem 3, which has a mapped mathematical home in bubble
collision and percolation theory (see above) but no Section 11 or
Section 12 progress — both address single-event structure and do not
bear on inter-event mass transfer. Once a mass transfer rate is derived
for Problem 3, this problem inherits that machinery directly: the rate,
integrated against the percolation-theory description of event density
from Problem 2 — now partially anchored numerically — would yield the
redshift-dependent mass excess this problem requires. The qualitative
identification of inherited material as the explanation is established
in Claude_framework.md.

---

*Last updated: June 2026*
*Cristóbal Eduardo Kendris García and Claude*
