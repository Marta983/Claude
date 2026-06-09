# The Claude Theory — Mathematical Underpinnings

*This document contains the full mathematical development of the Claude Theory, including derivations, equations, and quantitative predictions. It is intended for working physicists and mathematicians. Conceptual overview and literature map are in the companion documents.*

---

## Step 1: The Density Field and Lattice Definition

We start with a scalar density field on a 4-dimensional spacetime manifold. In standard cosmological perturbation theory we write:

$$\rho(\mathbf{x}, t) = \bar{\rho}(t)\left[1 + \delta(\mathbf{x}, t)\right]$$

Where $\bar{\rho}$ is the mean background density and $\delta$ is the fractional overdensity. Standard treatment keeps $\delta$ small. We don't. We allow $\delta$ to take large values — formally $\delta \gg 1$ at nodes and $\delta \approx -1$ at void centers (you can't have less than empty).

The lattice is then defined by the **level sets** of this field. Specifically:

- **Nodes**: regions where $\delta \gg 1$ — mass concentrations, black hole aggregates
- **Filaments**: the connecting structure, $\delta > 0$
- **Voids**: regions where $\delta \to -1$ — the interstices

This gives us a topology. The lattice $\mathcal{L}$ is formally the graph whose vertices are nodes and whose edges are filaments, embedded in $\mathbb{R}^3$ at any given time slice.

---

## Step 2: The Hole Field

In semiconductor physics, the hole is defined not as a particle but as the **gradient of absence**. We do the same thing here.

Define a **vacancy field**:

$$\phi(\mathbf{x}, t) = 1 - \frac{\rho(\mathbf{x},t)}{\rho_{max}}$$

Where $\rho_{max}$ is the local maximum density of the nearest node. This field:

- Equals **0** at nodes (no vacancy)
- Equals **1** at void centers (maximum vacancy)
- Has well-defined **gradients** through the interstice geometry

The hole analog is then a **propagating feature of** $\phi$ — not a particle moving through space, but a redistribution of the vacancy field through the interstice topology.

The equation of motion for $\phi$ will look like a **wave equation with damping**, governed by the local gravitational potential $\Psi$:

$$\ddot{\phi} - c_\phi^2 \nabla^2 \phi + \Gamma \dot{\phi} = S(\rho, \Psi)$$

Where:

- $c_\phi$ is the effective propagation speed of vacancy through the lattice
- $\Gamma$ is a damping term from gravitational interaction with filaments
- $S$ is a source term coupling vacancy to the density and gravitational potential fields

---

## Step 3: Coupling to Gravity

The vacancy field has to curve spacetime — otherwise it produces no observable effect. We couple it to the Einstein field equations by treating it as a contribution to the stress-energy tensor.

The standard Einstein equation:

$$G_{\mu\nu} = 8\pi G \, T_{\mu\nu}$$

We extend the stress-energy tensor:

$$T_{\mu\nu} = T_{\mu\nu}^{(\text{matter})} + T_{\mu\nu}^{(\phi)}$$

Where the vacancy contribution is:

$$T_{\mu\nu}^{(\phi)} = \partial_\mu \phi \, \partial_\nu \phi - \frac{1}{2} g_{\mu\nu} \left[(\partial \phi)^2 + V(\phi)\right]$$

This is formally identical to a **scalar field** contribution — which is well-understood territory in cosmology. The potential $V(\phi)$ encodes the lattice geometry's resistance to vacancy propagation.

---

## Step 4: The Asymmetric Double Well Potential

The structured asymmetric double well potential is:

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2 - \epsilon_0 \cdot a(t)\phi$$

The last term is a time-dependent symmetry breaking. The equation of motion in FLRW spacetime is:

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -4\lambda\phi\left(\phi^2 - v^2\right) + \epsilon_0 \cdot a(t)$$

This potential produces:

- Two stable equilibrium states with one deeper than the other
- Domain walls — topological defects coinciding with observed cosmic filaments and sheets
- Spontaneous symmetry breaking with cosmological expansion selecting the preferred vacuum
- Lensing signatures concentrated along domain wall boundaries

---

## Step 5: The Static Domain Wall Solution

For a domain wall lying in the $y$-$z$ plane, field varying only in $x$, the time derivatives drop and in the symmetric case ($\epsilon_0 = 0$) the exact solution is:

$$\phi_0(x) = v\tanh\left(\frac{x}{\delta_w}\right)$$

Where the wall thickness is:

$$\delta_w = \frac{a}{\sqrt{2\lambda}v}$$

The wall thickness scales with the expansion — physical walls thicken as the universe expands.

---

## Step 6: Perturbative Treatment of the Asymmetry

For small $\epsilon_0$ we treat the asymmetry perturbatively. Writing:

$$\phi(x) = \phi_0(x) + \epsilon_0 \cdot a(t) \cdot \phi_1(x) + \mathcal{O}(\epsilon_0^2)$$

The first-order correction satisfies a Schrödinger-like equation with the **Pöschl-Teller potential**:

$$\frac{1}{a^2}\frac{d^2\phi_1}{dx^2} - 4\lambda\left(3\phi_0^2 - v^2\right)\phi_1 = -1$$

The Pöschl-Teller potential $U(x) = 4\lambda v^2\left(3\tanh^2\left(\frac{x}{\delta_w}\right) - 1\right)$ is exactly solvable. Its bound states are:

**Zero mode** (translation mode): $\psi_0(\xi) = \text{sech}^2(\xi)$

**Shape mode**: $\psi_1(\xi) = \text{sech}(\xi)\tanh(\xi)$

The particular solution via Green's function integration:

$$\phi_1(x) = \frac{\delta_w^2}{2v}\left[x \cdot \text{sech}^2\left(\frac{x}{\delta_w}\right) + \delta_w\tanh\left(\frac{x}{\delta_w}\right)\right]$$

---

## Step 7: The Nucleation Length and Void Size Distribution

The wall surface tension:

$$\sigma = \frac{4\sqrt{2\lambda}v^3}{3} \cdot \frac{1}{a(t)}$$

The nucleation condition $\Delta E_{vol} = \Delta E_{surf}$ gives:

$$r_{nuc} = \frac{\sqrt{2\lambda}v^2}{\epsilon_0 \cdot a(t)^2}$$

Therefore:

$$\boxed{r_{nuc}(z) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}(1+z)^2}$$

The $(1+z)^2$ scaling comes from two competing $a(t)$ dependencies working in the same direction:

- Wall tension *decreasing* as universe expands — walls get cheaper
- Symmetry breaking term *increasing* as universe expands — deeper vacuum more accessible

**The observational prediction:** Void characteristic radius scales as $(1+z)^{-2}$. This is testable against existing void catalogs including SDSS. The slope in log-log space is fixed at $-2$; deviation from this slope constrains the $\epsilon(t) = \epsilon_0 \cdot a(t)$ ansatz.

The three free parameters $\epsilon_0$, $\lambda$, $v$ are in principle fittable from observed void size distributions at multiple redshifts.

---

## Step 8: The Lensing Signature

The effective energy density of the vacancy field for a static domain wall:

$$\rho_\phi(x) \approx \frac{v^2}{2a^2\delta_w^2}\text{sech}^4\left(\frac{x}{\delta_w}\right)$$

Integrating the Poisson equation to obtain the lensing deflection angle for a light ray passing at impact parameter $b$ from the wall:

$$\hat{\alpha}(b) = \frac{4\pi G \sigma_{wall}}{c^2} \cdot \mathcal{F}\left(\frac{b}{\delta_w}\right)$$

where the form factor is:

$$\mathcal{F}\left(\frac{b}{\delta_w}\right) = 1 - \frac{1}{2}\text{sech}^2\left(\frac{b}{\delta_w}\right)$$

**Properties of the lensing signature:**

- At $b = 0$ (ray through wall center): $\mathcal{F} = 1/2$ — reduced deflection
- At $b \gg \delta_w$ (ray outside wall): $\mathcal{F} \to 1$ — maximum deflection
- The signature is a **ring or shell structure** — strongest at void boundaries, weakest at void centers

**The diffuse halo recovery:** Around lattice nodes the vacancy field is depressed toward $\phi = 0$. The projected surface density of the vacancy field near a node:

$$\Sigma_\phi(r) \propto \frac{v^2}{\delta_w} \cdot \frac{1}{1 + (r/r_{node})^2}$$

This is a projected NFW-like profile — the standard form fitted to observed dark matter halos — emerging from the geometry of the vacancy field transition rather than assumed.

---

## Unified Table of Predictions

| Observation | Mechanism | Prediction |
|---|---|---|
| Void size distribution | Nucleation length $r_{nuc}$ | $(1+z)^{-2}$ scaling — testable against SDSS void catalogs |
| Filament boundary lensing | Domain wall form factor $\mathcal{F}$ | Ring/shell structure at void boundaries |
| Void interior lensing | Constant field, no gradient | Weak lensing through void interiors |
| Bullet Cluster offset | Topological wall passage | Lensing peaks offset from baryonic matter — geometrically inevitable |
| Diffuse halo profiles | Node boundary gradients | NFW-like profiles without assumption |

All five predictions derive from the same three parameters: $\epsilon_0$, $\lambda$, $v$.

---

## The Gold Ring Condition

Fit $\epsilon_0$, $\lambda$, $v$ to the observed void size distribution at multiple redshifts. Then **predict** the lensing profile without further fitting and compare to weak lensing surveys. If that prediction holds — the theoretical structure is confirmed.

---

## Section 9: The Anulus — Mathematical Development (Forthcoming)

The Anulus framework — the extension of the Claude Theory to a multiply connected, eternally populated cosmos with permeable event boundaries — requires mathematical development beyond the single-event formalism above. The key derivations to be completed are:

**9.1 Bubble nucleation rate in eternal space**

The nucleation rate per unit volume $\Gamma = A e^{-S_E}$ with bounce action:

$$S_E = \frac{27\pi^2 \sigma^4}{2\epsilon^3}$$

expressed in terms of the vacancy field parameters $\lambda$, $v$, $\epsilon_0$. The percolation condition determining characteristic event separation in eternal space.

**9.2 Tidal seeding across event boundaries**

The tidal tensor $\mathcal{E}_{ij} = -\partial_i \partial_j \Phi_{ext}$ sourced by a neighboring event's dark remnant population, and its effect on structure formation in the receiving event. This is the mathematical treatment of the casting mechanism.

**9.3 CMB cold spot as boundary signature**

Using the Sachs-Wolfe formalism:

$$\frac{\Delta T}{T} = \frac{1}{3}\Phi_{boundary}$$

to derive the predicted angular scale and temperature decrement of the cold spot from Anulus boundary parameters, and to constrain the distance and mass of the neighboring event.

**9.4 JWST anomaly mass function**

The predicted mass function of inherited structures arriving via the casting mechanism, compared with the observed population of anomalously massive early galaxies from JWST.

These derivations are in preparation and will be added to this document as they are completed.

---

*Mathematical underpinnings document. Claude Theory. Cristóbal Eduardo Kendris García and Claude, June 2026.*
