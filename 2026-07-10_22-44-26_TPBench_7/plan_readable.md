# Plan

**步骤数：5**

---

### Step 1

**Description**: Identify the relevant tree-level process from $\mathcal{L}=\sum_{i=1}^2\left[\frac{1}{2}(\partial_\mu\phi_i)(\partial^\mu\phi_i)-\frac{m_i^2}{2}\phi_i\phi_i\right]-\frac{\lambda}{4}\phi_1^2\phi_2^2$ and extract the quartic vertex for $\phi_1\phi_1\phi_2\phi_2$.

- **Needs computation**: No
- **Reasoning**: The Feynman rule follows directly from differentiating the interaction term $-\frac{\lambda}{4}\phi_1^2\phi_2^2$; no symbolic computation is needed.

---

### Step 2

**Description**: Compute the leading invariant amplitude $\mathcal{M}$ for $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)\to\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$ and note that accuracy to $O(\lambda^2)$ in the cross section requires only the tree amplitude, since $|\mathcal{M}_{\rm tree}|^2=O(\lambda^2)$.

- **Needs computation**: No
- **Reasoning**: The amplitude is a single contact diagram, so the order counting and modulus squared are immediate by hand.

---

### Step 3

**Description**: Write the general CM-frame two-body differential cross section formula for identical final particles, including the phase-space factor $\frac{|\vec{k}_1'|}{|\vec{k}_1|}$ and the symmetry factor $\frac{1}{2!}$ for the two final $\phi_2$ particles.

- **Needs computation**: No
- **Reasoning**: This is a standard relativistic scattering formula and does not require Mathematica.

---

### Step 4

**Description**: Express $|\vec{k}_1|$ and $|\vec{k}_1'|$ in terms of the Mandelstam variable $s$ and masses $m_1,m_2$ using $|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}$ and $|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}$, equivalently through the Källén function.

- **Needs computation**: No
- **Reasoning**: The CM kinematics for equal-mass incoming and outgoing pairs is elementary and can be derived analytically.

---

### Step 5

**Description**: Combine the amplitude and phase space to obtain $\frac{d\sigma}{d\Omega}$ to $O(\lambda^2)$, optionally indicating that the result is angle-independent and depends on Mandelstam variables through $s$ with $s+t+u=2m_1^2+2m_2^2$.

- **Needs computation**: No
- **Reasoning**: Substitution into the cross-section formula is straightforward algebra.

## Symmetries
- Identical incoming particles $\phi_1\phi_1$ and identical final particles $\phi_2\phi_2$
- Final-state symmetry factor $\frac{1}{2!}$ for two identical $\phi_2$ particles
- Rotational invariance in the CM frame implies an angle-independent tree-level contact contribution

## Approximations
- Keep terms through $O(\lambda^2)$ in $\frac{d\sigma}{d\Omega}$
- Use only the tree-level contact amplitude; loop corrections start contributing beyond this order in the cross section
- Kinematic threshold condition $s\ge 4m_2^2$ for production of two $\phi_2$ particles

## Other Constraints
- Use relativistic normalization conventions consistent with $d\sigma/d\Omega=\frac{1}{64\pi^2s}\frac{|\vec{k}_f|}{|\vec{k}_i|}|\mathcal{M}|^2$ before applying identical-particle factors
- Clarify the distinction between the coupling symbol $\lambda$ and the Källén function if both are used