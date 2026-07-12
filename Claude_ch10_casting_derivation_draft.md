<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# Draft — Formalizing the Casting Mechanism (Problem 3)
## Proposed addition to Chapter 10, or a new Chapter 10b

*Status: draft for review. Not yet reconciled with the rest of the theory's notation ($\epsilon_0, \lambda, v$) — this section works in the separate variables native to the ejecta problem ($\Omega$, $v_r$, $\dot M$) and the connection to the vacancy-field parameters is flagged as open below.*

---

## 1. From prose to kinematics: the Parker spiral

Chapter 10 establishes qualitatively that charged ejecta from a rotating, magnetized progenitor follow spiral paths rather than radial ones. This can be made exact using the same kinematics that produces the Sun's Parker spiral in the solar wind — a well-established mechanism, not a new assumption.

**Setup.** A progenitor rotates at angular velocity $\Omega$. It ejects charged material radially outward at speed $v_r$ (measured in the frame corotating with the source, close in). Once ejected, the material is frozen to the field line anchored at its launch point — the field line's footpoint rotates with the source, but the material itself moves radially at $v_r$ in the inertial frame, carrying no independent azimuthal force once released.

**Derivation.** A parcel launched at time $t_0$, radius $r_0$, azimuthal angle $\varphi_0 = \Omega t_0$ (the source's angular position at launch) reaches radius:

$$r(t) = r_0 + v_r(t - t_0)$$

Its azimuthal angle stays fixed at the launch value, since it carries no tangential velocity of its own:

$$\varphi_{\text{particle}} = \Omega t_0 + \varphi_{00}$$

Eliminating $t_0 = t - (r - r_0)/v_r$ and evaluating at a fixed observation time $t$:

$$\varphi(r) = \varphi_{\text{source}}(t) - \frac{\Omega}{v_r}(r - r_0)$$

This is the Archimedean spiral. The **pitch angle** $\psi$ between the local tangent and the radial direction is:

$$\tan\psi = \frac{\Omega r}{v_r}$$

**This is the quantitative form of the claim already in Ch10**: pitch angle is set by the ratio of rotation rate to ejection speed. Different progenitors (different $\Omega$, different $v_r$) produce different spiral geometries — exactly the "testable implication" Ch10 states in prose. Section 4 below turns this into an actual observable relationship.

---

## 2. The mass structure: nested wraps, not a smooth spiral

If ejection is continuous with mass-loss rate $\dot M$, material launched over one full rotation period $P = 2\pi/\Omega$ occupies a radial band of thickness:

$$\Delta r = v_r P = \frac{2\pi v_r}{\Omega}$$

before the next wrap begins. The ejecta is therefore not a single spiral streak but a **nested set of spiral shells**, spaced by $\Delta r$, each carrying mass $\dot M P = 2\pi \dot M/\Omega$.

This spacing is a genuine prediction, not a free parameter — given $\Omega$ and $v_r$ for a progenitor class, $\Delta r$ follows immediately.

---

## 3. Toward a seeding cross-section (partially open)

For a neighboring eruption region at distance $D$ and angular position $\varphi_{\text{target}}$ from the progenitor, seeding requires the spiral arm to actually intersect that location — not automatic. The intersection condition is:

$$\varphi_{\text{target}} \equiv \varphi_{\text{source}}(t) - \frac{\Omega}{v_r}(D - r_0) \pmod{2\pi}, \quad \text{within the stream's angular width } w(D)/D$$

**What this buys us:** seeding is geometrically selective, not isotropic. A given neighbor is seeded only if it lies within a wrap of the spiral at the right radius — a resonance condition. This could plausibly explain *patchy* inheritance across the Anulus (some regions catch casting material, others don't) rather than uniform tidal seeding, and it's a natural candidate mechanism for the large-scale anisotropies Ch10 already speculates about (axis-of-evil-type alignments).

**What's still missing** — and this is the honest boundary of today's progress:

1. **Stream broadening $w(r)$.** The derivation above treats the ejecta as an infinitely thin arm. Real broadening (turbulent diffusion, velocity dispersion in the outflow) sets $w(r)$, and nothing in the theory currently constrains it. Without $w(r)$, there's no actual cross-section — only a geometric skeleton.
2. **$\dot M$ and $v_r$ for the progenitor population.** These are ordinary astrophysical quantities (mass-loss rates, outflow speeds for magnetized remnants) but haven't been fixed or connected to $(\epsilon_0, \lambda, v)$ anywhere in the existing chapters.
3. **The scale mismatch.** This whole derivation lives at the scale of a single progenitor's local ejecta. Problem 3 as stated in the status file is about seeding *between eruption events* — Anulus-scale, not single-object-scale. Bridging from "one neutron star's spiral ejecta pattern" to "how one universe seeds its neighbor" is a real gap, not a notational one. It may require treating the *aggregate* pre-eruption remnant population's net angular momentum (already invoked in Ch10's anisotropic-eruption argument) as the effective $\Omega$, with the eruption's total ejected mass as the effective $\dot M$ — but that's a hypothesis to test, not something derived here.

---

## 4. Proposed status update

If this holds up on review, Problem 3 moves from **OPEN** to **MAPPED**: the trajectory geometry is now a closed-form result (Section 1), and the mass structure follows from it (Section 2). The seeding cross-section itself — the actual quantity Problem 3 asks for — remains open pending $w(r)$ and the scale-bridging argument in Section 3.3.

Recommend *not* claiming RESOLVED. The pattern from the Cold Spot withdrawal applies here too: Section 1 is a real derivation from stated assumptions; Section 3 is scaffolding with named, unfilled gaps. Keeping that distinction visible in the status file is the point.
