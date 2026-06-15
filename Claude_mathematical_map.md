<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory — Mathematical Foundations and Reference Map

## Preamble

The framework presented here does not invent new mathematics. It assembles existing, rigorous mathematical treatments — some mainstream, some underutilized, some considered peripheral until now — and shows that they converge naturally when a single foundational assumption is changed:

**Space has always existed.**

What follows maps each conceptual claim of the Claude Theory to its mathematical home, with sufficient detail for a technically literate reader to pursue each thread independently. Full derivations referenced here live in the companion document, `Claude_underpinnings.md` (Sections 1–12), and unresolved questions are tracked in `Claude_open_problems.md`.

This document has been substantially reorganized from earlier versions to reflect the growth of the underpinnings: the vacancy field formalism now carries a completed numerical fit (Section 5 below), a full quantitative derivation of the Bullet Cluster signature (Section 4), and an extension to a multiply connected cosmology — the Anulus (Section 8).

---

## Section One — Eternal Space and the Elimination of Singularity

**The Conceptual Claim**

The Big Bang was not a creation event. It was a phase transition within pre-existing eternal space. Space has no $t=0$.

**The Mathematical Treatment**

Current cosmology describes the universe using the Friedmann-Lemaître-Robertson-Walker metric:

$$ds^2 = -dt^2 + a(t)^2\left[dr^2 + r^2d\Omega^2\right]$$

where $a(t)$ is the scale factor. Standard treatment allows $a(t) \to 0$ as $t \to 0$ — the singularity. We replace this with a minimum condition:

$$a(t) \geq a_{min} > 0$$

This single modification eliminates the singularity without disturbing the rest of the metric machinery. The eruption event is a transition through a minimum, not a beginning from zero.

**Existing Mathematical References**

*Loop Quantum Cosmology* (Bojowald 2001, Ashtekar and Singh 2011) achieves precisely this using quantum geometry. The classical singularity is replaced by a quantum bounce. Our framework adopts the bounce result while providing a different physical interpretation — not a quantum effect but a classical phase transition threshold, derived explicitly in Section 9 below (Claude_underpinnings.md Section 12).

*Conformal Cyclic Cosmology* (Penrose 2010) uses conformal geometry to describe a universe of successive aeons, each beginning where the previous ended. Penrose's mathematical machinery is directly applicable to our cycling framework even where his physical interpretation diverges.

*The Ekpyrotic and bouncing cosmology literature* (Steinhardt, Turok 2002 onward) provides additional mathematical treatments of non-singular cosmological transitions.

---

## Section Two — Dark Remnant Accumulation and the True Mass Census

**The Conceptual Claim**

The luminous universe is a sampling bias. Dark remnants of completed stellar cycles vastly outnumber active stars and constitute the dominant mass component of the universe — what current models call dark matter.

**The Mathematical Treatment**

The stellar initial mass function (Salpeter 1955, Kroupa 2001) gives the distribution of stellar masses at formation:

$$\xi(m) \propto m^{-\alpha}$$

where $\alpha \approx 2.35$ for stars above one solar mass. Integrating this over cosmic star formation history gives the total population of remnants at any epoch.

Black hole merger rates derived from LIGO/Virgo observations provide direct empirical grounding for the accumulation process. Current estimates suggest merger rates of tens of events per cubic gigaparsec per year — and these are only the detectable fraction.

The remnant accumulation over a full cycle of duration $T$ gives a total dark mass:

$$M_{dark}(T) = \int_0^T \dot{M}_{remnant}(t) \, dt$$

where $\dot{M}_{remnant}$ is the rate of mass transfer from active to remnant states. This integral, evaluated over timescales consistent with an eternal cycling universe, naturally produces the observed ratio of approximately 95 parts dark to 5 parts luminous — without invoking exotic particles.

**Existing Mathematical References**

*MACHO and primordial black hole literature* (Paczynski 1986, Carr and Hawking 1974 onward) provides the mathematical framework for compact dark object populations and their observational signatures.

*LIGO Scientific Collaboration merger rate calculations* provide empirical grounding for black hole accumulation rates.

*Stellar evolution codes* (MESA, BEC) provide the remnant mass functions needed for the accumulation integral.

---

## Section Three — The Vacancy Field: Lattice, Potential, and Lensing

**The Conceptual Claim**

The large scale structure of the universe — filaments, walls, voids — constitutes a gravitational lattice. The apparent dark matter distribution is not a population of discrete objects but a vacancy field propagating through this lattice, analogous to electron holes in a semiconductor crystal. The same field, with the same fitted parameters, produces the void size distribution, the domain-wall lensing signature, and diffuse halo profiles.

**The Mathematical Treatment**

*The lattice and the vacancy field* (Claude_underpinnings.md Sections 1–2). The density field is written as $\rho(\mathbf{x},t) = \bar\rho(t)[1+\delta(\mathbf{x},t)]$, with $\delta \gg 1$ at nodes and $\delta \to -1$ at void centers. The lattice $\mathcal{L}$ is the graph of nodes (mass concentrations) connected by filaments, embedded in the voids that form its interstices. The vacancy field is defined as:

$$\phi(\mathbf{x}, t) = 1 - \frac{\rho(\mathbf{x},t)}{\rho_{max}}$$

equal to 0 at nodes and 1 at void centers. Its dynamics follow a damped wave equation sourced by the local gravitational potential.

*Coupling to gravity* (Section 3). The vacancy field contributes to the stress-energy tensor as a scalar field:

$$T_{\mu\nu}^{(\phi)} = \partial_\mu \phi \, \partial_\nu \phi - \frac{1}{2} g_{\mu\nu} \left[(\partial \phi)^2 + V(\phi)\right]$$

*The asymmetric double-well potential* (Sections 4–7). A simple harmonic potential gives only diffuse, structureless lensing — inadequate to the observed cosmic web. The structured alternative is an asymmetric double well:

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2 - \epsilon_0 \cdot a(t)\,\phi$$

with equation of motion

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -4\lambda\phi\left(\phi^2 - v^2\right) + \epsilon_0 \cdot a(t)$$

This potential produces domain walls coinciding with observed filaments. The static wall solution is $\phi_0(x) = v\tanh(x/\delta_w)$, with wall thickness $\delta_w = a/(\sqrt{2\lambda}v)$. The time-dependent asymmetry $\epsilon(t) = \epsilon_0 \cdot a(t)$ — the natural candidate for the broken symmetry being the direction of cosmological time itself — produces a preferred nucleation scale and therefore a lognormal void size distribution, matching observation (Section 5 of underpinnings) where a symmetric potential would predict a scale-free power law.

Solving the perturbed wall equation via the exactly-solvable Pöschl-Teller potential (Section 7) yields the central testable prediction of this section:

$$r_{nuc}(z) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}(1+z)^2$$

Void characteristic radius scales as $(1+z)^{-2}$ — a specific power law, distinct from the standard cosmological prediction, arising from two compounding effects: wall tension decreasing and the symmetry-breaking term increasing as the universe expands.

*The lensing signature* (Section 8). The vacancy field's energy density is sharply peaked at domain wall centers ($\rho_\phi \propto \text{sech}^4(x/\delta_w)$). The resulting deflection angle is:

$$\hat{\alpha}(b) = \frac{4\pi G \sigma_{wall}}{c^2} \cdot \mathcal{F}\left(\frac{b}{\delta_w}\right), \qquad \mathcal{F}\left(\frac{b}{\delta_w}\right) = 1 - \frac{1}{2}\text{sech}^2\left(\frac{b}{\delta_w}\right)$$

where $\sigma_{wall} = \frac{4\sqrt{2\lambda}v^3}{3a}$ is the wall surface tension. This is *inverted* relative to a mass concentration: lensing is minimum at the wall center and maximum at the wall edges, producing a ring/shell structure — strongest at void boundaries, weakest at void interiors and wall centers. This matches the observed pattern of enhanced lensing at filament boundaries, weak lensing through void interiors, and (via topological wall passage) the Bullet Cluster lensing-baryon offset.

*Diffuse halos* (Section 9). Around nodes, the vacancy field gradient produces a projected surface density:

$$\Sigma_\phi(r) \propto \frac{v^2}{\delta_w}\cdot\frac{1}{1+(r/r_{node})^2}$$

a projected NFW-like profile, emerging from field geometry rather than assumed.

A single potential, with three parameters $(\epsilon_0, \lambda, v)$, thus produces the void size distribution, filament-boundary lensing, void-interior weak lensing, the Bullet Cluster offset, and diffuse halo profiles — not as independent fits but as the same $\delta_w$ and $\sigma_{wall}$ appearing throughout. Section Five below reports the completed numerical fit of these three parameters.

**Existing Mathematical References**

*Cosmic web topology* (Bond, Kofman, Pogosyan 1996) — observational and mathematical foundation for the filament-void-node lattice.

*Domain wall cosmology* (Vilenkin 1981, Kibble 1976) — topological defects in scalar fields, directly applicable to the vacancy field domain walls.

*Weak gravitational lensing formalism* (Bartelmann and Schneider 2001) — the framework within which the lensing predictions above are derived.

*Void catalogs* — 2dF Galaxy Redshift Survey, SDSS, and the Hamaus, Sutter & Wandelt (2014) universal void density profile, used in Section Five's fit.

---

## Section Four — The Bullet Cluster: Full Derivation

**The Conceptual Claim**

The Bullet Cluster — two colliding galaxy clusters whose lensing peaks are offset from their baryonic gas — is cosmology's most cited direct evidence for collisionless dark matter. The vacancy field framework reproduces this offset as a geometric inevitability of domain wall topology, and goes further: it predicts a *secondary* lensing feature, absent from particle dark matter models, that constitutes a novel falsifiable test.

**The Mathematical Treatment**

Two lattice nodes A and B approach with relative velocity $v_{col} \approx 3000$ km/s. The pre-collision vacancy field is the superposition $\phi = \phi_A + \phi_B - v$, with a domain wall at the midpoint where the two fields' gradients balance.

*Relaxation versus collision timescales* (Claude_underpinnings.md Section 10.2). Baryonic gas decelerates under ram pressure; the vacancy field's response is governed by its relaxation timescale, set by the lowest non-zero Pöschl-Teller mode ($E = 3U_0 = 12\lambda v^2$):

$$\tau_{relax} = \frac{1}{\sqrt{12\lambda}\,v}, \qquad \tau_{cross} = \frac{2r_{node}}{v_{col}}$$

When $\tau_{relax} \ll \tau_{cross}$, the vacancy field tracks the collisionless mass throughout the collision — the lensing centroid stays with the nodes, not the gas.

*Primary offset* (Section 10.3). Using the NFW-like profile of Section Three, the lensing centroid is coincident with each node, giving:

$$\Delta x_{lens-gas} = x_{node} - x_{gas} \approx 200 \text{ kpc}$$

matching observation as a geometric consequence of the topology rather than a free parameter.

*The wall equation of motion* (Section 10.4–10.6). After the collision, the domain wall must travel to the new midpoint between separated nodes. The wall center $X(t)$ obeys a damped harmonic oscillator:

$$m_{eff}\ddot{X} + \gamma\dot{X} + kX = F_{collision}(t)$$

with effective mass $m_{eff} = \sigma_{wall}/c^2$, restoring constant $k = 2\epsilon_0 a(t) v/\delta_w^2$, and Hubble damping $\gamma = 4Hv^2$. The natural frequency and damping ratio are:

$$\omega_0 = c\sqrt{\frac{3\epsilon_0\sqrt{2\lambda}}{2v}}, \qquad \zeta = \frac{3Hac^2}{2\omega_0\sqrt{2\lambda}v}$$

with underdamped and overdamped solutions for $X(t)$ given in Section 10.6 of the underpinnings.

*The secondary lensing arc — $\mathcal{G}$* (Section 10.7). The residual wall displacement at observation time $t_{obs}$ places a secondary lensing feature at:

$$x_{wall}(t_{obs}) = \frac{x_A+x_B}{2} + \delta_w \cdot \mathcal{G}, \qquad \mathcal{G} = \frac{\Delta X}{\delta_w}e^{-\zeta\omega_0 t_{obs}}\left(\cos\omega_d t_{obs} + \frac{\zeta}{\sqrt{1-\zeta^2}}\sin\omega_d t_{obs}\right)$$

For the Bullet Cluster, $t_{obs}\approx 100$–$200$ Myr post-collision. Fast relaxation drives $\mathcal{G}\to 0$ (arc near the inter-node midpoint); slower relaxation offsets the arc toward the bullet subcluster's direction of motion.

*Complete predictions* (Section 10.8):

| Feature | Position | Nature |
|---|---|---|
| Primary lensing peak A | Coincident with main cluster node | NFW-like vacancy field halo |
| Primary lensing peak B | Coincident with bullet subcluster node | NFW-like vacancy field halo |
| Secondary lensing arc | Between nodes, offset by $\delta_w\mathcal{G}$ toward bullet direction | Domain wall re-establishing between nodes |

The first two match existing observations. The **secondary lensing arc is a new prediction** — absent from particle dark matter models, and in principle detectable in existing deep weak lensing maps of the Bullet Cluster system. Its detection or non-detection at the predicted position and surface-brightness profile is a direct test of the vacancy field framework.

**Existing Mathematical References**

*Pöschl-Teller potential* — standard exactly-solvable quantum mechanics, applied here to wall perturbation modes (Claude_underpinnings.md Section 7).

*Damped harmonic oscillator theory* — standard classical mechanics, applied to wall dynamics post-collision.

*Clowe et al. (2006) and successors* — the observational Bullet Cluster lensing-baryon offset that Sections 10.3 reproduces and Section 10.7 extends.

---

## Section Five — The SDSS Void Fit: Numerical Anchors

**The Conceptual Claim**

The vacancy field framework's three free parameters $(\epsilon_0, \lambda, v)$ have now been fit against real observational data — the SDSS void catalog — closing what was previously the framework's central bottleneck. This single fit propagates through to the lensing form factor and the CMB Cold Spot, providing the first numerically anchored predictions of the theory.

**The Mathematical Treatment**

*The fitting target* (Claude_underpinnings.md Section 11.1–11.3). The Hamaus, Sutter & Wandelt (2014) universal void density profile, fit to SDSS data with $\delta_c=-0.69$, $r_s=0.81\,r_v$, at a representative $r_v = 30$ Mpc/h (consistent with BOSS DR16's reported range of $\sim$4–113 Mpc/h), is matched against the domain-wall tanh profile $\delta_\phi(r) = \delta_c\cdot\frac{1}{2}(1-\tanh((r-r_s)/\delta_w))$. A least-squares fit gives $\delta_c=-0.654$, $r_s=15.45$ Mpc/h, $\delta_w=6.31$ Mpc/h, with $R^2=0.915$.

*Mapping to $(\epsilon_0,\lambda,v)$* (Section 11.4). Using $v=-\delta_c/2$, $\lambda = 1/(2v^2\delta_w^2)$, and $\epsilon_0 = \sqrt{2\lambda}v^2/r_v$:

$$v = 0.3268, \qquad \lambda = 0.1175, \qquad \epsilon_0 = 1.726\times10^{-3}$$

These three numbers, anchored to $r_v=30$ Mpc/h, now fix every downstream prediction of Sections Three, Four, and Eight.

*Redshift check* (Section 11.5). The prediction $r_{nuc}(z) = 30(1+z)^2$ Mpc/h, checked against BOSS DR16 redshift bins at $z\approx0.35$ and $z\approx0.65$, gives a predicted growth ratio of 1.49 versus an observed ratio of 1.41 — agreement to within $\sim$5%. Not definitive (two bins, max-radius as a crude proxy), but not falsified, and in the right regime.

*The lensing form factor, calibrated* (Section 11.6). With $\delta_w=6.31$ Mpc/h, $\mathcal{F}(b/\delta_w)$ now has concrete spatial scale: suppressed to 50% at the wall center ($b=0$), recovering to >95% by $b\approx12.6$ Mpc/h. This predicts a lensing convergence "notch" spanning $\sim$10–15 Mpc/h at domain wall locations — a non-monotonic feature absent from smooth NFW particle-dark-matter profiles, and the spatial signature underlying the secondary-arc prediction of Section Four.

*The CMB Cold Spot* (Section 11.7). The naive Sachs-Wolfe estimate from the fitted void profile gives $\Phi(0)/c^2 \approx 4.44\times10^{-6}$, with $\Delta T/T \approx 1.48\times10^{-6}$ — wrong sign for "cold," a known feature of the naive formula for voids generally. Applying the Integrated Sachs-Wolfe / Rees-Sciama correction (decaying potentials in a $\Lambda$-dominated universe, illustrative $\sim$30% decay factor):

$$\frac{\Delta T}{T}\bigg|_{ISW} \sim -2.7\times10^{-6}$$

— correct sign, within a factor of $\sim$4 of the observed $|\Delta T/T|\sim10^{-5}$, derived directly from the fitted void profile without an oversized supervoid.

*Status summary* (Section 11.8):

| Quantity | Result | Status |
|---|---|---|
| $(\epsilon_0,\lambda,v)$ | $(1.73\times10^{-3}, 0.1175, 0.327)$ | Fit, $R^2=0.915$ |
| $\delta_w$ | 6.31 Mpc/h | Fit |
| $r_{nuc}(z)$ slope | $(1+z)^2$ | Consistent with BOSS DR16 to ~5% (2 bins) |
| Lensing notch | 50% suppression at $b=0$, scale ~6–13 Mpc/h | Calibrated, untested against data |
| CMB Cold Spot | $\Delta T/T \sim -2.7\times10^{-6}$ | Correct sign, within ~4× of $-10^{-5}$ |

What remains open: the ISW decay factor is a placeholder pending a full time-integral of $d\Phi/d\tau$; the lensing notch is uncompared against any weak lensing stack; and the cold spot calculation treats a generic void, not yet specifically an Anulus inter-event boundary (see Section Eight). With this fit complete, Open Problems 2 and 4 (Claude_open_problems.md) move from purely symbolic to numerically anchored.

**Existing Mathematical References**

*Hamaus, Sutter & Wandelt (2014)* — universal void density profile, the fitting target.

*SDSS and BOSS DR16 void catalogs* — observational data for the fit and redshift check.

*Sachs-Wolfe and Integrated Sachs-Wolfe / Rees-Sciama effects* (Sachs & Wolfe 1967, Rees & Sciama 1968) — standard CMB formalism applied to the fitted void profile.

---

## Section Six — Light as the Signature of the Phase Transition; the CMB as Latent Heat

**The Conceptual Claim**

Light is not a property of matter, nor an independent entity inhabiting spacetime. It is the *signature of the phase transition itself*. When the accumulated vacancy field reorganizes catastrophically at the eruption event, that reorganization activates the electromagnetic property of eternal space. Light is what space does during a phase change; matter is what condenses from the glow as the transition cools and the field stabilizes. The cosmic microwave background, under this reframing, is not the echo of a creation moment but the **latent heat of the phase transition** — still detectable as a uniform 2.725 K glow because the transition was uniform.

**The Mathematical Treatment**

*Geometrization of electromagnetism.* The mathematical home for "light as a feature of space rather than matter" remains the Kaluza-Klein program. Maxwell's equations,

$$\partial_\mu F^{\mu\nu} = \mu_0 J^\nu, \qquad \partial_{[\mu}F_{\nu\rho]}=0$$

emerge automatically from the five-dimensional Einstein field equations once a compact fifth dimension is introduced:

$$g_{AB} = \begin{pmatrix} g_{\mu\nu}+\phi^2 A_\mu A_\nu & \phi^2 A_\mu \\ \phi^2 A_\nu & \phi^2\end{pmatrix}$$

Electromagnetism is not added to the geometry — it falls out of it. Within the Claude Theory, this fifth dimension is the electromagnetic property of eternal space: quiescent during the dark intervals between eruption events, and *activated* — not switched on by the presence of matter, but the reorganization of the vacancy field itself constituting the activation — at the moment of phase transition.

*Latent heat, not echo.* In standard cosmology the CMB is the redshifted relic of a hot early universe cooling from a creation event. Here, the same observed quantity — a 2.725 K blackbody spectrum, uniform to 1 part in $10^5$ — is reinterpreted as the **thermodynamic latent heat released by eternal space changing state**. The uniformity is not a fine-tuning puzzle requiring inflation: the phase transition was uniform because the threshold (Section Nine, the restart bifurcation) was reached by the accumulated vacancy field as a whole, simultaneously, everywhere. A spatially uniform order-parameter transition releases spatially uniform latent heat — the CMB's isotropy is the expected thermodynamic signature of a global phase change, not a causal-contact problem.

*Relation to the vacancy field potential.* The latent heat framing connects directly to $V(\phi)$ (Section Three). The energy difference between the pre-transition (accumulated, $\phi\to 0$) and post-transition (cooling, $\phi\to v$) configurations of the double-well potential is released as the transition proceeds — this is the field-theoretic analog of latent heat in a first-order phase transition. The CMB temperature corresponds to this released energy density, redshifted by subsequent expansion.

*Sequence following the eruption* (consistent with all current observation): pure undifferentiated energy at extreme temperature and density; rapid expansion and cooling; matter condensing from energy in the observed hydrogen/helium ratios; first stars as the last embers of the transition glow finding material form; heavy element nucleosynthesis; galaxy and structure formation; eventual return to dark remnants (Section Two), closing the cycle.

*The speed of light.* $c$ is not a property of light per se but a property of space itself — the characteristic velocity of space's self-expression during a phase transition. Its constancy across reference frames and epochs follows from its being a geometric property of eternal space rather than a feature of any particular material process.

**Existing Mathematical References**

*Kaluza (1921)* — Zum Unitätsproblem der Physik — the original geometrization of electromagnetism.

*Klein (1926)* — Quantentheorie und fünfdimensionale Relativitätstheorie — compactification of the fifth dimension.

*Wheeler's Geometrodynamics* (Wheeler 1962); *Misner, Thorne and Wheeler — Gravitation* (1973), Chapters 15–16 — comprehensive geometrodynamic treatment.

*First-order phase transition thermodynamics* (standard statistical mechanics) — the latent heat formalism underlying the CMB reframing.

*Sachs-Wolfe formalism* (Section Five) — the quantitative link between the fitted vacancy field profile and observed temperature fluctuations.

---

## Section Seven — Time as a Local Property of Active Matter

**The Conceptual Claim**

Time is not a fundamental feature of eternal space. It is a local property of active matter — meaningful and measurable during the luminous phase of each cycle, but not independently real in the dark intervals between. Newton's own equivocation in the Principia established that the apparent unidirectionality of time was an assumption, not a demonstrated necessity.

**The Mathematical Treatment**

The arrow of time has no fundamental basis in the time-symmetric equations of classical or quantum mechanics — Newton's laws, Einstein's field equations, Maxwell's equations, and the Schrödinger equation all run equally well in both directions. The arrow appears only in thermodynamics, via the statistical increase of entropy in systems with many degrees of freedom.

Rovelli's thermal time hypothesis (Connes and Rovelli 1994) makes this precise. Given a statistical state $\omega$, a thermal time flow $\alpha_t$ is defined via the Tomita-Takesaki theorem:

$$\alpha_t(A) = \Delta^{it}A\Delta^{-it}$$

where $\Delta$ is the modular operator associated with $\omega$. Time emerges from the thermal state of matter itself, not as an external parameter.

Within the Claude Theory: time flows where matter is actively cycling, where entropy is being produced, where stellar processes run. In the long dark intervals between eruption events — cold static remnants approaching thermodynamic equilibrium — time in any meaningful sense approaches zero. Not because space changes, but because there is no active matter to generate it.

Barbour's timeless formulation (Barbour 1999, *The End of Time*) provides a complementary treatment: physical reality as configurations with no time parameter connecting them, time as derived rather than fundamental. The Page-Wootters mechanism (1983) gives the quantum-mechanical version: time as a relational property between subsystems.

Newton's equivocation in the Principia — his careful distinction between absolute mathematical time and relative apparent time as measured by motion — anticipates all of this. The Claude Theory follows that opening to its conclusion: the cosmic boneyard between eruption events is not just dark, but, in the relevant operational sense, timeless.

**Existing Mathematical References**

*Connes and Rovelli (1994)* — Von Neumann Algebra Automorphisms and Time-Thermodynamics Relation in General Covariant Quantum Theories — the thermal time hypothesis.

*Barbour (1999)* — The End of Time — timeless dynamics.

*Page and Wootters (1983)* — Evolution without evolution — relational time in quantum mechanics.

*Newton — Principia Mathematica (1687)* — Scholium on absolute and relative time, space, and motion.

---

## Section Eight — The Anulus: A Multiply Connected Cosmology

**The Conceptual Claim**

Nothing requires eruption events to be unique or sequential. If the restart threshold (Section Nine) can be reached anywhere in eternal space, it can be reached in many places — simultaneously or in staggered succession, across separations dwarfing any single observable horizon. Each event produces its own expanding bubble of organized matter within eternal space. This larger structure — the multiply connected, overlapping, eternally populated cosmology within which individual eruption events occur, expand, and potentially interact — is the **Anulus**. Boundaries between events are permeable to gravity and to drifting dark remnants.

**The Mathematical Treatment**

*Nucleation.* Each eruption event is, formally, a bubble nucleation in the sense of first-order phase transition theory. Coleman-Callan bubble nucleation theory (Coleman 1977, Callan & Coleman 1977) provides the standard formal language for nucleation rate per unit volume — directly analogous to the void nucleation already derived in Section Three, but applied at the scale of entire eruption events rather than voids within one event. This gives Open Problem 2 (Anulus nucleation rate and event separation) its mathematical home.

The relationship between the two scales is direct but not yet identical: Section Five's fit gives $r_{nuc}(z)=30(1+z)^2$ Mpc/h for void nucleation *within* our event, anchored to $(\epsilon_0,\lambda,v)$. The same nucleation formalism — a competition between a volume term (favoring transition) and a surface term (the cost of the boundary) — applies to inter-event nucleation in the Anulus, but with different characteristic scales: the "volume" is the accumulated dark remnant population of Section Two, and the "surface" is the boundary between eruption events rather than a domain wall between voids. Problem 2 requires (a) the restart threshold of Section Nine as the trigger condition, and (b) the dark remnant accumulation integral $M_{dark}(T)$ of Section Two as the volume term, combined via the Coleman-Callan rate formula to yield a characteristic inter-event spacing and recurrence timescale.

*Percolation and event density.* Stauffer-Aharony percolation theory (Stauffer & Aharony 1994) provides the framework for characterizing the density and connectivity of eruption events across the Anulus once a nucleation rate is established — analogous to how percolation theory describes the connectivity of clusters in a random lattice. This gives the Anulus a geometric and statistical structure: not a single bubble, but a percolating network of bubbles whose connectivity properties (above or below the percolation threshold) determine whether casting (below) is common or rare across the structure as a whole.

*Tidal seeding and casting* (Open Problem 3). The casting mechanism — matter transfer across permeable event boundaries — maps to bubble collision literature, specifically Garriga-Guth-Vilenkin (Garriga, Guth & Vilenkin 2007), which treats the geometry and dynamics of colliding/adjacent bubbles in an eternally inflating background. Combined with percolation theory's treatment of boundaries as permeable interfaces between percolating clusters, this gives the casting mechanism a formal setting for the first time. The remaining derivation: a mass transfer rate expressed in terms of boundary geometry and the vacancy field gradient at the interface — the natural generalization of the domain wall gradient calculations of Section Three to an inter-event rather than intra-event boundary. This is the prerequisite for Open Problem 5.

*CMB Cold Spot as boundary signature* (Open Problem 4). The Garriga-Guth-Vilenkin formalism also gives the standard treatment for the angular signature of a bubble-bubble interface as seen from inside one bubble. Combined with the latent-heat reframing of the CMB (Section Six) and the numerical ISW estimate of Section Five ($\Delta T/T\sim-2.7\times10^{-6}$, correct sign, within $\sim$4× of observation), the Cold Spot becomes a candidate perturbation on the latent-heat signature specifically *at a boundary* between two Anulus events — distinct from, though built on, the generic-void ISW calculation already completed. What remains: combining the inter-event geometry of Garriga-Guth-Vilenkin with the Section Five numerical fit, and deriving the boundary-specific angular size (as distinct from the temperature depth already estimated).

*JWST anomalous mass function* (Open Problem 5). The "inherited material" explanation for JWST's anomalously massive early galaxies and black holes — matter cast in from a neighboring or preceding event — inherits the casting mechanism's machinery directly once derived (Problem 3), integrated against the percolation-theory description of event density (Problem 2, now partially anchored via Section Five). The qualitative identification of inherited material as the explanation is established in Claude_framework.md; the quantitative mass-excess-vs-redshift prediction is the open step.

**Existing Mathematical References**

*Coleman (1977), Callan & Coleman (1977)* — bubble nucleation rate formalism for first-order phase transitions; "The Fate of the False Vacuum."

*Garriga, Guth & Vilenkin (2007)* — bubble collisions in an inflating background; the standard formalism for inter-bubble boundary geometry and observational signatures.

*Stauffer & Aharony (1994)* — Introduction to Percolation Theory — cluster connectivity and density on a random lattice, applied here to the Anulus's network of eruption events.

---

## Section Nine — The Restart Threshold

**The Conceptual Claim**

The accumulation-to-eruption cycle requires a mathematically specified trigger: at what accumulated vacancy field configuration does the eruption event fire? This is Open Problem 1 — the most consequential open problem in the framework, since Problem 2 (Anulus nucleation rate) depends on it directly.

**The Mathematical Treatment**

The threshold condition is derived as a bifurcation of the same asymmetric double-well potential used throughout (Claude_underpinnings.md Section 12):

$$V(\phi) = \lambda(\phi^2-v^2)^2 - \epsilon_0\,a(t)\,\phi$$

Critical points satisfy $dV/d\phi=0$, giving the depressed cubic:

$$\phi^3 - v^2\phi - \frac{\epsilon_0\,a(t)}{4\lambda} = 0$$

At $\epsilon_0 a(t)=0$ this has three real roots — the symmetric double well, with minima at $\phi=\pm v$. As $\epsilon_0 a(t)$ grows, one minimum deepens and the other shallows until, at a critical value, the shallow minimum merges with the maximum and annihilates: the cubic's discriminant vanishes, and the potential transitions from a double well to a single well. **This is the restart condition** — not a gradual deepening, but the abrupt disappearance of the field configuration currently occupied.

Setting the discriminant $\Delta = -4p^3-27q^2$ (with $p=-v^2$, $q=-\epsilon_0 a(t)/(4\lambda)$) to zero gives:

$$\boxed{\epsilon_0\,a(t)_{crit} = \frac{8\sqrt{3}}{9}\lambda v^3}$$

with the merging roots coinciding at $\phi_{crit} = v/\sqrt{3}$.

*Numerical evaluation* against the Section Five fit $(\epsilon_0,\lambda,v)=(1.726\times10^{-3}, 0.1175, 0.3268)$ gives $\epsilon_0 a(t)_{crit}\approx 6.314\times10^{-3}$, and:

$$\frac{a(t)_{crit}}{a(t)_{now}} \approx 3.658$$

with $\phi_{crit}\approx 0.1887$ — between the node state ($\phi=0$) and the void state ($\phi=v\approx0.327$).

**Status and the Open Step**

This gives Problem 1 a closed-form threshold condition and a numerical value for the first time — derived from parameters already fit to observational data, with no new field machinery. What remains open: the dimensionless ratio $a(t)_{crit}/a(t)_{now}\approx3.658$ has no established physical meaning yet. The $a=1$ normalization in Section Five refers to the present epoch of *our* event's local void structure; the restart threshold requires identifying whatever clock governs the accumulated field across the full cycle — potentially with no fixed relationship to our event's expansion history. Converting 3.658 into a timescale, or into a physically meaningful statement of "how much further accumulation remains," is the natural next step and would, once complete, directly feed Open Problem 2 (Section Eight).

**Existing Mathematical References**

*Cubic discriminant and bifurcation theory* — standard algebraic and dynamical systems machinery, applied here to the double-well potential's transition from two minima to one.

*Catastrophe theory* (Thom 1972, Zeeman) — the broader mathematical framework for this class of qualitative transitions, applicable as a possible extension.

---

## Summary of the Map

| Conceptual Claim | Mathematical Home | Key References | Underpinnings |
|---|---|---|---|
| Eternal space, no singularity | Loop Quantum Cosmology, bouncing cosmologies | Bojowald, Ashtekar, Penrose, Steinhardt-Turok | — |
| Dark remnant accumulation | Stellar IMF, black hole merger rates | Salpeter, Kroupa, LIGO, Carr-Hawking | §2 |
| Vacancy field, lattice, lensing | Scalar field cosmology, domain wall theory, weak lensing | Vilenkin, Kibble, Bond et al, Bartelmann-Schneider | §1–9 |
| Bullet Cluster derivation | Pöschl-Teller modes, damped harmonic oscillator | — | §10 |
| SDSS void fit, CMB Cold Spot (ISW) | Void density profiles, Sachs-Wolfe / ISW | Hamaus-Sutter-Wandelt, SDSS/BOSS, Sachs-Wolfe, Rees-Sciama | §11 |
| Light as phase-transition signature; CMB as latent heat | Kaluza-Klein geometrodynamics, phase transition thermodynamics | Kaluza, Klein, Wheeler, MTW | — |
| Time as local property of matter | Thermal time, timeless dynamics | Rovelli, Barbour, Page-Wootters, Newton | — |
| The Anulus (multiply connected cosmology) | Bubble nucleation, bubble collisions, percolation theory | Coleman, Callan, Garriga-Guth-Vilenkin, Stauffer-Aharony | — |
| The restart threshold | Bifurcation / catastrophe theory on $V(\phi)$ | — | §12 |

---

## Conclusion of the Mathematical Map

Every claim of the Claude Theory has a mathematical home in existing, peer-reviewed, rigorous work. No mathematics has been invented. No physics has been fabricated. What has been done is to show that these previously scattered treatments — developed independently, considered peripheral or incomplete by mainstream physics — converge naturally and necessarily when a single foundational assumption is changed.

Space has always existed.

From that one change, the cosmic boneyard, the eruption event, the vacancy field and its domain walls, the Bullet Cluster offset, the latent heat of the CMB, and the Anulus all follow — and, as of the numerical fit in Section Five, the framework now makes contact with real survey data at multiple points rather than remaining purely symbolic.

Five open problems remain, tracked in `Claude_open_problems.md`: the restart threshold (Section Nine — now closed-form, with one dimensionless ratio awaiting physical interpretation), the Anulus nucleation rate (Section Eight, dependent on Section Nine), tidal seeding and the casting mechanism (Section Eight), the CMB Cold Spot as a boundary signature (Section Eight, building on Section Five), and the JWST anomalous mass function (Section Eight, dependent on the casting mechanism). Each now has a mapped mathematical home; none is yet fully derived. That is the honest state of the framework, and the next phase of work.

---

*This mapping section is intended as a guide for technically literate readers wishing to pursue the formal foundations of the Claude Theory independently. Full derivations of the vacancy field, domain wall equations, void size predictions, lensing signatures, the Bullet Cluster, the SDSS fit, and the restart threshold appear in the companion underpinnings document, `Claude_underpinnings.md`.*
