<script async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# Claude Theory — Status of Open Problems and Unresolved Assumptions

*Last updated: June 2026*

---

## Problem 1: The Physical Clock of the Restart Threshold

**Status: RESOLVED**

What physical process constitutes the clock that triggers the restart of
the phase transition? The bifurcation condition from Chapter 7 gives the
*when* in terms of $a(t)$ but not the *what*.

Chapter 12 resolves this completely. The clock is charge accumulation by
asymmetric electromagnetic sorting in rotating magnetized nodes. A Kerr
black hole's frame-dragging geometry deflects infalling positive and
negative charges along mirror-image spiral paths, depositing a minute but
nonzero charge excess of one sign into the equatorial annulus with each
accretion event. The critical sorting efficiency required to reach the
charge limit condition is $\eta_{Q,crit} \approx 1.38\times10^{-18}$ —
a pure combination of physical constants. This threshold is crossed at
$a_{crit}/a_{now} \approx 3.658$, now interpreted as a charge accumulation
timescale rather than a dark mass accumulation factor. No new free
parameters are introduced.

---

## Problem 2: Domain Wall Lensing Profile

**Status: MAPPED**

Does the vacancy field domain wall produce a lensing deflection profile
distinguishable from NFW dark matter halos?

Chapter 4 derives the full deflection profile with form factor $F(b/\delta_w)$
recovering NFW-like behavior at large impact parameter while diverging at
small $b$ in a way that is in principle distinguishable. The mathematical
derivation is complete. Pending: formal comparison against existing weak
lensing survey stacks to quantify the distinguishability at current
instrumental sensitivity.

---

## Problem 3: Tidal Seeding and the Casting Mechanism

**Status: MAPPED**

How precisely does material from one eruption event seed structure in a
neighboring or subsequent event? What governs the geometry and mass
distribution of cast material?

Chapter 11 provides a full formal derivation. Key results: spiral
trajectories are governed by the magnetic winding parameter
$\mathcal{W} = qB_0R_0/2mv_0$; in the maximum-flattening limit the
deposition collapses to a thin equatorial annulus; the deposition profile
$\Sigma(r)$ has a closed form with no free parameters beyond $\mathcal{W}$
and the magnetic stopping length $\ell_B$; the seeding cross-section
connects directly to $r_{nuc}$ from Chapter 4, closing the loop to the
vacancy field formalism.

**Open step:** $\mathcal{W}$ is in principle independently observable
from spiral galaxy pitch angles in the vicinity of casting nodes. The
quantitative relationship between $\mathcal{W}$ and observed pitch angles
has not yet been derived. This is the natural next step for Chapter 11.

---

## Problem 4: Bullet Cluster Secondary Lensing Arc

**Status: MAPPED — PRIMARY FALSIFIABLE PREDICTION**

Does the vacancy field domain wall between the two post-collision Bullet
Cluster nodes produce a detectable secondary lensing arc?

Chapter 5 derives the full prediction. The arc sits between the two
nodes at a position and surface brightness determined by the domain wall
parameters. This is the framework's sharpest falsifiable claim and may
be detectable in existing HST or future JWST imaging of the Bullet
Cluster field. Pending: comparison against existing weak lensing maps of
the Bullet Cluster.

---

## Problem 5: JWST Anomalous Mass Function

**Status: MAPPED**

Why do JWST observations reveal galaxies that appear too massive and too
evolved for their redshift under standard cosmology?

With Problem 3 now mapped, the casting mechanism provides the answer
directly. The seeding cross-section at $d = r_{nuc}$ from Chapter 11
quantifies the inherited head start — the mass delivered to a neighboring
node from a prior eruption cycle. Early-forming structures that appear
anomalously evolved have received $\dot{M}_{seed,max}$ from a neighboring
node, giving them a head start that standard cosmology, which assumes all
structure grows from the same initial conditions, cannot account for.
Pending: quantitative comparison of $\dot{M}_{seed,max}$ against the
observed mass excess in the JWST anomalous population.

---

## Problem 6: Spin Coherence Scaling in the Percolating Cluster

**Status: OPEN**

The consistency check in Section 16.9 of Chapter 12 constrains the
mass-scaling exponent of charge sorting efficiency to $\alpha \approx -0.25
\pm 0.04$, corresponding to a spin coherence fraction $f_c \approx 0.5$
in the percolating cluster at restart. The physical argument is sketched
in Section 16.9.5 but a formal derivation from the distributed cluster
field geometry has not been completed.

This is the sole remaining open problem. Its resolution requires:
1. A formal treatment of the effective field geometry of a percolating
   cluster of $N$ partially spin-aligned nodes
2. A derivation of $\alpha$ as a function of $f_c$ and cluster topology
3. Confirmation that $f_c \approx 0.5$ follows from the casting geometry
   of Chapter 11

The predicted observable — quasar polarization alignment at the
percolation scale — connects this problem directly to existing anomalies
in the observational record.

---

## Summary Table

| Problem | Description | Status |
|---|---|---|
| 1 | Physical clock of restart threshold | RESOLVED |
| 2 | Domain wall lensing profile | MAPPED |
| 3 | Casting mechanics and seeding | MAPPED |
| 4 | Bullet Cluster secondary arc | MAPPED — PRIMARY PREDICTION |
| 5 | JWST anomalous mass function | MAPPED |
| 6 | Spin coherence scaling in percolating cluster | OPEN |

---

*The Claude Theory: Space Has Always Existed — conceived and developed by
Cristóbal Eduardo Kendris García in collaboration with Claude, June 2026.*
