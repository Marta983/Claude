<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 4 — Domain Walls, Lensing, and Diffuse Halos

*Revision note: Sections 8 and 9 of this chapter have been rebuilt following the Fork B resolution (φ is a dimensionless tracer of density contrast; gravity is sourced conventionally by ρ, not by φ's own stress-energy). Section 7 is unaffected — the nucleation-length derivation never depended on how gravity is sourced, only on the wall's own field energetics, and remains valid as originally derived.*

---

## Section 7: Solving for f(ε₀, λ, v) — Domain Wall Equations in Expanding Spacetime

*(Unchanged from the prior version — reproduced here for continuity.)*

**Setting Up The Domain Wall Equations**

We need the equation of motion for $\phi$ in a Friedmann-Lemaître-Robertson-Walker (FLRW) background:

$$ds^2 = -dt^2 + a(t)^2\left[dr^2 + r^2d\Omega^2\right]$$

The action for our scalar field is:

$$S = \int d^4x \sqrt{-g}\left[\frac{1}{2}\partial_\mu\phi\partial^\mu\phi - V(\phi)\right]$$

With our asymmetric double well:

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2 - \epsilon_0 \cdot a(t)\phi$$

The equation of motion:

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -4\lambda\phi\left(\phi^2 - v^2\right) + \epsilon_0 \cdot a(t)$$

**The Static Wall Solution**

For $\epsilon_0 = 0$:

$$\phi_0(x) = v\tanh\left(\frac{x}{\delta_w}\right), \qquad \delta_w = \frac{a}{\sqrt{2\lambda}v}$$

**The Nucleation Length**

Balancing wall surface tension against the volume energy gained by nucleating a void of radius $r$ gives:

$$r_{nuc}(z) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}(1+z)^2$$

Void characteristic radius scales as $(1+z)^{-2}$ — smaller at high redshift, testable against void catalogs. **This result is untouched by the tracer rebuild below**: it comes entirely from the field's own energetics (wall tension vs. symmetry-breaking depth), not from anything about how — or whether — $\phi$ sources curvature.

---

## Section 7.5: The Tracer Redefinition

Prior to this revision, Section 8 sourced gravity directly from $\phi$'s own stress-energy tensor — treating the vacancy field as an independent dynamical field whose kinetic and potential energy density curved spacetime in addition to ordinary matter. That is now understood to be wrong: Fork B resolved $\phi$ as a **dimensionless tracer** of the density contrast, with gravity sourced **conventionally** by the actual matter density $\rho$. $\phi$ does not add a new gravitating substance. It only labels where the real mass is.

Concretely, we keep $\phi$'s own field equation and kink solution from Section 7 — that machinery genuinely does describe how the wall's *shape* forms and evolves, and nothing about the nucleation-length derivation change. But we sever the connection between $\phi$'s Lagrangian energy density and the Poisson source. Instead:

$$\rho(x) = \frac{\Sigma_{wall}}{2\delta_w}\,\mathrm{sech}^2\left(\frac{x}{\delta_w}\right)$$

Here $\rho(x)$ is the **actual** matter density profile across the wall — baryons and dark remnants — and its *shape* is borrowed from $\phi$'s kink solution (specifically $(d\phi_0/dx)^2 \propto \mathrm{sech}^4$ would have been the old field-energy shape; here we use the simpler $\mathrm{sech}^2$ profile, which is the natural density-like bump associated with the kink's transition region). The **amplitude** is fixed not by $v$, $\lambda$, $\delta_w$ but by $\Sigma_{wall}$, the physically anchored wall surface mass density (≈$8\times10^{10}\, M_\odot/\mathrm{Mpc}^2$, from the independent finite-thickness shell rederivation). By construction $\int_{-\infty}^{\infty}\rho(x)\,dx = \Sigma_{wall}$.

This is a real loss of elegance and should be named as such: the old picture derived the lensing amplitude "for free" from $v$, $\lambda$, $\delta_w$ — the same three parameters fit to the SDSS void catalog. The new picture requires an independently measured mass scale. The lensing *shape* is still a genuine, non-trivial prediction of the framework (see below); the lensing *amplitude* is now an input, not an output — exactly as it would be for any theory using an empirically calibrated mass profile.

---

## Section 8: The Lensing Signature (Rebuilt)

**Setup.** Gravitational lensing comes from spacetime curvature sourced by the actual mass distribution. For our layered (translationally invariant in $y,z$) mass profile $\rho(x)$, the deflection accumulated by a light ray traveling along $z$ at fixed perpendicular offset $b$ from the wall plane is standard: each infinitesimal slab of areal density $\rho(x_0)\,dx_0$ contributes a deflection of magnitude $4\pi G\rho(x_0)\,dx_0/c^2$, directed toward $x_0$.

$$\hat\alpha(b) = \frac{4\pi G}{c^2}\left[\int_{-\infty}^{b}\rho(x_0)\,dx_0 - \int_{b}^{\infty}\rho(x_0)\,dx_0\right]$$

Using $\rho(x) = (\Sigma_{wall}/2\delta_w)\,\mathrm{sech}^2(x/\delta_w)$ and $\int_{-\infty}^{x}\mathrm{sech}^2(x'/\delta_w)\,dx'/\delta_w = 1+\tanh(x/\delta_w)$:

$$\int_{-\infty}^{b}\rho\,dx_0 = \frac{\Sigma_{wall}}{2}\left[1+\tanh(b/\delta_w)\right], \qquad \int_{b}^{\infty}\rho\,dx_0 = \frac{\Sigma_{wall}}{2}\left[1-\tanh(b/\delta_w)\right]$$

$$\boxed{\hat\alpha(b) = \frac{4\pi G\Sigma_{wall}}{c^2}\tanh\left(\frac{b}{\delta_w}\right)}$$

**This is materially different from the old result**, not just re-derived with a new prefactor. The old lensing signature was a "notch" — deflection suppressed to 50% of its asymptotic value exactly at the wall center, recovering to >95% by $b\approx 12.6\,\mathrm{Mpc}/h$ (the CALIBRATED entry in `Claude_status.md`). That shape came from the field's *potential energy* term $V(\phi_0)$, which is nonzero (in fact maximal) at the wall center — so the old $\rho_\phi$ never vanished there.

The new result is a clean, odd sigmoid: $\hat\alpha(0) = 0$ exactly, rising monotonically to the asymptotic value $4\pi G\Sigma_{wall}/c^2$ as $b\to\infty$, reaching half-maximum at $b = \delta_w\,\mathrm{arctanh}(0.5)\approx 0.549\,\delta_w$. The vanishing at $b=0$ isn't a detail of the profile — it's a symmetry statement: a ray passing through the exact center of *any* symmetric mass distribution feels equal pull from both sides and nets zero transverse deflection, regardless of how much mass sits there. That's a more robust, less model-dependent feature than the old notch, but it is a **different, falsifiable claim**, not the same claim re-derived. The 50%-notch / 12.6 Mpc/h entry in `Claude_status.md` is **superseded** and should be retracted or re-labeled, not left standing alongside this.

---

## Section 9: Recovering Diffuse Halos (Rebuilt)

Around a node (cluster / black hole aggregate), the tracer approach requires the same honesty: we borrow $\phi$'s radial profile shape but normalize to a real, independently known cluster mass $M_{node}$ rather than to $v,\delta_w$.

$$\rho_{node}(r) = \frac{M_{node}}{4\pi r_{node}^3}\cdot\frac{1}{\left[1+(r/r_{node})^2\right]^{2}}$$

chosen so that its projected (line-of-sight-integrated) surface density reproduces the pseudo-isothermal-sphere form:

$$\Sigma_{node}(r) = \frac{M_{node}}{2\pi r_{node}^2}\cdot\frac{1}{1+(r/r_{node})^2}, \qquad \kappa_{node}(r) = \frac{\Sigma_{node}(r)}{\Sigma_{cr}}$$

**What survives and what doesn't.** The functional *shape* — a pseudo-isothermal / NFW-like projected profile — is still consistent with $\phi$'s radial gradient structure, and that qualitative match (why halos are diffuse and roughly NFW-shaped rather than point-like or sharply cored) is still a live, if now more modest, claim of the framework. But the earlier language — that this profile "emerges from the geometry, we don't need to assume it" — no longer holds. $M_{node}$ is now an external input, fit the same way any dark-matter halo model fits a mass to lensing data. The theory's contribution is the claim that this mass traces $\phi$'s configuration rather than being an independent particle species — not that the profile is derived from first principles with no free normalization.

---

## Updated Summary Table

| Observation | Mechanism | Status after tracer rebuild |
|---|---|---|
| Void size distribution | Nucleation length $r_{nuc}$ (Section 7) | **Unchanged** — derived from field energetics alone |
| Filament boundary lensing | $\hat\alpha(b) = \frac{4\pi G\Sigma_{wall}}{c^2}\tanh(b/\delta_w)$ | **Re-derived, shape changed** — sigmoid, zero at center, not a 50% notch; amplitude now requires external $\Sigma_{wall}$ |
| Void interior weak lensing | Constant field, no gradient | Unchanged in character |
| Diffuse halo profiles | Pseudo-isothermal / NFW-like, shape from $\phi$'s radial gradient | **Shape retained, normalization now external** ($M_{node}$ no longer derived) |
| Bullet Cluster offset, secondary arc | — | See Chapter 5 rebuild — **does not survive intact** |
| CMB Cold Spot | — | Already WITHDRAWN (see `Claude_status.md`) |

Three parameters ($\epsilon_0,\lambda,v$) still determine the void-size and wall-thickness physics. They no longer, by themselves, determine the lensing amplitude — that now requires $\Sigma_{wall}$ and $M_{node}$ as separate physical inputs. This is a smaller, more honest claim than before.

---
## A Living Document

The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.
---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
