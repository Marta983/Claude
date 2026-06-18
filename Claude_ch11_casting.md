<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 11 — Casting Mechanics and Spiral Seeding

---

## Section 15: The Casting Mechanism — Formal Derivation

### 15.1 Motivation and Scope

Chapter 10 established qualitatively that ejected material from a rotating, magnetized node follows spiral electromagnetic paths rather than radial ones, and that the geometry of what gets deposited in the surrounding medium is therefore inherited from the progenitor's field structure. This section derives that geometry formally.

The results are:

1. The trajectory of a charged, radiating particle ejected from a rotating magnetized node is a logarithmic spiral in the equatorial plane, with pitch angle determined by the ratio of initial kinetic energy to local magnetic energy density.

2. In the limit of maximum node rotation rate, the vertical extent of the deposition pattern collapses to a thin annular ring in the equatorial plane — a disk, not a sphere.

3. The deposition density profile in the equatorial plane follows a specific radial form that can be integrated to give the total seeding cross-section for a neighboring node.

4. The seeding cross-section connects directly to the nucleation length $r_{nuc}$ from Chapter 4, closing the loop between the casting mechanics and the vacancy field formalism.

---

### 15.2 The Trajectory Equation

Consider a charged particle of mass $m$, charge $q$, ejected from the node surface at radius $R_0$ with initial velocity $v_0$ in the equatorial plane. The node has surface magnetic field $B_0$, dipole geometry, and rotation rate $\Omega$.

In the equatorial plane the dipole field is purely vertical (perpendicular to the plane):

$$\mathbf{B}(r) = B_0 \left(\frac{R_0}{r}\right)^3 \hat{z}$$

The Lorentz force on the ejected particle:

$$\mathbf{F}_{L} = q\mathbf{v} \times \mathbf{B}$$

deflects the radial velocity into the azimuthal direction. Simultaneously, the particle loses energy through synchrotron radiation at the Larmor rate:

$$-\frac{dE}{dt} = \frac{q^4 B^2 v^2}{6\pi \epsilon_0 m^2 c^3} = \frac{\sigma_T c B^2 \gamma^2 \beta^2}{6\pi} \cdot \frac{q^2}{m^2}$$

where $\sigma_T$ is the Thomson cross-section and $\gamma$, $\beta$ are the usual relativistic factors. In the non-relativistic limit ($\beta \ll 1$):

$$-\frac{dE}{dt} = \frac{q^4 B(r)^2 v^2}{6\pi \epsilon_0 m^2 c^3}$$

The combined effect of Lorentz deflection and energy loss produces a spiral. In polar coordinates $(r, \theta)$ in the equatorial plane, the trajectory satisfies:

$$\frac{dr}{d\theta} = \frac{v_r}{v_\theta} \cdot r$$

where $v_r$ and $v_\theta$ are the radial and azimuthal velocity components. The Lorentz force converts radial momentum to azimuthal momentum at a rate proportional to $B(r)$, while synchrotron losses drain the total kinetic energy.

**The pitch angle** $\psi$ of the spiral — the angle between the trajectory and a circle centered on the node — evolves as:

$$\tan\psi(r) = \frac{v_r(r)}{v_\theta(r)} = \tan\psi_0 \cdot \exp\left(-\int_{R_0}^{r} \frac{qB(r')}{mv(r')} dr'\right)$$

where $\psi_0$ is the initial pitch angle at ejection (purely radial ejection gives $\psi_0 = \pi/2$).

Substituting the dipole field $B(r) = B_0(R_0/r)^3$:

$$\tan\psi(r) = \tan\psi_0 \cdot \exp\left(-\frac{qB_0 R_0^3}{mv_0}\int_{R_0}^{r} \frac{dr'}{r'^3}\right) = \tan\psi_0 \cdot \exp\left(-\frac{qB_0 R_0}{2mv_0}\left(1 - \frac{R_0^2}{r^2}\right)\right)$$

Define the **magnetic winding parameter**:

$$\mathcal{W} = \frac{qB_0 R_0}{2mv_0}$$

Then:

$$\tan\psi(r) = \tan\psi_0 \cdot e^{-\mathcal{W}(1 - R_0^2/r^2)}$$

For $r \gg R_0$:

$$\tan\psi(\infty) = \tan\psi_0 \cdot e^{-\mathcal{W}}$$

Large $\mathcal{W}$ — strong field or slow ejecta — winds the spiral tight. Small $\mathcal{W}$ — weak field or fast ejecta — leaves the trajectory nearly radial.

---

### 15.3 Maximum Flattening: The Thin Disk Limit

The vertical extent of the deposition pattern is controlled by the competition between the node's rotation rate $\Omega$ and the magnetic pressure in the vertical direction.

The centrifugal acceleration at radius $r$ in the equatorial plane:

$$a_{cent}(r) = \Omega^2 r$$

The magnetic restoring force per unit mass in the vertical direction for a displaced particle:

$$a_{mag,z}(r, z) \approx \frac{q^2 B(r)^2}{m^2 c^2} \cdot z = \omega_c(r)^2 \cdot z$$

where $\omega_c(r) = qB(r)/mc$ is the local cyclotron frequency.

The vertical equilibrium condition — the disk scale height $H(r)$ — balances these:

$$H(r) = \frac{v_{th}}{\omega_c(r)}$$

where $v_{th}$ is the thermal velocity of the ejected material. Maximum flattening occurs when $\Omega \gg \omega_c$ everywhere in the deposition zone, so that centrifugal effects dominate and $H(r) \to 0$. In this limit all deposited material lies in the equatorial plane and the three-dimensional deposition pattern collapses to a two-dimensional annular distribution.

**We adopt this limit throughout the remainder of this chapter**, consistent with the instruction to take the flattest possible toroid. The deposition geometry is then fully described by a radial surface density profile $\Sigma(r)$ in the equatorial plane.

---

### 15.4 The Deposition Profile

The surface density of deposited material $\Sigma(r)$ is determined by integrating the flux of escaping particles over the spiral trajectory family, weighted by the escape fraction $\epsilon'(\xi)$ from Chapter 8.

Each particle ejected at velocity $v_0$ from the node surface follows a spiral that reaches a maximum radius before synchrotron losses bring it to rest. The maximum radius $r_{max}(v_0)$ is found by integrating the energy loss equation:

$$\int_{R_0}^{r_{max}} \frac{m v \, dv}{dE/dr} \, dr = 0$$

Using the dipole field and non-relativistic Larmor formula:

$$r_{max}(v_0) = R_0 \left(1 + \frac{3\pi \epsilon_0 m^2 c^3 v_0^2}{q^4 B_0^2 R_0^2}\right)^{1/2}$$

Define the **magnetic stopping length**:

$$\ell_B = R_0 \sqrt{\frac{3\pi \epsilon_0 m^2 c^3}{q^4 B_0^2}} \cdot v_0$$

Then $r_{max} = R_0\sqrt{1 + (\ell_B/R_0)^2}$.

The surface density of deposited material at radius $r$ is proportional to the number of spiral trajectories that reach $r$ and deposit there:

$$\Sigma(r) = \Sigma_0 \cdot \frac{R_0}{r} \cdot \frac{1}{\tan\psi(r)} \cdot f_{esc}(r)$$

where $f_{esc}(r)$ is the fraction of ejected particles that reach radius $r$ before losing all kinetic energy, and the $R_0/r$ factor accounts for the geometric dilution of the spiral flux.

For the Maxwell-Boltzmann distribution of ejection velocities with mean $\bar{v}_0$:

$$f_{esc}(r) = \text{erfc}\left(\sqrt{\frac{r^2 - R_0^2}{\ell_B^2(\bar{v}_0)}}\right)$$

The full deposition profile is therefore:

$$\boxed{\Sigma(r) = \Sigma_0 \cdot \frac{R_0}{r} \cdot e^{\mathcal{W}(1-R_0^2/r^2)} \cdot \text{erfc}\left(\frac{\sqrt{r^2-R_0^2}}{\ell_B}\right)}$$

This profile has three regimes:

- **Near zone** ($r \sim R_0$): $\Sigma \approx \Sigma_0$ — dense deposition close to the node
- **Intermediate zone** ($R_0 \ll r \ll \ell_B$): $\Sigma \propto r^{-1} e^{\mathcal{W}}$ — power law fall-off modulated by spiral winding
- **Far zone** ($r \gg \ell_B$): $\Sigma$ drops exponentially — particles cannot reach here

---

### 15.5 The Seeding Cross-Section

A neighboring node at distance $d$ from the casting node captures all material deposited within its gravitational catchment radius $r_{catch}$. The catchment radius is determined by the condition that the escape velocity from the neighboring node equals the drift velocity of the interstitial material:

$$r_{catch} = \sqrt{\frac{2GM_{neighbor}}{v_{drift}^2}}$$

where $v_{drift}$ is the characteristic velocity of cast material at distance $d$.

The seeding cross-section — the total mass delivered to the neighboring node per eruption cycle — is:

$$\dot{M}_{seed} = \int_{d - r_{catch}}^{d + r_{catch}} \Sigma(r) \cdot v_{drift}(r) \cdot 2\pi r \, dr$$

In the limit $r_{catch} \ll d$ (neighboring node small compared to separation):

$$\dot{M}_{seed} \approx \Sigma(d) \cdot v_{drift}(d) \cdot \pi r_{catch}^2$$

This is the standard gravitational focusing formula, with $\Sigma(d)$ given by the deposition profile derived above.

**Connection to $r_{nuc}$:** The nucleation length from Chapter 4 sets the minimum void size — equivalently, the minimum separation at which two nodes can coexist without their vacancy fields merging. The effective minimum casting distance is therefore $d_{min} \sim r_{nuc}$. Nodes closer than $r_{nuc}$ are not independent — they share a vacancy field configuration and cannot be treated as separate casting sources.

The seeding cross-section evaluated at $d = r_{nuc}$:

$$\dot{M}_{seed,max} = \Sigma(r_{nuc}) \cdot v_{drift}(r_{nuc}) \cdot \pi r_{catch}^2$$

gives the **maximum possible seeding rate** — the rate for the closest independent neighbor. This is the quantity relevant to the JWST anomaly: an early-forming structure that appears too massive or too evolved for our event's timeline may have received $\dot{M}_{seed,max}$ from a neighboring node, effectively inheriting a head start.

---

### 15.6 Numerical Estimate

Using the Chapter 6 fitted parameters with $r_{nuc}(0) = 30$ Mpc/h and characteristic node mass $M_{node}$:

The magnetic winding parameter for a stellar-mass black hole aggregate:

$$\mathcal{W} \sim \frac{qB_0 R_0}{2mv_0} \sim 10^2 - 10^4$$

for typical neutron star surface fields ($B_0 \sim 10^8$ T) and escape velocities. This places cast material firmly in the **tight spiral** regime — ejecta wind many times around the node before escaping to large radii. The deposition ring is narrow and well-defined.

The magnetic stopping length:

$$\ell_B \sim 1 - 10 \text{ Mpc/h}$$

for typical ejection velocities, placing the bulk of the deposition well within the void interior but short of the neighboring node at $r_{nuc} = 30$ Mpc/h. Most cast material is deposited in the interstitial medium, with a small fraction reaching neighboring nodes directly — consistent with the slow Anulus-scale redistribution described in Chapter 7.

---

### 15.7 Summary of New Results

| Result | Expression | Significance |
|---|---|---|
| Spiral pitch angle | $\tan\psi(r) = \tan\psi_0 \cdot e^{-\mathcal{W}(1-R_0^2/r^2)}$ | Trajectory fully determined by $\mathcal{W}$ |
| Magnetic winding parameter | $\mathcal{W} = qB_0R_0/2mv_0$ | Single parameter governing spiral tightness |
| Thin disk limit | $H(r) \to 0$ as $\Omega \to \infty$ | Maximum flattening collapses deposition to equatorial annulus |
| Deposition profile | $\Sigma(r) \propto r^{-1} e^{\mathcal{W}(1-R_0^2/r^2)} \cdot \text{erfc}(\sqrt{r^2-R_0^2}/\ell_B)$ | Three-regime radial profile, no free parameters beyond $\mathcal{W}$ and $\ell_B$ |
| Seeding cross-section | $\dot{M}_{seed} \approx \Sigma(d) \cdot v_{drift} \cdot \pi r_{catch}^2$ | Standard gravitational focusing on the spiral deposition profile |
| Minimum casting distance | $d_{min} \sim r_{nuc}$ | Set by vacancy field nucleation length — closes loop to Chapter 4 |
| JWST connection | $\dot{M}_{seed,max}$ at $d = r_{nuc}$ | Quantifies inherited head start for anomalously evolved early structures |

The casting mechanism is now formally grounded in the same three parameters $(\epsilon_0, \lambda, v)$ that anchor the rest of the framework — plus the magnetic winding parameter $\mathcal{W}$, which is a property of the node's electromagnetic structure and in principle independently observable from the pitch angles of spiral galaxies in the vicinity of the casting node.

---

## A Living Document

Some conceptual areas explored here are still under active development. The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
