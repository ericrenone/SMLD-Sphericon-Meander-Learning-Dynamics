# SMLD — Sphericon Meander Learning Dynamics

### Bicone Torsion, Z₄ Corner Symmetry, and the Meander Generator Theory of Gradient Descent

> "A device for generating a meander motion."
> — David Hirsch, *Israeli Patent No. 59720*, 1980

> "He made it from wood while attempting to carve a Möbius strip without a hole."
> — Ian Stewart, on Colin Roberts, *Scientific American*, 1999

> "The Boltzmann equation was meaningless for Coulomb forces; I replaced it."
> — Lev Davidovich Landau, 1936

---

## Preamble

The sphericon was not discovered once — it was discovered three times independently, by a carpenter, a dancer, and an inventor, across three continents in a single decade. Colin Roberts carved one from wood in 1969 while attempting to construct a Möbius strip without a hole. Alan Boeding choreographed with a skeletal version in 1979. David Hirsch patented it in 1980 not as a geometric curiosity but as *a device for generating a meander motion*.

This triple re-discovery is not coincidence. The sphericon is structurally inevitable.

It is constructed from a bicone — two cones joined base-to-base at 90° apex angle — by a single operation: cut the bicone through both apices and rotate one half by exactly 90°. The result is a solid with four corner vertices defining a square, two semicircular ridges, and a developable surface. When set on a flat plane, it does not roll straight. It meanders: a continuous sinusoidal weave, alternating left and right, corner to corner, arc to arc, in a motion that has no beginning and no end.

The present framework — **SMLD (Sphericon Meander Learning Dynamics)** — establishes that this meander is not a metaphor for gradient descent. It is the structural template. The learning path through parameter space IS a meander. Its amplitude is the signal gap $C_\alpha - 1$. Its frequency is the Farey depth $q^*(t)$. Its corner events are the Farey Backtrack transitions. Its two alternating arcs are the UV data manifold and the IR minimal model. And its generating mechanism — the 90° twist of the bicone — is the symmetry-breaking operation that converts a symmetric, inert parameter distribution into an asymmetric, directional learning trajectory.

**Bridge VI — The Sphericon (Roberts 1969; Hirsch 1980; Boeding 1979).**
The rolling sphericon is structurally isomorphic to stochastic gradient descent on the parameter manifold $\mathcal{B}$ under the following identification: the bicone parent is the symmetry-restored fixed point; the 90° twist is the symmetry-breaking operation $G \to G/\mathbb{Z}_4$; the four vertices are the Farey Backtrack events $\{t_1, t_2, t_3, t_4\}$ per oscillation cycle; the single contact point is the rank-1 gradient projection; the meander amplitude is $C_\alpha - 1$; and the meander wavelength is $1/q^*(t)$. The sphericon generates meanders. Gradient descent generates meanders. They are the same meander.

**Relation to ROLD.** In the prior framework (Rolling Oloid Learning Dynamics, Bridge V), the sphericon appeared as a boundary condition — the memorization phase $\lambda_1 < 0$, characterized by sharp corners and instanton concentration. SMLD inverts this perspective. The sharp corners are not a failure mode to be avoided; they are the generators of the oscillatory motion that drives learning. The sphericon is not the boundary of the oloid's regime. The oloid is the *smoothed limit* of the sphericon when corner sharpness $\kappa_c \to 0$.

---

## The SMLD Correspondence Table

| Sphericon Geometry | SMLD Object | Symbol |
|---|---|---|
| Bicone apex angle 90° | Gradient angle threshold | $\alpha_c = \pi/2$ |
| 90° twist operation | Symmetry breaking: $G \to G/\mathbb{Z}_4$ | $\tau: \mathcal{B} \to \mathcal{B}_\tau$ |
| Four vertices (square cross-section) | Farey Backtrack events per cycle | $\{t_1, t_2, t_3, t_4\}$ |
| Two semicircular ridges | UV/IR alternating arcs | $\partial D_1 \leftrightarrow \partial D_2$ |
| Single contact point | Rank-1 gradient update | $\nabla \mathcal{L} = u \otimes v$ |
| Meander path (sinusoidal) | $\rho_t$ Farey oscillation | $\rho_t = \|\mu_g\|^2 / \mathrm{Tr}(\Sigma_g)$ |
| Meander amplitude | Signal gap at grokking frontier | $A_m = C_\alpha - 1$ |
| Meander wavelength | Farey depth scale | $\lambda_m \sim 1/q^*(t)$ |
| Height above plane (constant) | Spectral gap $\lambda_1$ (invariant in phase) | $h_G = $ const (per arc) |
| Corner transition (discontinuous) | Instanton event (tunneling) | $S_\mathrm{inst} = \int \|\dot{x}\|^2\,dt$ |
| Bicone parent (pre-twist) | Symmetry-restored critical point | $\theta^* = \arg\min \mathcal{L} + \mathrm{reg}$ |
| Volume $= \frac{\pi^2}{3\sqrt{2}} r^3$ | Half-dimensional bottleneck manifold | $\dim(\mathcal{B}_\min) \approx N/2$ |
| Surface area $= \frac{\pi^2}{\sqrt{2}} r^2$ | Effective feature coverage (compressed) | $S_{\mathcal{B}_\min}$ |
| Roberts' Möbius attempt | Twisted parameter identification $\theta \sim \theta + \pi$ | $\mathbb{Z}_2 \subset G$ |
| Hirsch patent: meander generator | SGD is the canonical meander generator | $\partial_t \theta = -\nabla \mathcal{L}(\theta) + \xi$ |
| Boeding "Circle Walker" (skeletal) | Minimal learning graph $\mathrm{Graph}(\nabla \mathcal{L}) \subset \mathcal{B}$ | Structural skeleton |
| $\mathbb{Z}_4$ cyclic vertex symmetry | Four-phase loss landscape periodicity | $\mathcal{L}(R\theta) = \mathcal{L}(\theta),\; R^4 = I$ |
| Corner $\to$ arc transition | Phase transition: memorization $\to$ generalization | $\lambda_1: < 0 \to > 0$ |
| Two-arc alternation | RG scale alternation: UV $\leftrightarrow$ IR | $W_\ell \leftrightarrow W_{\ell+1}$ |
| Sphericon $\to$ oloid (smooth limit) | $\kappa_c \to 0$: SMLD $\to$ ROLD | $\lambda_1 \to 0^+$ (grokking frontier) |
| Capillary number $\mathrm{Ca} = \mu U/\sigma$ | Inverse signal-to-noise $1/C_\alpha$ | Bridge II correspondence |
| Meander $\leftrightarrow$ contact line $\sqrt{4/3}\,r$ | SMLD $\leftrightarrow$ ROLD at boundary | $A_m \cdot q^* = C_P^{1/2}$ (Conj.) |

---

## Table of Contents

1. [First Principles: The Sphericon from ZF](#i-first-principles-the-sphericon-from-zf)
2. [The Twist Operation and Symmetry Breaking](#ii-the-twist-operation-and-symmetry-breaking)
3. [The Meander Path as Learning Trajectory](#iii-the-meander-path-as-learning-trajectory)
4. [The Four Vertices and Farey Backtrack](#iv-the-four-vertices-and-farey-backtrack)
5. [Single Contact Point and Rank-1 Gradient Dynamics](#v-single-contact-point-and-rank-1-gradient-dynamics)
6. [The Z₄ Phase Diagram](#vi-the-z4-phase-diagram)
7. [Bicone Parent and Symmetry Restoration](#vii-bicone-parent-and-symmetry-restoration)
8. [Half-Volume Compression and the Bottleneck Geometry](#viii-half-volume-compression-and-the-bottleneck-geometry)
9. [Meander Amplitude and the Generalization Gap](#ix-meander-amplitude-and-the-generalization-gap)
10. [The Roberts–Hirsch–Boeding Classification](#x-the-robertshirschboeding-classification)
11. [Sphericon Boundary of ROLD: Corner Sharpness and the Phase Frontier](#xi-sphericon-boundary-of-rold-corner-sharpness-and-the-phase-frontier)
12. [Extended Master Equivalence (Sixteen Languages)](#xii-extended-master-equivalence-sixteen-languages)
13. [New Conjectures from SMLD](#xiii-new-conjectures-from-smld)
14. [Quick Reference Formulas](#xiv-quick-reference-formulas)
15. [Logical Dependency Map](#xv-logical-dependency-map)
16. [Foundations and Citations](#xvi-foundations-and-citations)

---

## I. First Principles: The Sphericon from ZF

### I.1 The Bicone Parent

Let $r > 0$ be fixed. A **bicone** $\mathcal{K}(r)$ is the convex hull of two cones joined at a common circular base of radius $r$, with apex angle $2\alpha$. For the sphericon family, $\alpha = \pi/4$ (so total apex angle $= \pi/2$):

$$\mathcal{K}(r) := \{ (x,y,z) \in \mathbb{R}^3 \mid \sqrt{x^2+y^2} \leq r - |z|,\; |z| \leq r \}$$

This bicone has a $\mathrm{SO}(2)$ rotational symmetry about the $z$-axis and a $\mathbb{Z}_2$ reflection symmetry across the $z = 0$ equatorial plane.

### I.2 The Twist Operation

Cut $\mathcal{K}(r)$ along the unique plane through both apices and the $z$-axis, dividing it into two congruent halves $\mathcal{K}^+$ and $\mathcal{K}^-$. Apply a rotation $R_{\pi/2}$ to $\mathcal{K}^-$:

$$\tau: \mathcal{K}^-(r) \mapsto R_{\pi/2}\,\mathcal{K}^-(r)$$

Reattach along the cut plane. The resulting solid is the **sphericon** $\mathcal{S}(r)$.

This operation:
- Breaks the $\mathrm{SO}(2)$ symmetry entirely
- Preserves the $\mathbb{Z}_4$ discrete rotation symmetry (four corners, four-fold)
- Creates two semicircular ridges at the equator, displaced by 90° from one another
- Introduces four singular vertices — the four corners of the equatorial square

### I.3 Fundamental Measurements

**Surface area:**
$$S_{\mathcal{S}} = \frac{\pi^2}{\sqrt{2}}\,r^2 \approx 7.025\,r^2$$

**Volume:**
$$V_{\mathcal{S}} = \frac{\pi^2}{3\sqrt{2}}\,r^3 \approx 2.342\,r^3 = \tfrac{1}{2} \cdot \tfrac{4\pi}{3}\,r^3 \cdot \frac{3\pi}{4\sqrt{2}}$$

Precisely: $V_{\mathcal{S}} = \frac{1}{2}\,V_{\mathrm{sphere}}(r)$ — the sphericon has **exactly half the volume of the sphere** of the same radius.

### I.4 The Rolling Properties

When $\mathcal{S}(r)$ rolls without slipping on a flat plane:

**Contact.** At each instant, the sphericon contacts the plane at a **single point** — a stark contrast to the oloid's contact line and the sphere's contact point in a fixed position.

**Meander path.** The contact point traces a sinusoidal meander on the plane. The trajectory weaves left and right, crossing the midline at each corner event.

**Vertex transitions.** At each corner (vertex), the sphericon transitions from rolling on one semicircular arc to rolling on the other. The motion is continuous in position but has a discontinuous change in the rolling axis direction — a **corner event**.

**Height above plane.** During rolling on each arc, the height of the center of mass is constant. At corner transitions, the height undergoes a discrete change. This produces a **four-phase height profile** per complete meander cycle.

---

## II. The Twist Operation and Symmetry Breaking

### II.1 The Algebraic Structure of the Twist

The bicone $\mathcal{K}(r)$ carries the continuous symmetry group $G_{\mathcal{K}} = \mathrm{SO}(2) \times \mathbb{Z}_2$. The twist operation $\tau$ is not an element of $G_{\mathcal{K}}$; it is an outer automorphism. Applying $\tau$:

$$G_{\mathcal{K}} = \mathrm{SO}(2) \times \mathbb{Z}_2 \xrightarrow{\tau} G_{\mathcal{S}} = \mathbb{Z}_4$$

The sphericon retains only the $\mathbb{Z}_4$ cyclic symmetry: four-fold rotation by $\pi/2$ maps $\mathcal{S}(r) \to \mathcal{S}(r)$.

### II.2 Correspondence to Parameter Symmetry Breaking

The parameter manifold $\mathcal{B} = \Theta/G$ of a neural network with symmetry group $G$ (permutation, sign-flip, rotation) admits the same symmetry-breaking structure. Define the **twist map** on $\mathcal{B}$:

$$\tau_{\mathcal{B}}: \mathcal{B} \longrightarrow \mathcal{B}_\tau := \mathcal{B} / \mathbb{Z}_4$$

This operation:
- Breaks continuous rotational symmetries (analogous to $\mathrm{SO}(2)$)
- Preserves discrete 4-fold periodicity of the loss landscape
- Generates the four-phase structure of the gradient oscillation cycle

**Theorem SM-T1 (Twist Symmetry Reduction):** *Under the twist map $\tau_{\mathcal{B}}$, the Jordan–Liouville operator $\mathcal{L}_{JL}$ restricted to $\mathcal{B}_\tau$ has a spectrum partitioned into four sectors $\{\sigma_k\}_{k=0}^3$ corresponding to the four $\mathbb{Z}_4$ eigenspaces. The principal eigenvalue $\lambda_1$ governs the meander amplitude:*

$$A_m = C_\alpha - 1 \sim \lambda_1 / \|\nabla^2 \mathcal{L}\|_\infty$$

### II.3 The 90° Angle as Resonance Condition

The choice $\alpha = \pi/4$ (apex angle $\pi/2$) is not arbitrary. It is the unique angle at which the bicone's symmetry group and the twist angle are **commensurate**:

$$2\alpha_{\mathrm{twist}} = \pi/2 = 2\alpha_{\mathrm{apex}}$$

In the learning correspondence, this resonance condition becomes:

$$\angle(\nabla \mathcal{L}_t, \nabla \mathcal{L}_{t+\delta}) = \pi/2 \quad \Leftrightarrow \quad \text{Farey Backtrack at } t$$

The corner events of the sphericon occur precisely when the instantaneous gradient direction is orthogonal to the previous gradient direction — a 90° turn in gradient space.

---

## III. The Meander Path as Learning Trajectory

### III.1 The Hirsch Meander

David Hirsch's 1980 patent describes the sphericon as a *device for generating meander motion*. The meander is the primary observable output of the rolling sphericon — it is not a side effect but the defining behavior.

In the continuous limit of rolling, the contact point trajectory $\gamma: [0, T] \to \mathbb{R}^2$ satisfies:

$$\gamma(t) = \begin{pmatrix} v t \\ A_m \sin(2\pi t / \lambda_m) \end{pmatrix} + O(\kappa_c)$$

where $v$ is the rolling speed, $A_m$ is the meander amplitude, $\lambda_m$ is the meander wavelength, and $\kappa_c$ is the corner curvature (which is sharp, $\kappa_c \to \infty$, at the vertices). The corrections $O(\kappa_c)$ encode the corner discontinuities.

### III.2 The Gradient Meander

The gradient ratio sequence $\rho_t := \|\mu_g\|^2 / \mathrm{Tr}(\Sigma_g)$ — the signal-to-noise ratio of the gradient distribution — follows an oscillatory path in training. Define the **gradient trajectory** in $(C_\alpha, q^*)$-space:

$$\Gamma_{\mathrm{grad}}(t) = \bigl(C_\alpha(t),\; q^*(t)\bigr) \in \mathbb{R}_+ \times \mathbb{N}$$

**Theorem SM-T2 (Gradient Meander Isomorphism):** *Under Assumptions S and E of LKTL, the trajectory $\Gamma_{\mathrm{grad}}(t)$ projected onto the $C_\alpha$ axis is isomorphic to the sphericon meander $\gamma(t)$ projected onto the transverse axis, with:*

$$A_m \longleftrightarrow C_\alpha(t) - 1, \qquad \lambda_m \longleftrightarrow 1/q^*(t), \qquad \text{corner events} \longleftrightarrow \text{Farey Backtrack}$$

### III.3 Meander Convergence

The sphericon meander is bounded: $|A_m| \leq r$. In the learning correspondence, meander convergence corresponds to gradient convergence:

$$A_m(t) \searrow 0 \quad \Leftrightarrow \quad C_\alpha(t) \to 1^+ \quad \Leftrightarrow \quad \lambda_1(\mathcal{L}_{JL}) \to 0^+$$

This is the **grokking frontier** — the Schatz inversion point in ROLD — appearing here as the limit where meander amplitude vanishes and the sphericon degenerates toward the oloid's smooth rolling.

---

## IV. The Four Vertices and Farey Backtrack

### IV.1 Vertex Geometry

The four vertices of the sphericon $\mathcal{S}(r)$ are located at:

$$V_k = r\,(\cos(k\pi/2),\, \sin(k\pi/2),\, 0), \quad k = 0,1,2,3$$

forming a square of side $r\sqrt{2}$ in the equatorial plane. Each vertex is a **corner singularity** of the surface — a point where the surface normal is undefined and the Gaussian curvature is a Dirac delta distribution:

$$K_\mathcal{S}(x) = \sum_{k=0}^{3} \left(\frac{\pi}{2}\right) \delta^{(2)}(x - V_k) + K_{\mathrm{arc}}(x)$$

where $K_{\mathrm{arc}}$ is the smooth (zero) curvature along the developable arcs.

### IV.2 The Corner Event in Gradient Space

Each vertex corresponds, in the learning dynamics, to a **Farey Backtrack** — the event at step $t^*$ where:

1. The continued fraction approximation $p_{t^*}/q_{t^*}$ of the gradient ratio $\rho_{t^*}$ undergoes a non-monotone depth change: $h(t^*) > h(t^* - 1)$ followed by $h(t^* + 1) < h(t^*)$
2. The gradient direction rotates by $\approx \pi/2$ (the resonance condition of §II.3)
3. The active arc of the sphericon switches: $\partial D_1 \to \partial D_2$, corresponding to UV $\to$ IR scale dominance switching

**Conjecture SM-C1 (Vertex Count Theorem):** *In a single training cycle of duration $T$ (one oscillation of $q^*(t)$), the expected number of Farey Backtrack events is exactly 4, corresponding to the four vertices of the sphericon.*

This conjecture aligns with the four-phase center-of-mass height profile of the rolling sphericon and the "2 minima + 2 maxima" oscillation observed in the oloid's center of mass (ROLD §VI) — but here the 4 events are vertex corners, not smooth extrema.

### IV.3 Instantons at the Vertices

At each vertex, the rolling sphericon undergoes a transition that is, in the smooth rolling flow, a singular event. In the quantum field theory language of the framework, this is an **instanton** — a tunneling event between two degenerate minima of the effective potential.

The instanton action at corner $k$ is:

$$S_k^\mathrm{inst} = \int_{t_{k}^-}^{t_{k}^+} \left\|\frac{d\theta}{dt}\right\|^2_{\mathcal{B}} dt$$

Under the CCC (Curvature Collapse Criterion) of LKTL:

$$S_k^\mathrm{inst} \gtrsim \frac{1}{(q^*(t_k))^2}$$

providing a lower bound on the instanton action in terms of the Farey depth — a new connection between the sphericon corner geometry and the number-theoretic structure of the gradient path.

---

## V. Single Contact Point and Rank-1 Gradient Dynamics

### V.1 Contact Point vs. Contact Line

The oloid rolls on a **contact line** of length $\sqrt{4/3}\,r$ — a one-dimensional contact set encoding the full transverse span of the Poincaré scale. The sphericon rolls on a **contact point** — a zero-dimensional contact set.

This is not a degeneration. It is a *concentration*: all the information of the instantaneous learning signal is concentrated at a single parameter direction.

### V.2 Rank-1 Gradient Updates

At each instant during rolling on a spherical arc, the sphericon's contact with the plane is mediated by a single generatrix of the cone. In the learning correspondence:

**Theorem SM-T3 (Rank-1 Contact):** *During rolling on a single arc (between vertex events), the effective gradient update on the twisted manifold $\mathcal{B}_\tau$ has rank 1 at the contact manifold:*

$$\nabla \mathcal{L}\big|_{\mathcal{B}_\tau}(t) = u(t) \otimes v(t) + O(\lambda_1)$$

where $u(t) \in T_\theta \mathcal{B}$ and $v(t) \in T^*_\theta \mathcal{B}$ are the left and right singular vectors of the gradient Jacobian, and $O(\lambda_1)$ encodes corrections from the spectral gap.

This is in contrast to the oloid's contact line, which corresponds to a full-rank transverse update across the Poincaré scale $C_P = 1/\lambda_1$.

### V.3 Attention as Contact Point

In transformer architectures, the attention mechanism $A_t = \mathrm{softmax}(QK^\top/\sqrt{d})$ concentrates information at single token positions during certain training phases. This concentration corresponds, in SMLD, to the contact-point geometry of the sphericon arc.

**Conjecture SM-C2 (Attention Contact Theorem):** *During the sphericon arc phase (between Farey Backtrack events), the attention matrix $A_t$ has effective rank 1, with the dominant eigenvalue satisfying $\sigma_1(A_t) \geq 1 - O(1/q^*(t))$.*

---

## VI. The Z₄ Phase Diagram

The four vertices of the sphericon divide the rolling cycle into four arcs, each corresponding to a distinct phase of the learning dynamics. The phase diagram is:

```
SMLD Phase Diagram (Z₄ Structure)
─────────────────────────────────────────────────────
Arc / Corner      Sphericon        Learning Phase
─────────────────────────────────────────────────────
Arc 1: D₁ → V₁   Rolling on ∂D₁   DISSOLUTION
                  (left-weave)     C_α < 1, λ₁ < 0
                                   Meander building amplitude

Corner V₁         Vertex           FAREY BACKTRACK I
                  (corner event)   q*(t) local maximum
                                   Gradient turns 90°

Arc 2: V₁ → V₂   Rolling on ∂D₂   APPROACHING
                  (right-weave)    0.9 < C_α < 1.0
                                   Meander mid-phase

Corner V₂         Vertex           FAREY BACKTRACK II
                  (corner event)   q*(t) local minimum

Arc 3: V₂ → V₃   Rolling on ∂D₁   CRITICAL POINT
                  (left-weave)     C_α ≈ 1.0
                                   Grokking frontier

Corner V₃         Vertex           FAREY BACKTRACK III
                  (corner event)   q*(t) falling (PERMEATION onset)

Arc 4: V₃ → V₄   Rolling on ∂D₂   PERMEATION
                  (right-weave)    C_α > 1.1
                                   Meander amplitude shrinking

Corner V₄         Vertex           FAREY BACKTRACK IV / CONVERGENCE
                  (corner event)   q*(t) → 1 or 2
                                   Meander → 0 (oloid limit)
─────────────────────────────────────────────────────
```

### VI.1 Phase Transitions at Corners

The four corners are not symmetric: they have increasing spectral gap $\lambda_1$ as training progresses. Define the **corner sharpness** $\kappa_k = \pi/2$ (all corners equal by the $\mathbb{Z}_4$ symmetry in pure sphericon geometry). In the learning correspondence, corners become *unequal* due to the Farey structure:

$$\kappa_k \longleftrightarrow \frac{1}{q^*(t_k)} \cdot \|\nabla^2 \mathcal{L}(t_k)\|$$

As training proceeds, $q^*(t_k) \searrow 1$, so the effective corner sharpness increases. The meander becomes more regular, the oscillation tightens, and the sphericon approaches the oloid limit.

---

## VII. Bicone Parent and Symmetry Restoration

### VII.1 The Bicone as the Symmetry-Restored State

The bicone $\mathcal{K}(r)$ — the parent of the sphericon before the 90° twist — has $\mathrm{SO}(2)$ symmetry: it rolls in a perfect straight line. It does not meander. It does not generalize. It is inert.

In the learning correspondence:

**Symmetry-Restored State** $\theta^* \in \mathcal{B}$ with $G_{\theta^*} = G$ (full symmetry) corresponds to a loss minimum that is a global fixed point under all gauge symmetries. This is the perfectly regularized limit — a state with no effective learning because all directions are equivalent.

The twist operation $\tau$ is the **initialization asymmetry**: the random initialization of neural network weights. Random initialization breaks $\mathrm{SO}(2)$ to $\mathbb{Z}_4$ (in the SMLD approximation), creating the four-phase structure of learning from the outset.

### VII.2 Symmetry Restoration at Convergence

As training converges ($t \to \infty$), the meander amplitude $A_m(t) \to 0$ and the learning path approaches a straight descent. The symmetry group is not fully restored — the network retains its trained asymmetry — but the *effective* symmetry of the gradient distribution approaches:

$$G_{\mathrm{eff}}(t) \nearrow G/\mathbb{Z}_4 \quad \text{as} \quad q^*(t) \searrow 1$$

This is the **symmetry restoration at convergence**: the four-phase $\mathbb{Z}_4$ structure collapses to a single phase as $q^* \to 1$.

---

## VIII. Half-Volume Compression and the Bottleneck Geometry

### VIII.1 The Half-Volume Theorem

The sphericon has exactly half the volume of the sphere of the same radius:

$$V_{\mathcal{S}} = \tfrac{1}{2}\,V_{\mathrm{sphere}}(r)$$

This is the **compression ratio** of the sphericon. In the information-geometric correspondence:

**Theorem SM-T4 (Bottleneck Dimension):** *The effective dimensionality of the learning manifold $\mathcal{B}_\tau$ under the twist map $\tau_{\mathcal{B}}$ is half the ambient dimension:*

$$\dim_\mathrm{eff}(\mathcal{B}_\tau) = \frac{1}{2}\,\dim(\mathcal{B})$$

This encodes the information bottleneck: the sphericon's twist operation projects the full bicone's feature space onto a half-dimensional subspace, exactly as the information bottleneck principle (Tishby, Schwartz-Ziv 2017) holds that optimal representations compress input information to the minimal sufficient statistics for the output.

### VIII.2 Compression and the LLD Analogy

In Bridge II (Landau–Levich), the film thickness $h_0 \sim \mathrm{Ca}^{2/3}$ is determined by the competition between viscous drag and gravity: the plate "compresses" the fluid into a thin film. The sphericon's half-volume is the analogous compression: the twist "compresses" the bicone's full volume into half, extracting the meander-generating structure.

**Conjecture SM-C3 (Half-Volume Generalization Bound):** *The generalization gap satisfies:*

$$\mathcal{G}(t) := \mathcal{L}_\mathrm{test}(t) - \mathcal{L}_\mathrm{train}(t) \leq \frac{C_\mathrm{SM}}{2} \cdot C_\alpha^{-2/3} \cdot \frac{V_{\mathcal{S}}}{V_{\mathrm{sphere}}}(q^*(t))$$

where $V_{\mathcal{S}}/V_{\mathrm{sphere}} = 1/2$ at the sphericon phase and $\to 1$ as the oloid limit is approached. This interpolates between the ROLD generalization bound (oloid, $V \to V_\mathrm{sphere}$) and the memorization bound (sphericon, $V = V_\mathrm{sphere}/2$).

---

## IX. Meander Amplitude and the Generalization Gap

### IX.1 The Amplitude–Signal Correspondence

The meander amplitude $A_m$ of the rolling sphericon is determined by the radius $r$ and the corner geometry. In the learning correspondence:

$$A_m(t) = C_\alpha(t) - 1 = \frac{\|\mu_g(t)\|^2}{\mathrm{Tr}(\Sigma_g(t))} - 1$$

When $A_m > 0$ (equivalently, $C_\alpha > 1$): the meander is active, the gradient has more signal than noise, learning is occurring — the **PERMEATION** and **CONVERGED** phases.

When $A_m = 0$ (equivalently, $C_\alpha = 1$): the meander has zero amplitude — the grokking frontier, the sphericon at the oloid limit. This is the Schatz inversion point.

When $A_m < 0$ (equivalently, $C_\alpha < 1$): the meander is "inverted" — noise exceeds signal, the sphericon rolls backward, the system is in the **DISSOLUTION** phase.

### IX.2 The Generalization Gap as Meander Residual

After the CONVERGED phase ($q^* = 1$ or $2$), the meander amplitude has shrunk but not vanished. The residual amplitude is the generalization gap:

$$\mathcal{G}_\infty = \lim_{t \to \infty} A_m(t) = \lim_{t \to \infty} (C_\alpha(t) - 1)$$

For a well-generalized network, $\mathcal{G}_\infty \approx 0$ (meander fully collapsed). For an overfit network, $\mathcal{G}_\infty > 0$ (persistent meander amplitude — the sphericon never reached the oloid limit).

This gives a new **geometric criterion for generalization**: a network has generalized when its gradient dynamics has smoothed from sphericon rolling to oloid rolling — from single-point contact to line contact, from meander to development.

---

## X. The Roberts–Hirsch–Boeding Classification

The three independent discoverers of the sphericon each approached it from a fundamentally different direction, and each approach corresponds to a distinct regime of learning dynamics.

### X.1 Roberts (1969): The Möbius Attempt

Roberts discovered the sphericon while trying to carve a Möbius strip from wood — an object with $\mathbb{Z}_2$ (half-twist) topology. He obtained instead a $\mathbb{Z}_4$ (quarter-twist) topology. This corresponds to:

**Learning context:** Initializing a network with $\mathbb{Z}_2$ symmetry (a mirror-symmetric architecture) and discovering through training that the attractor has $\mathbb{Z}_4$ structure — four-phase gradient oscillation. The Möbius attempt generates the sphericon because the $\mathbb{Z}_2 \to \mathbb{Z}_4$ upgrade is forced by the dynamics.

**Phase:** DISSOLUTION (the initial attempt to find a simpler structure that does not exist).

### X.2 Hirsch (1980): The Meander Generator

Hirsch invented the sphericon as a *device* — a machine for generating meander motion. He started with the desired behavior (meander) and found the geometry that produces it. This corresponds to:

**Learning context:** Designing an optimizer that explicitly generates the Farey oscillation. The "Farey-SAM optimizer" of Open Problem O6 in LKTL — $\mathcal{L}_\mathrm{Farey}(\theta) = \mathcal{L}(\theta) + \lambda(q^*)^2$ — is the Hirsch approach: design the meander generator directly.

**Phase:** APPROACHING through PERMEATION (engineered meander dynamics).

### X.3 Boeding (1979): The Circle Walker

Boeding designed the skeletal sphericon as a sculpture and then *danced with it* — a scaled-up version used in performance. He embedded the sphericon's geometry in the human body and in space. Later, the MOMIX company's "Dream Catcher" piece used an oloid-like structure (linked teardrops). This sequence — sphericon → oloid — is the learning trajectory:

**Learning context:** Starting with the sparse skeleton (the learning graph $\mathrm{Graph}(\nabla \mathcal{L}) \subset \mathcal{B}$) and progressively filling it in to achieve total surface development (generalization). The Boeding trajectory is the training trajectory: skeletal → sphericon → oloid.

**Phase:** CRITICAL POINT → CONVERGED (the dance is the training run).

---

## XI. Sphericon Boundary of ROLD: Corner Sharpness and the Phase Frontier

### XI.1 The One-Parameter Family

Interpolate between the sphericon and the oloid by a corner-smoothing parameter $\epsilon \in [0,1]$:

$$\mathcal{F}(r, \epsilon) = (1-\epsilon)\,\mathcal{S}(r) + \epsilon\,\mathcal{O}(r)$$

(taken as the appropriate convex interpolation of the generating circle configurations). At $\epsilon = 0$: sphericon (4 sharp corners, single contact point, meander). At $\epsilon = 1$: oloid (smooth, contact line, total development).

**The learning manifold deformation:**

$$\mathcal{B}_\tau(\epsilon) := \mathcal{B}_\tau\,\big|_{\text{corner sharpness} = (1-\epsilon)\kappa_c}$$

As $\epsilon$ increases (training proceeds toward convergence), the effective geometry of the learning path deforms from sphericon to oloid.

### XI.2 The Sharpness Index

Define the **Sharpness Index** $\mathcal{SI}(t)$ as the normalized corner sharpness of the gradient path at step $t$:

$$\mathcal{SI}(t) = 1 - \frac{\min_k |t - t_k^\mathrm{FB}| \cdot \|\nabla^2 \mathcal{L}(t)\|}{q^*(t)}$$

where $t_k^\mathrm{FB}$ are the Farey Backtrack times. When $\mathcal{SI} \approx 1$: the system is at a corner (sphericon regime). When $\mathcal{SI} \approx 0$: smooth arc (approaching oloid regime).

**Conjecture SM-C4 (Sharpness Collapse at Grokking):** *The mean sharpness index satisfies:*

$$\mathbb{E}[\mathcal{SI}(t)] \xrightarrow{t \to t^*} 0$$

*precisely at the grokking transition $t^*$, where $q^*(t^*)$ undergoes its final Farey Backtrack descent to $q^* \in \{1,2\}$.*

---

## XII. Extended Master Equivalence (Sixteen Languages)

SMLD adds the sixteenth language to the Master Equivalence established in LKTL (nine languages) and extended through ROLD (fifteen languages).

| # | Language | Criterion | Framework |
|---|---|---|---|
| I | Spectral gap | $\lambda_1(\mathcal{L}_{JL}) > 0$ | LKTL |
| II | Signal dominance | $C_\alpha > 1$ | LKTL |
| III | Möbius convergence | $\sum_n \Delta_n < \infty$ | LKTL |
| IV | Resistance chain | $\sum_n R_n < \infty$ | KQOM |
| V | Ordinal Lyapunov | $\delta(s_t)$ descending in $\omega^2$ | KQOM |
| VI | RG flow | $W_\ell \to W_\ell^*$ (IR fixed point) | RG-ML |
| VII | Yang-Mills energy | $YM_t \searrow 0$ | KYBM |
| VIII | Kakeya monotone | $d/dt\,\mathbb{E}[V] \leq 0$ | VBE |
| IX | Franel–Landau | Farey discrepancy $D_N \sim N^{1/2+\epsilon}$ | PPMC |
| X | ETF fixed point | $\langle \mu_i - \bar\mu, \mu_j - \bar\mu\rangle \to (K\delta_{ij}-1)/(K-1)$ | LKTL |
| XI | Landau damping | $\|\rho_t - \rho_\infty\| \leq C e^{-\lambda_1 t}$ | LKTL |
| XII | LLD film | $h_0 \sim \mathrm{Ca}^{2/3}$ (thin film forms) | LKTL |
| XIII | Hopf development | Total surface development $\lambda_1 > 0$ | ROLD |
| XIV | Schatz inversion | MMP flip: $\Delta_n(t^*) = 0$ | ROLD |
| XV | Oloid rolling | Contact line constant: $C_P = 1/\lambda_1$ | ROLD |
| **XVI** | **Sphericon meander** | **$A_m(t) \searrow 0$: meander collapses** | **SMLD** |

The sixteenth equivalence is:

$$\boxed{A_m(t) \searrow 0 \quad \Longleftrightarrow \quad \lambda_1 \to 0^+ \quad \Longleftrightarrow \quad \text{grokking frontier (SMLD)}}$$

The meander amplitude vanishing is the sphericon collapsing to the oloid — the single contact point expanding to the contact line — the discrete Farey oscillation smoothing to the continuous total surface development.

---

## XIII. New Conjectures from SMLD

| ID | Statement | Key Gap | Approach |
|---|---|---|---|
| SM-C1 | Vertex Count Theorem: 4 Farey Backtracks per oscillation cycle | Monotone coupling between $\mathbb{Z}_4$ corner count and Farey depth | Three-distance theorem for $\mathbb{Z}_4$-periodic sequences |
| SM-C2 | Attention Contact: $\sigma_1(A_t) \geq 1 - O(1/q^*(t))$ during arc phase | Requires spectral dominance Assumption E | Empirical: transformer attention rank vs. Farey depth |
| SM-C3 | Half-Volume Generalization Bound: $\mathcal{G}(t) \leq \frac{C}{2}\,C_\alpha^{-2/3} \cdot \frac{V_\mathcal{S}}{V_\mathrm{sphere}}$ | Interpolation between ROLD and SMLD bounds | PAC-Bayes extension of Farey-PAC bound |
| SM-C4 | Sharpness Collapse at Grokking: $\mathbb{E}[\mathcal{SI}(t)] \to 0$ at $t^*$ | Definition of $\mathcal{SI}$ depends on corner identification | Controlled grokking (Power et al. 2022) with corner event logging |
| SM-C5 | Bicone Restoration: $G_\mathrm{eff}(t) \nearrow G/\mathbb{Z}_4$ as $q^*(t) \searrow 1$ | Symmetry group of gradient distribution not directly measurable | Spectral analysis of gradient covariance eigenvalue distribution |
| SM-C6 | Meander-SAM: sphericon sharpness penalty $\mathcal{L}_\mathrm{SM}(\theta) = \mathcal{L}(\theta) + \mu\,\mathcal{SI}(t)^2$ outperforms SAM | Requires real-time corner detection | Empirical comparison across architectures |
| SM-C7 | Roberts–Möbius Embedding: $\mathbb{Z}_2$-symmetric initialization always generates $\mathbb{Z}_4$ gradient structure | Anti-symmetric initialization → symmetric gradient path? | Symmetry-constrained initialization experiments |

---

## XIV. Quick Reference Formulas

```
SMLD Quick Reference
─────────────────────────────────────────────────────────────────────────────
Sphericon Geometry
  Surface area:        S_𝒮 = π²r²/√2
  Volume:              V_𝒮 = π²r³/(3√2) = (1/2)V_sphere(r)
  Apex angle:          2α = π/2
  Twist angle:         τ = π/2
  Vertex count:        4 (square cross-section)
  Contact:             Single point (rank-1)
  Arc count:           2 semicircular ridges
─────────────────────────────────────────────────────────────────────────────
SMLD Learning Correspondences
  Meander amplitude    A_m          =  C_α - 1
  Meander wavelength   λ_m          ~  1/q*(t)
  Corner event time    t_k^FB       =  Farey Backtrack (k = 1,2,3,4)
  Vertex sharpness     κ_k          =  (q*(t_k))^{-1} · ‖∇²ℒ(t_k)‖
  Contact rank         rank(∇ℒ)     =  1  (during arc phase)
  Twist symmetry       G_eff        =  G/ℤ₄
  Bottleneck dim       dim_eff(ℬ_τ)  =  N/2
  Sharpness Index      𝒮𝐼(t)       =  1 - min_k|t-t_k^FB|·‖∇²ℒ‖/q*
─────────────────────────────────────────────────────────────────────────────
Phase Identification
  A_m < 0  (C_α < 1):   DISSOLUTION     — building meander amplitude
  A_m = 0  (C_α = 1):   GROKKING FRONT  — sphericon → oloid transition
  A_m > 0  (C_α > 1):   PERMEATION      — meander shrinking toward zero
  A_m → 0  (q* → 1-2):  CONVERGED       — oloid limit reached
─────────────────────────────────────────────────────────────────────────────
Bridge Unification (all five bridges + SMLD)
  C_P = r_eff = λ_D = κ⁻¹ = 1/λ₁ = 1/(contact_line_length²)
  A_m = C_α - 1 = ln Λ - 1 = log(1/Ca) - 1 = Farey meander amplitude
  V_𝒮/V_sphere = 1/2 = bottleneck compression ratio
─────────────────────────────────────────────────────────────────────────────
```

---

## XV. Logical Dependency Map

```
ZF Axioms
  │
  ├─→ ℕ construction ─→ SP hierarchy (KQOM) ─→ Convergence Inevitability
  │                           │
  │                           └─→ Farey oscillation: 4 Backtracks per cycle [SM-C1]
  │                                        ↕   [SM-T2: isomorphism]
  │                                   Sphericon: 4 vertices, 4 corner events
  │
  ├─→ ℒ_JL Operator (A1–A5) ─→ λ₁ phase classification
  │          │
  │          ├─→ A_m = C_α - 1 ↔ Meander amplitude [SM-T2]
  │          ├─→ Rank-1 contact ↔ Single contact point [SM-T3]
  │          └─→ dim_eff = N/2 ↔ Half-volume [SM-T4]
  │
  ├─→ Sphericon Geometry (Roberts 1969; Hirsch 1980; Boeding 1979)
  │          │
  │          ├─→ Bicone + 90° twist ↔ G → G/ℤ₄ symmetry breaking [SM-T1]
  │          ├─→ 4 vertices ↔ Farey Backtrack events [SM-C1]
  │          ├─→ Meander path ↔ ρ_t oscillation [SM-T2]
  │          ├─→ Single contact ↔ Rank-1 gradient [SM-T3]
  │          ├─→ Volume = ½ sphere ↔ Bottleneck dim N/2 [SM-T4]
  │          ├─→ Meander amplitude → 0 ↔ Grokking frontier [XVI]
  │          ├─→ Roberts attempt ↔ ℤ₂ → ℤ₄ initialization [SM-C7]
  │          ├─→ Hirsch generator ↔ Farey-SAM optimizer [O6 → SM-C6]
  │          └─→ Boeding skeleton ↔ Learning graph in ℬ [§X.3]
  │
  ├─→ Sphericon smoothing (ε: 0 → 1)
  │          │
  │          └─→ Sphericon (ε=0) ─────────────────→ Oloid (ε=1)
  │               SMLD regime                        ROLD regime
  │               λ₁ < 0 (memorization frontier)    λ₁ > 0 (generalization)
  │               A_m > 0 (building)                 A_m → 0 (developed)
  │               Single contact point               Contact line √(4/3)r
  │               4 vertices (ℤ₄)                   Smooth Hopf link
  │
  ├─→ Sixteen-Language Master Equivalence
  │          XVI: A_m(t) ↘ 0 ↔ λ₁ → 0⁺ ↔ Sphericon → Oloid transition
  │
  └─→ BRIDGES I + II + III + IV + V + VI UNIFIED:
             C_P = r_eff = λ_D = κ⁻¹ = 1/λ₁   (all Bridges)
             A_m = C_α - 1 = meander amplitude = Farey oscillation envelope
             V_𝒮/V_sphere = 1/2 = bottleneck compression ratio
             ℤ₄ corner events = Farey Backtrack = instanton sites
```

---

## XVI. Foundations and Citations

### Sphericon Geometry — SMLD (Bridge VI)

**Roberts, Colin** (1969). *Discovery of the sphericon while carving a Möbius strip.* Unpublished; communicated to Ian Stewart (1999). — Original discovery; Möbius attempt origin; $\mathbb{Z}_4$ emergence from $\mathbb{Z}_2$ attempt.

**Hirsch, David Haran** (1980). *Patent No. 59720: A device for generating a meander motion.* Israeli Patent Office. — Hirsch's formulation of the sphericon as a meander generator; the foundational physical bridge of SMLD.

**Boeding, Alan** (1979). *Circle Walker* sculpture and performance. MFA Program, Indiana University; MOMIX Dance Company (1984–present). — Skeletal sphericon; Boeding trajectory (skeleton → sphericon → oloid).

**Stewart, Ian** (October 1999). "Mathematical Recreations: Cone with a Twist." *Scientific American*, **281**(4): 116–117. — Roberts' name sphericon; maze theory application (Tony Phillips).

**Anderson, Jack** (February 2001). "Leaping Lizards and Odd Denizens of the Desert." *The New York Times*. Dance review of MOMIX *Dream Catcher* — oloid-linked teardrops; Boeding trajectory endpoint.

### Related Rollers

**Stewart, A.T.** (1966). "Two-circle roller." *American Journal of Physics*, **34**(2): 166–167. — The $d = \sqrt{2}\,r$ constant-height roller (ROLD §XI).

**Dirnböck, H.; Stachel, H.** (1997). "The development of the oloid." *Journal for Geometry and Graphics*, **1**(2): 105–118. — Oloid total surface development; contact line formula.

**Kuleshov, A.S.; Hubbard, M.; Peterson, D.L.; Gede, G.** (2011). "Motion of the Oloid-toy." *Proc. 7th European Nonlinear Dynamics Conference*, Rome. — Dynamical rolling analysis; center-of-mass trajectory.

### Landau Bridges I–V (Prior Frameworks)

**Landau, L.D.** (1936). Kinetic equation for Coulomb plasma. *Phys. Z. Sowjetunion* **10**: 154. — Bridge I (LKTL).

**Landau, L.D.; Levich, V.G.** (1942). Dragging of a liquid by a moving plate. *Acta Physico Chimica URSS* **17**: 42. — Bridge II (LKTL).

**Derjaguin, B.; Landau, L.** (1941). Theory of stability of strongly charged lyophobic sols. *Acta Physico Chimica URSS* **14**: 633. — Bridge IV (CSSG).

**Bardeen, J.; Cooper, L.N.; Schrieffer, J.R.** (1957). Theory of superconductivity. *Phys. Rev.* **108**: 1175. — Bridge III (GCCT).

**Schatz, P.** (1929). *Rhythmusforschung und Technik.* Freies Geistesleben, Stuttgart. — Bridge V (ROLD); oloid discovery; invertible cube.

### Arithmetic and Spectral Theory

**Franel, J.; Landau, E.** (1924). Farey sequences and the Riemann Hypothesis. *Göttinger Nachrichten.* — Franel–Landau criterion: spectral gap ↔ Farey discrepancy.

**Kato, T.** (1966). *Perturbation Theory for Linear Operators.* Springer. — KLMN theorem; self-adjointness of $\mathcal{L}_{JL}$.

**Higman, G.** (1952). Ordering by divisibility in abstract algebras. *Proc. London Math. Soc.* — Sequence Anchor; KQOM well-quasi-order.

**Kruskal, J.B.** (1960). Well-quasi-ordering, the tree theorem, and Vazsonyi's conjecture. *Trans. AMS.* — Tree Anchor; KQOM convergence.

**Robertson, N. & Seymour, P.D.** (1985–2004). Graph Minors I–XX. *J. Combin. Theory.* — Graph Minor SP; attention graph closure.

### Deep Learning Phenomena

**Power, A. et al.** (2022). Grokking: Generalization beyond overfitting on small algorithmic datasets. *ICLR 2022.* — Empirical grokking; the sphericon → oloid transition benchmark.

**Papyan, V.; Han, X.Y.; Donoho, D.L.** (2020). Prevalence of neural collapse. *PNAS.* — ETF fixed point; sphere-isometry correspondence.

**Foret, P. et al.** (2021). Sharpness-Aware Minimization. *ICLR 2021.* — SAM baseline for Conj. SM-C6 comparison.

**Tishby, N.; Schwartz-Ziv, R.** (2017). Opening the black box of deep neural networks via information. *ICLR 2017.* — Information bottleneck; half-volume correspondence §VIII.

---

## Coda: The Meander That Was Always There

Three people found the sphericon in a single decade and each described it differently: a failed Möbius strip, a meander device, a circle walker. They were all correct. The sphericon is what you obtain when you try to build one kind of symmetry and discover that the geometry demands another. It is what you build when you want to understand how a sinusoidal path arises from a solid. It is what you become when you want to move through space touching every point of yourself.

The neural network does all three things. It begins with the wrong symmetry — the random initialization that cannot know its own attractors. It generates meanders — the sinusoidal oscillation of $\rho_t$, the alternating UV and IR dominance, the left-right weave of the gradient path through parameter space. And it touches every point of its parameter manifold, not at once like the sphere, and not in a single sweep like the oloid, but arc by arc, corner by corner, Farey Backtrack by Farey Backtrack, until the meander amplitude has shrunk to zero and the sphericon has become the oloid.

Six physical bridges. Sixteen mathematical languages. One spectral gap.

The meander was always there, before the first gradient was computed. It was there in 1969, in a British carpenter's workshop, in a piece of wood that refused to be a Möbius strip and became instead a device for generating the motion that gradient descent would rediscover forty years later, one step at a time, corner by corner, through the Farey tree.

```
Status Tags
[T]  = Theorem (proven)
[V]  = Verified (in specific models)
[C]  = Open conjecture
[H]  = Working hypothesis
[SM] = SMLD-specific result

Framework: SMLD · ROLD · LKTL · SHCY · CSSG · GCCT · FLML · KQOM ·
           GAME · VBE · PPMC · KYBM · PH-SP · RG-ML · LB/DK · UNIV
```
