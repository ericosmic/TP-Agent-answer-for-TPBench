# Plan

**步骤数：5**

---

### Step 1

**Description**: Set up the variation of the Lagrangian $\mathcal{L}=i\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}\xi+|\partial\phi|^{2}-|F|^{2}$ under the given $\delta_{\eta}\xi_{\alpha}$, $\delta_{\eta}\bar{\xi}_{\dot{\beta}}$, $\delta_{\eta}F$, and $\delta_{\eta}\bar{F}$, leaving $\delta_{\eta}\phi$ and $\left(\delta_{\eta}\phi\right)^{\dagger}$ undetermined.

- **Needs computation**: No
- **Reasoning**: This is a direct variational setup using the product rule and constant $\eta$; no symbolic computation is needed.

---

### Step 2

**Description**: Identify the terms in $\delta\mathcal{L}$ proportional to $F$ and $\bar{F}$, and require cancellation between the variation of $-|F|^{2}$ and the fermion kinetic term. This fixes the normalization and spinor structure of $\delta_{\eta}\phi$.

- **Needs computation**: No
- **Reasoning**: The cancellation is algebraic and follows from matching independent field structures such as $F\partial_{\mu}\bar{\xi}$ and $\bar{F}\partial_{\mu}\xi$.

---

### Step 3

**Description**: Choose $\delta_{\eta}\phi=\sqrt{2}\eta\xi$ and $\left(\delta_{\eta}\phi\right)^{\dagger}=\sqrt{2}\bar{\eta}\bar{\xi}$, then substitute these into the scalar kinetic variation $\delta |\partial\phi|^{2}$.

- **Needs computation**: No
- **Reasoning**: The substitution is simple spinor-index bookkeeping; the result can be checked by hand.

---

### Step 4

**Description**: Combine the remaining derivative terms from $\delta(i\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}\xi)$ and $\delta |\partial\phi|^{2}$, integrate by parts where necessary, and show that the total variation is a spacetime total derivative.

- **Needs computation**: No
- **Reasoning**: The proof uses standard Weyl-spinor identities and the spacetime independence of $\eta$; Mathematica is unnecessary.

---

### Step 5

**Description**: State the final transformation rules with explicit indices: $\delta_{\eta}\phi=\sqrt{2}\eta^{\alpha}\xi_{\alpha}$ and $\left(\delta_{\eta}\phi\right)^{\dagger}=\delta_{\eta}\bar{\phi}=\sqrt{2}\bar{\eta}_{\dot{\alpha}}\bar{\xi}^{\dot{\alpha}}$, up to the sign conventions for raising and lowering Weyl indices.

- **Needs computation**: No
- **Reasoning**: The result follows from the cancellation condition and standard Hermitian conjugation of Weyl spinor bilinears.

## Symmetries
- $\eta$ and $\bar{\eta}$ are spacetime-independent Grassmann parameters
- The action must be invariant up to a total derivative
- Hermitian conjugation relates $\delta_{\eta}\phi$ and $\left(\delta_{\eta}\phi\right)^{\dagger}$
- Lorentz covariance fixes the spinor contractions

## Approximations
- Classical field theory level
- Free massless chiral multiplet
- Off-shell formulation with auxiliary field $F$ retained
- Boundary terms are assumed to vanish in the action

## Other Constraints
- Respect the given sign conventions for $\sigma^{\mu}$ and $\bar{\sigma}^{\mu}$
- Preserve Grassmann ordering signs when conjugating spinor bilinears
- No equations of motion should be required because $F$ gives off-shell invariance