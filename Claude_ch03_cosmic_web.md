<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 3 — The Cosmic Web

---

## Section 5: Observational Data on Wall Formation

**What We Observe**

The cosmic web is not conjecture — it's one of the most robustly observed structures in astronomy.

*Redshift Surveys*

- The 2dF Galaxy Redshift Survey and SDSS mapped hundreds of thousands of galaxies and confirmed the filament-void-node topology at large scales
- The voids are real, measurable, and statistically characterizable — typical void diameter 20-50 Mpc
- The walls — thin sheets of galaxies bounding voids — are observed directly as **two-dimensional structures** separating adjacent void regions

*Specific Wall Observations*

- The **Boötes Void** — roughly 330 million light years across, nearly empty, bounded by a shell of galaxies
- The **Sloan Great Wall** — a filamentary structure roughly 1.37 billion light years long
- The **Hercules-Corona Borealis Great Wall** — potentially the largest observed structure, ~10 billion light years, though its status is debated
- These structures suggest walls form at multiple scales — not a single characteristic length

*What the Walls Look Like Structurally*

- Thickness is small relative to extent — genuinely sheet-like
- Galaxy density inside voids is roughly 20% of mean cosmic density — not empty but significantly underdense
- The boundaries are **sharp relative to void interiors** — the transition from void to wall happens over surprisingly small distances
- This sharpness is exactly what a domain wall solution would predict

**What Simulations Show**

The Millennium Simulation and its successors reproduce the cosmic web topology from gravitational dynamics alone — starting from CMB-era perturbations and evolving forward. Key findings:

- Wall formation is a **gravitational sheet collapse** phenomenon — pancake collapse in Zel'dovich approximation
- Walls form first, then fragment into filaments, then nodes — there's a **formation sequence**
- The sharpness of boundaries increases over time as matter drains from voids into walls and filaments
- Void interiors become increasingly empty as the universe ages — the lattice is **sharpening with time**

**What This Means For Our Potential**

This observational picture is suggestive of the structured potential over the simple restoring force, for several reasons:

The **sharpness of boundaries** is hard to produce from a linear field. Domain walls are naturally sharp — their thickness is set by $1/\sqrt{\lambda} \cdot v$ and can be made arbitrarily thin by choosing $\lambda$ large. The observed wall geometry matches this.

The **formation sequence** — walls before filaments before nodes — maps naturally onto a symmetry breaking scenario where the field settles into its vacuum state progressively, with defects forming at the intersections.

The **multi-scale structure** — walls at many scales, not one characteristic length — suggests the potential may have more structure than a simple double well. Possibly a **hierarchy of minima** at different scales.

The **sharpening over time** — voids getting emptier, walls getting denser — is consistent with the vacancy field deepening into its minimum over cosmological time. The field is still settling.

**The Tension**

Standard cosmology reproduces the cosmic web topology **without** invoking a structured scalar field. It does it with gravity alone, starting from quantum fluctuations inflated to cosmic scales. That's a competing explanation for the same observations.

What this framework needs — and what would distinguish it observationally — is a prediction about wall properties that **differs** from the gravitational collapse picture. Candidates:

- A characteristic wall thickness predicted by $V(\phi)$ parameters that differs from gravitational sheet collapse predictions
- A specific **void size distribution** determined by the lattice geometry rather than initial perturbation spectrum
- Polarization or phase coherence in the CMB that reflects domain wall boundaries rather than acoustic oscillations

**The Most Provocative Observation**

The void size distribution in the observed universe follows a roughly **lognormal distribution** — not a random Poisson distribution. That regularity suggests the lattice has a preferred scale, or at least a scale-dependent structure.

That is exactly what a structured potential with a specific $v$ would produce.

---

## Section 6: The Void Size Distribution as a Probe of V(φ)

The observed void size distribution is well-fitted empirically by a lognormal:

$$P(r) = \frac{1}{r\sigma\sqrt{2\pi}}\exp\left(-\frac{(\ln r - \mu)^2}{2\sigma^2}\right)$$

Where $r$ is void radius, $\mu$ is the log-mean, and $\sigma$ is the log-variance. This is observationally established. The question is what *generates* it.

**What Standard Cosmology Says**

Standard cosmology derives the void size distribution from the **initial power spectrum** of density perturbations — essentially the pattern of quantum fluctuations from inflation, stretched to cosmic scales. The lognormal emerges as a statistical consequence of gravitational collapse acting on Gaussian initial conditions.

It's a bottom-up explanation. Small fluctuations grow, collapse, and leave voids as a residue.

**What Our Framework Says**

In our framework the void size distribution is determined by the **vacuum structure of** $V(\phi)$ — specifically by the characteristic length scale over which the field transitions between vacua.

For a double well potential the domain wall thickness is:

$$\delta_w = \frac{1}{v\sqrt{\lambda}}$$

And the characteristic void radius is set by the **nucleation length** — the minimum size a void region must reach before the field stabilizes into its vacuum state. This is analogous to bubble nucleation in a phase transition:

$$r_{nuc} = \frac{3\delta_w}{\epsilon}$$

Where $\epsilon$ is the energy difference between the two vacua — the asymmetry of the potential if the wells are not perfectly symmetric.

**The Key Implication**

If the two vacua are **exactly symmetric** — $\epsilon = 0$ — then:

- Void sizes have no preferred scale
- Distribution is scale-free — a power law, not lognormal
- The lattice has no characteristic cell size

If the vacua are **asymmetric** — $\epsilon \neq 0$ — then:

- There is a preferred nucleation scale $r_{nuc}$
- The distribution peaks at that scale and falls off on either side
- **This produces the lognormal**

The observed lognormal therefore implies $\epsilon \neq 0$ — the potential is **asymmetric**. The two vacua are not equivalent. One is deeper than the other.

**What Breaks The Symmetry**

The natural candidate is **the direction of time** — the cosmological expansion preferentially selects one vacuum over the other as the universe ages and voids deepen.

Mathematically we can encode this as a time-dependent asymmetry:

$$\epsilon(t) = \epsilon_0 \cdot a(t)$$

Where $a(t)$ is the cosmological scale factor. As the universe expands, the asymmetry grows, the preferred vacuum deepens, and the characteristic void scale shifts — slowly, but measurably.

**The Testable Prediction**

This gives us something concrete. If $\epsilon(t) = \epsilon_0 \cdot a(t)$ then the peak of the void size distribution should **shift with redshift** — voids at higher redshift should have a different characteristic size than voids at low redshift, in a specific calculable way.

That prediction is:

$$r_{nuc}(z) = \frac{r_{nuc,0}}{1+z} \cdot f(\epsilon_0, \lambda, v)$$

Where $f$ is a function of the potential parameters solved for in Chapter 4.

---
---
## A Living Document

Some conceptual areas explored here are still under active development. The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.
---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
