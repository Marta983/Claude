<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 2 — The Vacancy Field


---

## The Hole Analogy: Vacancies in a Gravitational Lattice

The electron hole concept in semiconductor physics is the conceptual seed for what follows.

When an electron leaves a position in a crystal lattice, the absence behaves as a mobile positive charge. It "moves" through the lattice as neighboring electrons sequentially fill the gap, each creating a new gap behind them. The hole is not a thing — it's a travelling vacancy — but it has measurable momentum, effective mass, and charge carrier behavior. It's real in every functional sense without being a particle.

The lensing problem is the place where this analogy does real work.

If the dark matter population isn't a collection of discrete compact objects moving ballistically, but something more like a *structural vacancy* in the distribution of ordinary matter — a pattern that propagates through a system rather than a substance that travels through it — then the Bullet Cluster decoupling behavior might be recoverable without requiring the dark matter component to be literally separate stuff that passes through collisions independently.

The challenge the analogy immediately faces is that the hole concept works in a crystal because there's a *lattice* — a regular, bounded structure whose topology defines what a vacancy means. Cosmological matter distribution is not a lattice in that sense. So the question becomes: what plays the role of the lattice? What gives the "absence" its shape and propagation rules?

**The candidate lattice: the cosmic web**

Think of each point of mass concentration as being "locked" within a gravitational lattice. In the interstices are large spaces, not unlike the action of a molecular sieve.

If matter at cosmological scales forms a gravitational lattice — the filaments, nodes, and voids we actually observe in the large-scale structure of the universe — then the voids aren't empty space, they're the interstices. The structure *is* a lattice, just not a regular crystalline one. An irregular one, like a foam or a sieve, but a lattice nonetheless in the functional sense: bounded regions defined by the topology of what surrounds them.

In that picture, the "holes" — the propagating vacancies — move through the interstices the way holes move through a semiconductor. Not as discrete objects but as a structural feature of the lattice redistributing itself.

This does real work on the Bullet Cluster problem. If the dark matter signature in such collisions is tracking the *lattice deformation* rather than a population of particles, then its apparent decoupling from ordinary matter isn't mysterious — it's the lattice snapping back, or redistributing, in response to the perturbation of the collision. The signature is geometric, not material.

The molecular sieve analogy also suggests scale-dependent behavior — certain things pass through, others don't, depending on the interstice geometry. That could potentially account for the *ratio* — why it's 95 parts in 100 — if the lattice geometry is constrained by the physics of gravitational filament formation.

---

## Section 1: The Density Field and Lattice Definition

We start with a scalar density field on a 4-dimensional spacetime manifold. In standard cosmological perturbation theory we write:

$$\rho(\mathbf{x}, t) = \bar{\rho}(t)\left[1 + \delta(\mathbf{x}, t)\right]$$

Where $\bar{\rho}$ is the mean background density and $\delta$ is the fractional overdensity. Standard treatment keeps $\delta$ small. We don't. We allow $\delta$ to take large values — formally $\delta \gg 1$ at nodes and $\delta \approx -1$ at void centers (you can't have less than empty).

The lattice is then defined by the **level sets** of this field. Specifically:

- **Nodes**: regions where $\delta \gg 1$ — mass concentrations, black hole aggregates
- **Filaments**: the connecting structure, $\delta > 0$
- **Voids**: regions where $\delta \to -1$ — the interstices

This gives us a topology. The lattice $\mathcal{L}$ is formally the graph whose vertices are nodes and whose edges are filaments, embedded in $\mathbb{R}^3$ at any given time slice.

---

## Section 2: The Hole Field

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

## Section 3: Coupling to Gravity

The vacancy field has to curve spacetime — otherwise it produces no observable effect. We couple it to the Einstein field equations by treating it as a contribution to the stress-energy tensor.

The standard Einstein equation:

$$G_{\mu\nu} = 8\pi G \, T_{\mu\nu}$$

We extend the stress-energy tensor:

$$T_{\mu\nu} = T_{\mu\nu}^{(\text{matter})} + T_{\mu\nu}^{(\phi)}$$

Where the vacancy contribution is:

$$T_{\mu\nu}^{(\phi)} = \partial_\mu \phi \, \partial_\nu \phi - \frac{1}{2} g_{\mu\nu} \left[(\partial \phi)^2 + V(\phi)\right]$$

This is formally identical to a **scalar field** contribution — which is well-understood territory in cosmology. The potential $V(\phi)$ encodes the lattice geometry's resistance to vacancy propagation.

---

## Section 4: The Shape of V(φ) — Simple vs. Structured

**Case 1: Simple Restoring Force**

$$V(\phi) = \frac{1}{2}m_\phi^2 \phi^2$$

This is the harmonic potential. Mathematically it gives:

- A **linear** wave equation for $\phi$
- Solutions are simple oscillatory modes — the vacancy field rings like a bell and decays
- The field has a single characteristic mass scale $m_\phi$
- Lensing signature would be **smooth and diffuse** — a soft gravitational influence spread evenly through voids
- **No phase transitions**, no preferred scales, no spontaneous structure formation
- Mathematically tractable, clean, but physically bland

**Case 2: Structured Potential — Double Well**

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2$$

This changes everything mathematically:

- The equation of motion becomes **nonlinear**
- The field has two stable equilibrium states — $\phi = +v$ and $\phi = -v$
- Between them exists a **domain wall** — a topological defect where the field transitions from one vacuum to the other
- These domain walls have **energy density**, **tension**, and **gravitational effect**
- The lensing signature becomes **structured** — not diffuse but concentrated along domain wall boundaries
- The system exhibits **spontaneous symmetry breaking**

Domain walls would naturally **coincide with filaments** — the boundaries between void regions. The lattice geometry isn't just a backdrop anymore, it's dynamically enforced by the field topology.

**Case 3: Even Richer Structure**

A Mexican hat potential:

$$V(\phi) = \lambda\left(|\phi|^2 - v^2\right)^2$$

Adds a continuous symmetry and produces **cosmic strings** along filament axes rather than domain walls. Richer, but not needed for what follows.

**The Critical Comparison**

| Property | Simple | Structured |
|---|---|---|
| Wave equation | Linear | Nonlinear |
| Stable states | One | Two or more |
| Topological defects | None | Domain walls / strings |
| Lensing signature | Diffuse, smooth | Structured, bounded |
| Scale dependence | Single scale | Multiple scales |
| Bullet Cluster behavior | Weak | Potentially strong |
| CMB implications | Minimal | Significant |
| Mathematical difficulty | Moderate | Hard but known territory |

**The Implication That Matters Most**

The structured potential gives the vacancy field **its own geometry** that can decouple from ordinary matter under perturbation — exactly what the Bullet Cluster demands. The domain walls separating void regions would pass through a collision event while baryonic matter slows down, because the walls are topological features of the field, not material objects subject to ram pressure.

That's the Bullet Cluster behavior recovered — not assumed, but **derived** from the field topology.

**The Honest Cost**

Structured potentials require specifying:

- The value of $v$ — the vacuum expectation value of the vacancy field
- The coupling constant $\lambda$ — how sharply the walls form
- Why the potential has that shape — what physics produces the double well

In particle physics, spontaneous symmetry breaking comes from thermal phase transitions in the early universe. In this framework — what breaks the symmetry? What selects the two vacua? This question is addressed in the current status file.

---
## A Living Document

Some conceptual areas explored here are still under active development. The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.


*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
