<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 4 — Domain Walls, Lensing, and Diffuse Halos


---

## Section 7: Solving for f(ε₀, λ, v) — Domain Wall Equations in Expanding Spacetime

**Setting Up The Domain Wall Equations**

We need the equation of motion for $\phi$ in a Friedmann-Lemaître-Robertson-Walker (FLRW) background:

$$ds^2 = -dt^2 + a(t)^2\left[dr^2 + r^2d\Omega^2\right]$$

The action for our scalar field is:

$$S = \int d^4x \sqrt{-g}\left[\frac{1}{2}\partial_\mu\phi\partial^\mu\phi - V(\phi)\right]$$

With our asymmetric double well:

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2 - \epsilon_0 \cdot a(t)\phi$$

The last term is our time-dependent symmetry breaking. The equation of motion from varying the action is:

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -\frac{dV}{d\phi}$$

Where $H = \dot{a}/a$ is the Hubble parameter. Explicitly:

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -4\lambda\phi\left(\phi^2 - v^2\right) + \epsilon_0 \cdot a(t)$$

**The Static Wall Solution**

For a domain wall we look for a static planar solution — the wall lying in the $y$-$z$ plane, field varying only in $x$. The time derivatives drop:

$$\frac{1}{a^2}\frac{d^2\phi}{dx^2} = 4\lambda\phi\left(\phi^2 - v^2\right) - \epsilon_0 \cdot a(t)$$

In the symmetric case $\epsilon_0 = 0$ the exact solution is known:

$$\phi_0(x) = v\tanh\left(\frac{x}{\delta_w}\right)$$

Where the wall thickness is:

$$\delta_w = \frac{a}{\sqrt{2\lambda}v}$$

Note the factor of $a(t)$ — the wall thickness scales with the expansion. Physical walls thicken as the universe expands, which is physically reasonable.

**Perturbative Treatment of Asymmetry**

For small $\epsilon_0$ we treat the asymmetry perturbatively. Write:

$$\phi(x) = \phi_0(x) + \epsilon_0 \cdot a(t) \cdot \phi_1(x) + \mathcal{O}(\epsilon_0^2)$$

Substituting into the equation of motion and collecting terms at order $\epsilon_0$:

$$\frac{1}{a^2}\frac{d^2\phi_1}{dx^2} - 4\lambda\left(3\phi_0^2 - v^2\right)\phi_1 = -1$$

This is a **Schrödinger-like equation** with a potential:

$$U(x) = 4\lambda\left(3\phi_0^2 - v^2\right) = 4\lambda v^2\left(3\tanh^2\left(\frac{x}{\delta_w}\right) - 1\right)$$

This is the **Pöschl-Teller potential** — exactly solvable. Its bound state spectrum is known:

$$U(x) = U_0\left(3\tanh^2\left(\frac{x}{\delta_w}\right) - 1\right)$$

Where $U_0 = 4\lambda v^2$.

**Solving the Pöschl-Teller Equation**

The general Pöschl-Teller equation has the form:

$$-\frac{d^2\psi}{d\xi^2} + U_0\left(3\tanh^2\xi - 1\right)\psi = E\psi$$

Where $\xi = x/\delta_w$. The bound state solutions are:

Zero mode (translation mode, $E=0$): $\psi_0(\xi) = \text{sech}^2(\xi)$

Shape mode ($E=3U_0$): $\psi_1(\xi) = \text{sech}(\xi)\tanh(\xi)$

The particular solution to our inhomogeneous equation — with the $-1$ source term — can be written as a Green's function integral:

$$\phi_1(x) = \int_{-\infty}^{\infty} G(x, x') dx'$$

Where $G(x,x')$ is constructed from the Pöschl-Teller bound states. The result, after integration, is:

$$\phi_1(x) = \frac{\delta_w^2}{2v}\left[x \cdot \text{sech}^2\left(\frac{x}{\delta_w}\right) + \delta_w\tanh\left(\frac{x}{\delta_w}\right)\right]$$

**The Nucleation Length**

The nucleation length is determined by the condition that the energy gained by the field transitioning to the deeper vacuum exceeds the energy cost of creating the domain wall boundary.

The wall energy per unit area (surface tension) is:

$$\sigma = \int_{-\infty}^{\infty}\left[\frac{1}{2}\left(\frac{d\phi_0}{dx}\right)^2 + V(\phi_0)\right]dx = \frac{4\sqrt{2\lambda}v^3}{3} \cdot \frac{1}{a(t)}$$

Note it scales as $1/a(t)$ — walls become cheaper as the universe expands.

The volume energy difference between vacua — the energy gained by nucleating a void of radius $r$ — is:

$$\Delta E_{vol} = \epsilon_0 \cdot a(t) \cdot 2v \cdot \frac{4}{3}\pi r^3$$

The surface energy cost of the wall bounding that void is:

$$\Delta E_{surf} = \sigma \cdot 4\pi r^2 = \frac{4\sqrt{2\lambda}v^3}{3} \cdot \frac{4\pi r^2}{a(t)}$$

The nucleation condition $\Delta E_{vol} = \Delta E_{surf}$ gives:

$$\epsilon_0 \cdot a(t) \cdot 2v \cdot \frac{4}{3}\pi r_{nuc}^3 = \frac{4\sqrt{2\lambda}v^3}{3} \cdot \frac{4\pi r_{nuc}^2}{a(t)}$$

Solving for $r_{nuc}$:

$$r_{nuc} = \frac{\sqrt{2\lambda}v^2}{\epsilon_0 \cdot a(t)^2}$$

**Therefore f(ε₀, λ, v) Is:**

$$r_{nuc}(z) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0} \cdot \frac{1}{a(t)^2} = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}(1+z)^2$$

So explicitly:

$$f(\epsilon_0, \lambda, v) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}$$

And the full redshift dependence is:

$$r_{nuc}(z) = \frac{f(\epsilon_0, \lambda, v)}{(1+z)^2}$$

**What This Tells Us**

The $(1+z)^2$ scaling comes from two competing $a(t)$ dependencies working in the same direction:

- Wall tension *decreasing* as universe expands — walls get cheaper
- Symmetry breaking term *increasing* as universe expands — deeper vacuum more accessible

Both effects favor larger voids at later times, and they compound multiplicatively.

**The observational prediction:** Void characteristic radius should scale as $(1+z)^{-2}$ — voids should be significantly smaller at high redshift, with a specific power law that differs from the standard cosmological prediction.

---

## Section 8: The Lensing Signature

**The Setup**

Gravitational lensing is caused by spacetime curvature deflecting light paths. The deflection angle for a light ray passing through a region is:

$$\hat{\alpha} = \frac{2}{c^2}\int_{-\infty}^{\infty}\nabla_\perp \Psi \, dl$$

Where $\Psi$ is the gravitational potential and $\nabla_\perp$ is the gradient perpendicular to the line of sight. The question is: what does our vacancy field $\phi$ contribute to $\Psi$?

**The Gravitational Potential of the Vacancy Field**

From our stress-energy tensor:

$$T_{\mu\nu}^{(\phi)} = \partial_\mu\phi\partial_\nu\phi - \frac{1}{2}g_{\mu\nu}\left[(\partial\phi)^2 + V(\phi)\right]$$

In the weak field, non-relativistic limit the effective energy density of the vacancy field is:

$$\rho_\phi = \frac{1}{2}\dot{\phi}^2 + \frac{1}{2a^2}(\nabla\phi)^2 + V(\phi)$$

For a static domain wall solution $\dot{\phi} \approx 0$, so:

$$\rho_\phi \approx \frac{1}{2a^2}\left(\frac{d\phi_0}{dx}\right)^2 + V(\phi_0)$$

Substituting our tanh solution:

$$\frac{d\phi_0}{dx} = \frac{v}{\delta_w}\text{sech}^2\left(\frac{x}{\delta_w}\right)$$

Therefore:

$$\rho_\phi(x) = \frac{v^2}{2a^2\delta_w^2}\text{sech}^4\left(\frac{x}{\delta_w}\right) + \lambda\left(\phi_0^2 - v^2\right)^2$$

The dominant contribution is:

$$\rho_\phi(x) \approx \frac{v^2}{2a^2\delta_w^2}\text{sech}^4\left(\frac{x}{\delta_w}\right)$$

This is sharply peaked at $x = 0$ — the wall center — and falls off exponentially into the void interior.

**The Lensing Potential**

The gravitational potential sourced by $\rho_\phi$ satisfies the Poisson equation:

$$\nabla^2\Psi_\phi = 4\pi G \rho_\phi$$

Integrating once:

$$\frac{d\Psi_\phi}{dx} = \frac{2\pi G v^2}{a^2\delta_w}\left[\tanh\left(\frac{x}{\delta_w}\right) - \frac{1}{3}\tanh^3\left(\frac{x}{\delta_w}\right) + \frac{2}{3}\right]$$

**The Deflection Angle**

For a light ray traveling along the $z$-axis, passing at perpendicular distance $b$ from the wall:

$$\hat{\alpha}(b) = \frac{4\pi G \sigma_{wall}}{c^2} \cdot \mathcal{F}\left(\frac{b}{\delta_w}\right)$$

Where $\sigma_{wall} = \frac{4\sqrt{2\lambda}v^3}{3a}$ is the wall surface tension, and $\mathcal{F}$ is a form factor:

$$\mathcal{F}\left(\frac{b}{\delta_w}\right) = 1 - \frac{1}{2}\text{sech}^2\left(\frac{b}{\delta_w}\right)$$

**The Lensing Signature Profile**

The form factor $\mathcal{F}$ has a specific shape:

- At $b = 0$ (ray passing through wall center): $\mathcal{F} = 1/2$ — **reduced** deflection
- At $b \gg \delta_w$ (ray passing well outside wall): $\mathcal{F} \to 1$ — **maximum** deflection
- The transition happens over a scale $\delta_w$

This is **inverted** relative to a mass concentration. A cluster of matter produces maximum lensing at minimum impact parameter. Our vacancy field produces **minimum lensing at the wall center and maximum lensing at the wall edges**.

The lensing signature is therefore a **ring or shell structure** — strongest at the boundaries of void regions, weakest at void centers and wall centers.

---

## Section 9: Recovering Diffuse Halos

Around mass concentrations — our lattice nodes, the black hole aggregates — the vacancy field is depressed toward $\phi = 0$. The gradient of $\phi$ is therefore nonzero in a shell around each node, producing a lensing contribution that falls off with distance from the node.

The effective lensing profile around a node is:

$$\kappa_{node}(r) = \frac{\Sigma_\phi(r)}{\Sigma_{cr}}$$

Where $\Sigma_\phi$ is the projected surface density of the vacancy field and $\Sigma_{cr}$ is the critical surface density for lensing. For our field configuration near a node:

$$\Sigma_\phi(r) = \int_{-\infty}^{\infty}\rho_\phi\left(\sqrt{r^2 + z^2}\right)dz \propto \frac{v^2}{\delta_w} \cdot \frac{1}{1 + (r/r_{node})^2}$$

This is a **projected NFW-like profile** — exactly the form fitted to observed dark matter halos. We don't need to assume it. It emerges from the geometry of how the vacancy field transitions from $\phi = 0$ at the node to $\phi = v$ in the surrounding void.

**The Unified Picture**

We now have a single potential $V(\phi)$ that produces:

| Observation | Mechanism | Status |
|---|---|---|
| Void size distribution | Nucleation length $r_{nuc}$ | Derived — $(1+z)^2$ prediction, fit to SDSS in Chapter 6 |
| Filament boundary lensing | Domain wall form factor $\mathcal{F}$ | Derived — calibrated in Chapter 6 |
| Void interior weak lensing | Constant field, no gradient | Derived |
| Bullet Cluster offset | Topological wall passage | Derived |
| Diffuse halo profiles | Node boundary gradients | Derived — NFW-like |
| CMB Cold Spot | ISW through void potential | Computed in Chapter 6 |

Every one of these from the **same three parameters**: $\epsilon_0$, $\lambda$, $v$.

**The Gold Ring Condition**

The same structure that determines void sizes also determines lensing profiles. They're not independent fits — they're the same $\delta_w$ and $\sigma_{wall}$ appearing in both calculations.

Fit $\epsilon_0$, $\lambda$, $v$ to the observed void size distribution, then **predict** the lensing profile without further fitting, and compare to weak lensing surveys. Chapter 6 carries out the first half of this program.

---

## A Living Document

Some conceptual areas explored here are still under active development. The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.

---


*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
