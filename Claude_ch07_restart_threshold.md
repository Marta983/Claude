<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory: Space Has Always Existed
## Chapter 7 — The Restart Threshold, Elastic Trigger, and Conserved Anulus

---

## Section 12: The Restart Threshold — A Bifurcation Condition on V(φ)

### 12.1 Setup

Problem 1 (the restart threshold, Claude_status.md) asks: at what accumulated field configuration does the eruption event fire? This section derives a closed-form threshold condition directly from the potential already fitted in Chapter 6, with no new field machinery.

Recall the asymmetric double-well potential from Chapters 2–4:

$$V(\phi) = \lambda(\phi^2 - v^2)^2 - \epsilon_0\, a(t)\,\phi$$

where $\lambda$, $v$, $\epsilon_0$ are bare constants of the potential itself. The $a(t)$-dependence of derived quantities such as $\delta_w(a)$ and $\sigma_{wall}(a)$ in Chapter 4 follows from these bare constants combined with $a(t)$ through the kinetic term — it is not a separate input. The bifurcation analysis below is therefore performed with the same bare constants fitted numerically in Chapter 6.

### 12.2 The Bifurcation Condition

Critical points of $V(\phi)$ satisfy $dV/d\phi = 0$:

$$4\lambda\phi(\phi^2 - v^2) - \epsilon_0\, a(t) = 0$$

This is a depressed cubic in $\phi$:

$$\phi^3 - v^2\phi - \frac{\epsilon_0\, a(t)}{4\lambda} = 0$$

For $\epsilon_0 a(t) = 0$ (the symmetric case), this cubic has three real roots — two minima at $\phi = \pm v$ and a maximum at $\phi = 0$: the double well. As $\epsilon_0 a(t)$ grows, the asymmetry deepens one minimum and shallows the other, until at a critical value the shallow minimum merges with the maximum and annihilates — the cubic transitions from three real roots to one. Beyond this point $V(\phi)$ is a single well: the field has only one stable configuration.

This is the restart condition: not a gradual deepening, but the abrupt disappearance of the configuration the field currently occupies.

The transition occurs where the cubic's discriminant vanishes. For a depressed cubic $\phi^3 + p\phi + q = 0$ with $p = -v^2$ and $q = -\epsilon_0 a(t)/(4\lambda)$, the discriminant is $\Delta = -4p^3 - 27q^2$. Setting $\Delta = 0$ and solving for the critical combination:

$$\boxed{\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}\,\lambda v^3}$$

At this point the two merging roots coincide at:

$$\phi_{crit} = \frac{v}{\sqrt{3}}$$

### 12.3 Numerical Evaluation Against the Chapter 6 Fit

Using $(\epsilon_0, \lambda, v) = (1.726\times10^{-3}, 0.1175, 0.3268)$ from Chapter 6:

$$\epsilon_0\, a(t)_{crit} = \frac{8\sqrt{3}}{9}(0.1175)(0.3268)^3 \approx 6.314\times10^{-3}$$

Compared to the fitted value $\epsilon_0 \approx 1.726\times10^{-3}$ at $a=1$, the ratio is:

$$\frac{a(t)_{crit}}{a(t)_{now}} \approx 3.658$$

and the merging field value is $\phi_{crit} = v/\sqrt{3} \approx 0.1887$ — between $\phi=0$ (node/accumulation state) and $\phi=v\approx0.327$ (void state).

### 12.4 Status and the Open Step

This is a closed-form threshold condition derived from parameters already fitted to observational data. What remains open: the ratio $a(t)_{crit}/a(t)_{now} \approx 3.658$ is dimensionless and its physical meaning is not yet established. Converting the ratio 3.658 into a timescale, or into a physically meaningful "how much further accumulation," requires identifying what clock governs the accumulated field across the full cycle. See Claude_status.md.

### 12.5 Note on the Dark Mass Accumulation Interpretation

The ratio $a_{crit}/a_{now} \approx 3.658$ was initially interpreted here
as a dark mass accumulation factor, explicitly flagged as pending
justification. That interpretation is superseded.

Chapter 12 provides a full derivation of the physical clock. The ratio
3.658 is a charge accumulation timescale — the cosmic expansion required
for a node to accumulate sufficient charge imbalance, through asymmetric
electromagnetic sorting in its Kerr geometry, to reach the classical
charge limit condition. See Chapter 12 for the complete derivation.

---

## Section 13: The Elastic Trigger, the Critical Mass Ratio, and the Conserved Anulus

### 13.1 Motivation and Scope

The preceding sections established the vacancy field framework, derived its three free parameters from SDSS void data, and identified the restart threshold as a bifurcation condition on $V(\phi)$. What remained open was the *physical mechanism* by which accumulation at a dormant node produces an eruption event — specifically, what determines the trigger, whether all eruptions share a common character, and what the long-run behavior of the Anulus looks like under the constraint that mass-energy is globally conserved.

This section addresses all three questions. The results are:

1. The originating point has an intrinsic elastic property inherited from its previous eruption. Infalling mass compresses it against a restoring pressure until a critical strain is reached and the stored energy releases catastrophically.

2. The trigger condition is not an absolute mass threshold but a **fixed dimensionless ratio** $\mathcal{R}_c = M_{infall}/M_{point}$ — a universal constant set by the elastic properties of space at the transition. This ratio-gating makes all eruptions **geometrically similar**: different in absolute scale, identical in their internal mass relationships.

3. The Anulus is a **conserved closed system**. Total mass-energy $M_{Anulus}$ is fixed and eternal. Every escaped fraction redistributes into interstitial space and eventually re-enters the cycle at other nodes. Nothing is created; nothing is destroyed.

4. Because the escaped fraction is never fully recovered at any given node, individual nodes **deflate slowly** across cycles — each eruption produces a slightly smaller universe than the last at that node. The Anulus as a whole trends toward increasing quietude over infinite time, not from thermodynamic entropy alone but from geometric mass redistribution.

---

### 13.2 Physical Dimensions of the Originating Point

In the Claude Theory the eruption event is a phase transition within eternal space — not a creation event. The originating point is therefore not a mathematical singularity but a physical region of space with a finite characteristic radius $R_0$ — its **equilibrium radius** between eruption cycles, when the accumulated field has settled and no net infall is occurring.

This is not an auxiliary assumption. It follows from the same field framework already in hand: the vacancy field $\phi$ has a nonzero wall thickness $\delta_w$, a finite nucleation length $r_{nuc}$, and a potential $V(\phi)$ with a well-defined spatial scale set by $(\epsilon_0, \lambda, v)$. A field theory with finite spatial scales cannot have a structureless point as its source. The originating point is the region where $\phi \to 0$ — the node in the lattice — and it has the geometry of a node: a compact region of radius $R_0$ within which the vacancy field is fully suppressed.

The equilibrium radius is set by the balance between the gravitational self-attraction of the accumulated node mass and the elastic restoring pressure of the field. At equilibrium:

$$P_{grav}(R_0) = P_{elastic}(R_0)$$

where the gravitational pressure at the node surface scales as $P_{grav} \sim G M_{point}^2 / R_0^4$ and the elastic restoring pressure is a property of the potential $V(\phi)$ evaluated at the node boundary.

---

### 13.3 Elastic Compression and the Restoring Force

As infalling mass accumulates at the node it compresses the region below $R_0$. Define the dimensionless **strain**:

$$\xi = \frac{R_0 - R}{R_0}$$

running from $\xi = 0$ (relaxed, no compression) to $\xi = 1$ (total collapse). For small to moderate strains the restoring pressure is linear — Hooke's law in spherical form:

$$P_{elastic}(\xi) = K \cdot \xi$$

where $K$ is the **bulk stiffness** of the node, with units of pressure. The stiffness is determined by the curvature of $V(\phi)$ at the node boundary, which is already fixed by $(\epsilon_0, \lambda, v)$:

$$K = \left.\frac{d^2 V}{d\phi^2}\right|_{\phi=0} \cdot \frac{1}{R_0} = 8\lambda v^2 \cdot \frac{1}{R_0}$$

The stored elastic energy at compression $\xi$ is:

$$E_{stored}(\xi) = \frac{1}{2} K \xi^2 \cdot \frac{4}{3}\pi R_0^3 = \frac{16\pi}{3}\lambda v^2 \xi^2 R_0^2$$

This is the energy available to seed the next eruption event — the initial energy budget of the new universe.

---

### 13.4 The Trigger Condition: A Universal Critical Ratio

Eruption occurs when the ram pressure of infalling mass equals the elastic restoring pressure at some critical strain $\xi_c$:

$$P_{infall}(R_c) = K \cdot \xi_c$$

Setting the two equal and substituting $R_c = R_0(1-\xi_c)$ and $K = 8\lambda v^2 / R_0$:

$$M_{infall} = \frac{32\pi\lambda v^2 R_0^3 \xi_c (1-\xi_c)^4}{G}$$

The **critical mass ratio** is therefore:

$$\boxed{\mathcal{R}_c = \frac{M_{infall}}{M_{point}} = \frac{24\lambda v^2 \xi_c (1-\xi_c)^4}{G \rho_{node}}}$$

This is a dimensionless constant. It depends only on $\lambda$, $v$, $\xi_c$, and $\rho_{node}$ — all properties of the field and its equilibrium configuration, not of the absolute scale of the node. The critical ratio $\mathcal{R}_c$ is **the same for every node in the Anulus**, regardless of absolute size.

---

### 13.5 Geometric Similarity of All Eruptions

The universality of $\mathcal{R}_c$ has an immediate structural consequence: all eruption events are **geometrically similar**.

Two nodes of different absolute mass fire at the same ratio $\mathcal{R}_c$. The two universes that result are identical in every **dimensionless ratio** — same ratio of dark remnants to luminous matter, same ratio of node mass to void mass, same $\mathcal{R}_c$ at their own eventual restart. They differ only in absolute scale.

**Implication for observability:** We cannot determine from within our own universe whether we are a large eruption or a small one. All internal ratios are identical across eruptions. The absolute scale of our event is in principle unobservable from inside it.

---

### 13.6 The Inherited Properties of Successive Cycles

Define the **escape fraction** $\epsilon'$ as the fraction of total eruption mass that permanently exits the node's gravitational catchment. The node mass obeys:

$$M_{point,n+1} \approx M_{point,n}(1 - \epsilon')$$

Over many cycles:

$$M_{point,n} = M_{point,0}(1-\epsilon')^n$$

Each successive eruption is smaller in absolute scale. Critically: $\mathcal{R}_c$ does not change. The ratio is a property of the field, not of absolute node mass. All cycles at this node are geometrically similar; they are simply scaled down from cycle to cycle.

---

### 13.7 The Conserved Anulus

The escaped fractions drift as dark remnants into the interstitial regions of the Anulus and eventually contribute to accumulation at neighboring nodes. The total mass-energy inventory of the Anulus is therefore **fixed**:

$$M_{Anulus} = \sum_i \left[ M_{point,i} + M_{active,i} + M_{interstitial,i} \right] = \text{const}$$

This conservation law follows from the foundational premise — space has always existed — combined with the absence of any creation mechanism. The Anulus is a **closed redistributive system**.

The consequences are precise:

**(i) The Anulus has always been active.** Some nodes are always firing. There was no quiet beginning.

**(ii) The number of nodes is finite.** Each active node requires a minimum mass $M_{point,min}$. Since $M_{Anulus}$ is fixed:

$$N_{max} \leq \frac{M_{Anulus}}{M_{point,min}}$$

**(iii) Our eruption is typical.** The ratio $\mathcal{R}_c$ is universal; the field parameters are universal. We are one instance of a generic process.

**(iv) The Anulus trends toward quietude.** Over infinite time the system tends toward a state where all mass-energy is distributed too thinly for any node to reach $\mathcal{R}_c$ — a **gravitational dilution death**: the same conserved inventory, too spread out to erupt.

---

### 13.8 The Long-Run Dynamics

Let $N(t)$ be the number of active nodes at Anulus time $t$ and $M_{inter}(t)$ the total interstitial mass. The coupled evolution equations are:

$$\dot{M}_{inter} = \epsilon' \sum_{i\,active} \dot{M}_{erupt,i} - \Gamma_{seed} M_{inter}$$

$$\dot{N} = \Gamma_{seed} \frac{M_{inter}}{M_{point,min}} - \Gamma_{exhaust} N$$

The system has no stable fixed point with $N > 0$ — it always trends toward $N \to 0$ asymptotically. The characteristic timescale for this approach to quietude:

$$T_{quiet} \sim \frac{1}{\epsilon' \Gamma_{exhaust}}$$

is vastly longer than any single eruption cycle.

**The Anulus arrow of time.** The slow deflation of individual nodes and the monotonic growth of interstitial mass provide an arrow of time at the Anulus scale independent of thermodynamic entropy within any single eruption event. The Anulus is not time-symmetric. It has a direction: from many large active events toward fewer smaller ones, tending asymptotically toward silence.

---

### 13.9 The Unobservability of $M_{Anulus}$ From Within a Single Cycle

All internal observables are set by $M_{point}$, $\mathcal{R}_c$, and $(\epsilon_0, \lambda, v)$. None carries information about how many other nodes exist or how much interstitial mass drifts between them. The only window onto the Anulus scale from within our event would be through casting — the gravitational influence of neighboring eruption events on our own structure formation. This remains Open Problem 3 and is the next analytical frontier of the Claude Theory.

---

### 13.10 Summary of New Results

| Result | Expression | Significance |
|---|---|---|
| Node stiffness | $K = 8\lambda v^2 / R_0$ | Derived from $V(\phi)$, no new parameters |
| Stored energy at trigger | $E_{stored} = \frac{16\pi}{3}\lambda v^2 \xi_c^2 R_0^2$ | Initial energy budget of each eruption |
| Critical mass ratio | $\mathcal{R}_c = 24\lambda v^2 \xi_c(1-\xi_c)^4 / G\rho_{node}$ | Universal, dimensionless, geometry-fixing |
| Cycle deflation | $M_{point,n} = M_{point,0}(1-\epsilon')^n$ | Monotonic, irreversible at node level |
| Conservation law | $M_{Anulus} = \text{const}$ | Follows from eternal space + no creation mechanism |
| Anulus arrow of time | $dM_{inter}/dt > 0$ in early Anulus | Independent of thermodynamic entropy |
| Far future | $N \to 0$, gravitational dilution | Asymptotic, not sudden |

---
## A Living Document

Some conceptual areas explored here are still under active development. The current status of open problems and unresolved assumptions is maintained in [Claude_status.md]. Readers are directed there for the most current picture.

---

*The Claude Theory: Space Has Always Existed — conceived and developed by Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
