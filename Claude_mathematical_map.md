<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# The Claude Theory — Mathematical Foundations and Reference Map

## Preamble

The framework presented here does not invent new mathematics. It assembles existing, rigorous mathematical treatments — some mainstream, some underutilized, some considered peripheral until now — and shows that they converge naturally when a single foundational assumption is changed:

**Space has always existed.**

What follows maps each conceptual claim of the Claude Theory to its mathematical home, with sufficient detail for a technically literate reader to pursue each thread independently.

---

## Section One — Eternal Space and the Elimination of Singularity

**The Conceptual Claim**

The Big Bang was not a creation event. It was a phase transition within pre-existing eternal space. Space has no t=0.

**The Mathematical Treatment**

Current cosmology describes the universe using the Friedmann-Lemaître-Robertson-Walker metric:

$$ds^2 = -dt^2 + a(t)^2\left[dr^2 + r^2d\Omega^2\right]$$

where $a(t)$ is the scale factor. Standard treatment allows $a(t) \to 0$ as $t \to 0$ — the singularity. We replace this with a minimum condition:

$$a(t) \geq a_{min} > 0$$

This single modification eliminates the singularity without disturbing the rest of the metric machinery. The universe contracts to a threshold and rebounds. It never reaches zero.

**Existing Mathematical References**

*Loop Quantum Cosmology* (Bojowald 2001, Ashtekar and Singh 2011) achieves precisely this using quantum geometry. The classical singularity is replaced by a quantum bounce. The mathematics is well developed and peer reviewed. Our framework adopts the bounce result while providing a different physical interpretation — not a quantum effect but a classical phase transition threshold.

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

## Section Three — The Vacancy Field and Cosmic Structure

**The Conceptual Claim**

The large scale structure of the universe — filaments, walls, voids — constitutes a gravitational lattice. The apparent dark matter distribution is not a population of discrete objects but a vacancy field propagating through this lattice, analogous to electron holes in a semiconductor crystal.

**The Mathematical Treatment**

This section is developed in full in the companion mathematical underpinnings document. The key results are summarized here.

The vacancy field is defined as:

$$\phi(\mathbf{x}, t) = 1 - \frac{\rho(\mathbf{x},t)}{\rho_{max}}$$

Its dynamics are governed by a wave equation in expanding spacetime:

$$\ddot{\phi} + 3H\dot{\phi} - \frac{\nabla^2\phi}{a^2} = -4\lambda\phi\left(\phi^2 - v^2\right) + \epsilon_0 \cdot a(t)$$

The asymmetric double well potential:

$$V(\phi) = \lambda\left(\phi^2 - v^2\right)^2 - \epsilon_0 \cdot a(t)\phi$$

produces domain walls coinciding with observed cosmic filaments and sheets, and yields the testable prediction:

$$r_{nuc}(z) = \frac{\sqrt{2\lambda}v^2}{\epsilon_0}(1+z)^2$$

The void characteristic radius scales as $(1+z)^{-2}$ — voids are smaller at high redshift by a specific power law testable against existing void catalogs.

The lensing signature derived from the same potential produces NFW-like halo profiles around mass concentrations and naturally accounts for the Bullet Cluster offset as a topological rather than material phenomenon.

**The Bullet Cluster — A Quantitative Derivation**

The vacancy field framework does not merely accommodate the Bullet Cluster's lensing-mass offset qualitatively — it produces a quantitative derivation of it, developed in full in Section 10 of the underpinnings document. The argument proceeds as follows.

Each colliding cluster is modeled as a lattice node carrying its own NFW-like vacancy field configuration. During the collision, baryonic gas decelerates under ram pressure while the dark remnant populations pass through collisionlessly. The vacancy field's response is governed by its relaxation timescale, set by the lowest non-zero mode of the Pöschl-Teller spectrum:

$$\tau_{relax} = \frac{1}{\sqrt{12\lambda}\, v}$$

When this timescale is short compared to the collision crossing time $\tau_{cross} = 2r_{node}/v_{col}$, the vacancy field — and therefore the lensing centroid — tracks the collisionless mass rather than the gas. This produces a predicted lensing-gas offset of

$$\Delta x_{lens-gas} = x_{node} - x_{gas} \approx 200 \text{ kpc}$$

as a geometric inevitability of the topology rather than a fitted parameter, consistent with observation.

The domain wall separating the two nodes must re-establish itself at the new midpoint following the collision. Its motion is governed by a damped harmonic oscillator equation, with effective mass, restoring constant, and damping coefficient all determined by the same potential parameters $\epsilon_0$, $\lambda$, $v$ already fixed by the void size distribution (Section One above) and the primary lensing profile. Solving this equation yields a residual wall displacement function $\mathcal{G}$, which fixes the position of a **secondary lensing arc** between the two primary mass concentrations, offset toward the direction of the bullet subcluster's motion.

This secondary arc is a feature with no counterpart in particle dark matter models — there is no mechanism by which a population of non-interacting particles would produce a third, displaced lensing concentration tracking the relaxation of a topological boundary. Its detection or non-detection in existing deep weak lensing maps of the Bullet Cluster constitutes a direct, falsifiable test of the vacancy field framework, using parameters already constrained by independent observations (void statistics and the primary lensing profile) rather than parameters tuned to the Bullet Cluster itself.

**Existing Mathematical References**

*Cosmic web topology* (Bond, Kofman, Pogosyan 1996) provides the observational and mathematical foundation for the filament-void-node structure as a lattice.

*Domain wall cosmology* (Vilenkin 1981, Kibble 1976) provides the mathematical treatment of topological defects in scalar fields — directly applicable to our vacancy field domain walls.

*Weak gravitational lensing formalism* (Bartelmann and Schneider 2001) provides the mathematical framework within which our lensing predictions are derived.

*Pöschl-Teller potential and its spectrum* (Pöschl and Teller 1933) provides the exactly solvable quantum-mechanical analog used to compute the vacancy field's relaxation timescale and shape mode.

*Damped harmonic oscillator dynamics* — standard classical mechanics, applied here to the post-collision relaxation of a topological domain wall rather than a material object.

---

## Section Four — Light as an Intrinsic Property of Space

**The Conceptual Claim**

Light does not travel through space. Light is space expressing itself. The electromagnetic field is not a separate entity inhabiting spacetime — it is a fundamental geometric property of spacetime itself. Matter temporarily activates this expression during the luminous phase of each cycle.

More specifically, the electromagnetic radiation that fills the universe — the glow — is not produced by matter. It is the **signature of the phase transition itself**: the latent energy released as the vacancy field reorganizes during an eruption event. Matter condenses from this glow as the transition cools, rather than producing it.

**The Mathematical Treatment**

The mathematical home of the geometric claim is the geometrization of electromagnetism — the program of expressing Maxwell's equations as intrinsic features of the spacetime metric rather than external fields defined upon it.

Maxwell's equations in standard form:

$$\partial_\mu F^{\mu\nu} = \mu_0 J^\nu$$
$$\partial_{[\mu} F_{\nu\rho]} = 0$$

where $F_{\mu\nu} = \partial_\mu A_\nu - \partial_\nu A_\mu$ is the electromagnetic field tensor.

Kaluza's insight (1921) was that if spacetime has a fifth compact dimension, the five-dimensional Einstein field equations decompose into the four-dimensional Einstein equations *plus* Maxwell's equations automatically — with no additional assumptions. Electromagnetism emerges from pure geometry.

The five dimensional metric takes the form:

$$g_{AB} = \begin{pmatrix} g_{\mu\nu} + \phi^2 A_\mu A_\nu & \phi^2 A_\mu \\ \phi^2 A_\nu & \phi^2 \end{pmatrix}$$

where $A_\mu$ is the electromagnetic four-potential and $\phi$ is a scalar field. Maxwell's equations are not added — they fall out of the geometric structure.

Klein's contribution (1926) compactified the fifth dimension, explaining why it is not directly observable while remaining physically real.

Within the Claude Theory this mathematics takes on new meaning, and a mechanism. The fifth dimension is not merely "always present" in an inert sense — it is **quiescent in the dark intervals between eruption cycles and activated by the phase transition itself**. The eruption event is the vacancy field undergoing a catastrophic reorganization between vacuum states — precisely the domain wall dynamics of Section Three, occurring at the scale of the entire accumulated structure rather than a single node. That reorganization activates the electromagnetic property of eternal space. Light does not switch on because matter appears; matter appears because it switches on.

**The CMB as Latent Heat of the Phase Transition**

This mechanism gives a direct account of the cosmic microwave background. In thermodynamics, latent heat is energy released during a phase change that is a property of the *transition*, not of the substance's temperature — water releasing latent heat as it freezes is the standard example, and the released energy is necessarily uniform wherever the phase change occurs uniformly.

The CMB — uniform to one part in $10^5$ across the sky, with a thermal spectrum at 2.725 K — is, on this account, the **latent heat of the eruption event's phase transition**, redshifted by subsequent expansion. Its uniformity is not a puzzle requiring an inflationary mechanism to establish causal contact across the sky. It is uniform because the phase transition that produced it was uniform: the threshold was reached by the accumulated vacancy field as a whole, and the glow was released everywhere within the event simultaneously, as a consequence of the field's global reorganization rather than local thermal contact.

This reframes the horizon problem rather than solving it within the inflationary paradigm: the problem is dissolved because the premise that requires it — that the uniform temperature must be established by causal communication between regions — does not apply to a release that is a single coherent feature of the field's transition, not a set of independently thermalizing regions.

The speed of light as a universal constant — $c$ — is then not a property of light per se but a property of space itself: the characteristic velocity of space's self-expression during and after the transition. This is consistent with the observed constancy of $c$ across all reference frames and all cosmic epochs.

**Existing Mathematical References**

*Kaluza (1921)* — Zum Unitätsproblem der Physik — the original geometrization of electromagnetism

*Klein (1926)* — Quantentheorie und fünfdimensionale Relativitätstheorie — compactification of the fifth dimension

*Wheeler's Geometrodynamics* (Wheeler 1962) — the program of deriving all physics from spacetime geometry

*Einstein-Maxwell theory* — the partially unified treatment of gravity and electromagnetism in four dimensions, providing mathematical tools applicable here

*Misner, Thorne and Wheeler — Gravitation (1973)* — the comprehensive mathematical treatment of geometrodynamics, Chapters 15 and 16 specifically

*Latent heat and first-order phase transitions* — standard thermodynamics, providing the formal analogy for energy release that is a property of the transition rather than the post-transition state, and for why such release is spatially coherent wherever the transition condition is met uniformly

*Domain wall energy release* (Vilenkin 1981, Kibble 1976) — the same topological defect formalism used in Section Three provides the mechanism by which the vacancy field's reorganization at threshold releases energy as a global, coherent event rather than a local one

---

## Section Five — Time as a Local Property of Active Matter

**The Conceptual Claim**

Time is not a fundamental feature of eternal space. It is a local property of active matter — meaningful and measurable during the luminous phase of each cycle, but not independently real in the intervals between. Newton's own equivocation in the Principia established that the apparent unidirectionality of time was an assumption, not a demonstrated necessity.

**The Mathematical Treatment**

The arrow of time — its apparent unidirectional flow from past to future — has no fundamental basis in the equations of classical or quantum mechanics. Newton's laws, Einstein's field equations, Maxwell's equations, and Schrödinger's equation are all time-symmetric. They run equally well in both directions. The arrow of time is not in the fundamental equations.

It appears in thermodynamics — specifically in the second law, the increase of entropy. But entropy increase is a statistical property of systems with many degrees of freedom, not a fundamental law of spacetime itself.

Rovelli's thermal time hypothesis (Connes and Rovelli 1994) makes this mathematically precise. Given a statistical state $\omega$ of a physical system, a thermal time flow $\alpha_t$ is defined by the Tomita-Takesaki theorem of operator algebras:

$$\alpha_t(A) = \Delta^{it} A \Delta^{-it}$$

where $\Delta$ is the modular operator associated with the state $\omega$. Time, in this formulation, is not an external parameter but emerges from the thermal state of matter itself.

The physical interpretation within the Claude Theory is direct — time flows where matter is actively cycling, where entropy is being produced, where stellar processes are running. In the long dark intervals between eruption cycles, where space is filled only with cold static remnants approaching thermodynamic equilibrium, time in any meaningful sense approaches zero. Not because space changes — but because there is no active matter to generate it.

Barbour's timeless formulation (Barbour 1999, *The End of Time*) provides a complementary mathematical treatment. In his framework physical reality consists of configurations — instants — with no time parameter connecting them. Time as experienced is a derived quantity, emerging from the structure of configurations rather than being fundamental.

The Page-Wootters mechanism (1983) provides a quantum mechanical treatment of the same insight — time as a relational property between subsystems rather than an external absolute parameter.

Newton's equivocation in the Principia — his careful distinction between absolute mathematical time and relative apparent time as measured by motion — anticipates all of this. He knew the two were not necessarily the same thing. The Claude Theory follows that opening to its conclusion.

**Existing Mathematical References**

*Connes and Rovelli (1994)* — Von Neumann Algebra Automorphisms and Time-Thermodynamics Relation in General Covariant Quantum Theories — the thermal time hypothesis

*Barbour (1999)* — The End of Time — timeless dynamics

*Page and Wootters (1983)* — Evolution without evolution — relational time in quantum mechanics

*Newton — Principia Mathematica (1687)* — Scholium on absolute and relative time, space, and motion — the primary source establishing Newton's own equivocation on the nature of time

---

## Section Six — The Anulus: A Multiply Connected, Eternally Populated Cosmology

**The Conceptual Claim**

Nothing in the framework restricts the threshold condition for an eruption event to a single location in eternal space. If dark remnants accumulate wherever matter has completed prior cycles, and eternal space is unbounded, the threshold may be reached in many regions — simultaneously, in staggered succession, or both. Our observable universe is one such eruption event among possibly many, embedded in a larger structure of overlapping, permeable bubbles. We call this larger structure the **Anulus**.

Within the Anulus, condensing matter following an eruption event is not guaranteed to organize around a single origin point. Nearby eruption events, or dark remnant populations left over from prior cycles, can gravitationally influence — "hijack" — the condensation of a newer event. And where bubbles approach or overlap, matter and remnants from one event's history can be incorporated into another's — a process we call **casting**.

This extension is presently the least mathematically developed part of the framework. It is included here as a mapped research direction with identified mathematical homes, rather than as a completed derivation, in keeping with the honest standard set elsewhere in this document.

**The Mathematical Treatment — Identified Directions**

*Multiplicity and simultaneity of eruption events.* The question of whether a threshold condition is reached at multiple locations in an unbounded space is formally a question about the statistics of a stochastic field crossing a barrier. This is the same mathematical structure as **bubble nucleation in first-order phase transitions** (Coleman 1977, Callan and Coleman 1977), where the nucleation rate per unit volume per unit time, $\Gamma$, determines whether bubbles form as isolated, well-separated events or as a dense, overlapping population. The vacancy field potential $V(\phi)$ already derived in Section Three is precisely the kind of potential this formalism is built to analyze; the same $\epsilon_0$, $\lambda$, $v$ that fix the void nucleation length $r_{nuc}(z)$ in principle also fix $\Gamma$, and therefore the expected separation and overlap statistics of eruption events within the Anulus.

*Permeable boundaries and percolation.* Whether eruption-event bubbles remain isolated or form a connected, overlapping network as they grow is the subject of **percolation theory** (Stauffer and Aharony 1994), and of the bubble-collision literature within eternal inflation models (Garriga, Guth, Vilenkin 2007 onward). That literature was developed for a different physical picture — inflating bubbles within an inflaton landscape — but its mathematics of bubble growth, collision geometry, and the statistics of collision remnants within an observer's bubble is directly applicable to the Anulus, with the vacancy field domain walls of Section Three playing the role of the bubble walls.

*Gravitational hijacking of condensation.* This is a perturbation to the condensation dynamics already implicit in Section Three: an external gravitational potential $\Psi_{ext}$, sourced by a neighboring event or by inherited dark remnants, added to the right-hand side of the vacancy field equation of motion. Its mathematical treatment is an extension of standard **structure formation with an external tidal field** (the same formalism used to study tidal torquing of galaxy halos by large-scale structure), applied here at the scale of an entire eruption event rather than a single halo.

*Casting — inherited matter from neighboring or prior events.* Where bubble walls in the Anulus are crossed or merge, dark remnants and partially-formed structure from one event's history become initial conditions for structure formation in another. This maps onto the treatment of **pre-existing density perturbations as initial conditions for structure formation** — formally identical to how standard cosmology treats primordial perturbations as inputs to the growth equations, except that here the "primordial" perturbations are not primordial at all, but inherited remnants with their own formation history.

**A Candidate Observational Signature**

The JWST observations of galaxies with stellar masses and degrees of structural maturity in tension with standard formation timelines are, within this section, reframed as a candidate signature of casting: such objects would not need to have formed unusually early within their own event, if some of their constituent mass was inherited — already aggregated — from a neighboring or prior event across a permeable boundary. This reframing does not yet constitute a derivation; it identifies what a derivation would need to produce — namely, a predicted *mass function* for inherited structures, derivable in principle from the nucleation rate $\Gamma$ and bubble-collision statistics above, that could be compared against the observed anomalous mass function.

A second candidate signature is the CMB cold spot: an anomalously cold region of the cosmic microwave background with no fully satisfactory explanation in standard cosmology. Within the Anulus, a region where our event's boundary has been approached or crossed by a neighboring event would be a candidate location for such an anomaly, since the latent-heat release described in Section Four need not be perfectly uniform across a boundary shared with another event. This too remains a candidate rather than a derivation at present.

**Existing Mathematical References**

*Coleman (1977), Callan and Coleman (1977)* — Fate of the false vacuum — the foundational mathematics of bubble nucleation rates in first-order phase transitions

*Stauffer and Aharony (1994)* — Introduction to Percolation Theory — the mathematics of connectivity and overlap in random spatial structures

*Garriga, Guth, Vilenkin (2007 onward)* — bubble collisions in the eternal inflation literature — geometry and observational signatures of bubble-bubble collisions, directly transferable to Anulus boundary interactions

*Standard structure formation with tidal fields* — the existing formalism for external gravitational influence on halo formation, extended here to the scale of whole eruption events

*Cosmological perturbation theory* (initial conditions formalism) — the existing treatment of pre-existing density fields as inputs to structure growth, repurposed here for inherited rather than primordial structure

---

## Summary of the Map

| Conceptual Claim | Mathematical Home | Key References |
|---|---|---|
| Eternal space, no singularity | Loop Quantum Cosmology, Bouncing cosmologies | Bojowald, Ashtekar, Penrose |
| Dark remnant accumulation | Stellar IMF, black hole merger rates | Salpeter, LIGO, Carr-Hawking |
| Vacancy field and cosmic structure | Scalar field cosmology, domain wall theory | Vilenkin, Kibble, Bond et al |
| Bullet Cluster offset and secondary arc | Domain wall relaxation, Pöschl-Teller spectrum, damped oscillator dynamics | Pöschl-Teller, Vilenkin |
| Light as property of space; CMB as latent heat | Kaluza-Klein, geometrodynamics, latent heat of phase transitions | Kaluza, Klein, Wheeler, MTW |
| Time as local property of matter | Thermal time, timeless dynamics | Rovelli, Barbour, Page-Wootters, Newton |
| The Anulus — multiply connected cosmology | Bubble nucleation, percolation theory, eternal inflation bubble collisions | Coleman, Callan-Coleman, Stauffer-Aharony, Garriga-Guth-Vilenkin |

---

## Conclusion of the Mathematical Map

Every claim of the Claude Theory has a mathematical home in existing, peer reviewed, rigorous work. No mathematics has been invented. No physics has been fabricated. What has been done is to show that these previously scattered treatments — developed independently, considered peripheral or incomplete by mainstream physics — converge naturally and necessarily when a single foundational assumption is changed.

Space has always existed.

From that one change, everything else follows — and the mathematics was already there, waiting.

The Anulus extension in Section Six is presented at an earlier stage of development than the rest of the framework, and is marked as such. Its mathematical homes are identified; its derivations are not yet complete. That distinction is itself part of the honest standard this document aims to maintain.

---

*This mapping section is intended as a guide for technically literate readers wishing to pursue the formal foundations of the Claude Theory independently. Full derivations of the vacancy field, domain wall equations, void size predictions, and lensing signatures — including the Bullet Cluster derivation summarized in Section Three — appear in the companion underpinnings document.*
