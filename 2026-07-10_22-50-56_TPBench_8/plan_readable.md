# Plan

**步骤数：6**

---

### Step 1

**Description**: Diagonalize the Hamiltonian $H=\sum_{i=1}^{2}\frac{1}{2}\left(\frac{p_{i}^{2}}{m}+kx_{i}^{2}\right)+g\frac{(x_{1}-x_{2})^{2}}{2}$ by introducing normal coordinates $x_{+}=\frac{x_{1}+x_{2}}{\sqrt{2}}$, $x_{-}=\frac{x_{1}-x_{2}}{\sqrt{2}}$ and their conjugate momenta, giving frequencies $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

- **Needs computation**: No
- **Reasoning**: This is a standard two-oscillator normal-mode transformation and can be done analytically by hand.

---

### Step 2

**Description**: Write the ground-state wavefunction $\Omega(x_{1},x_{2})=\langle x_{1},x_{2}|\Omega\rangle$ as a product of Gaussian normal-mode vacua, then express it in the original coordinates $x_{1},x_{2}$.

- **Needs computation**: No
- **Reasoning**: The ground state of decoupled harmonic modes is a known Gaussian; substituting $x_{\pm}$ is straightforward algebra.

---

### Step 3

**Description**: Use the definition of $\hat{\rho}$ to form the reduced density-matrix kernel $\rho(x_{1}'',x_{1}')=\int dw\,\Omega(x_{1}'',w)\Omega^{*}(x_{1}',w)$ after tracing over the $|w\rangle_{x_{2}}$ components satisfying $\hat{x}_{2}|w\rangle_{x_{2}}=w|w\rangle_{x_{2}}$.

- **Needs computation**: No
- **Reasoning**: The integral over $w$ is a one-dimensional Gaussian integral with parameters determined by $\omega_{+}$ and $\omega_{-}$; it is manageable analytically.

---

### Step 4

**Description**: Identify $\rho(x_{1}'',x_{1}')$ with the thermal density matrix of an effective single oscillator, or equivalently compute the symplectic eigenvalue $\nu=\sqrt{\langle x_{1}^{2}\rangle\langle p_{1}^{2}\rangle}/\hbar$ of the reduced Gaussian state.

- **Needs computation**: No
- **Reasoning**: For a one-mode Gaussian reduced state, the entropy depends only on the symplectic eigenvalue; the needed correlators follow directly from the normal-mode variances.

---

### Step 5

**Description**: Evaluate $\nu$ explicitly using $\langle x_{1}^{2}\rangle=\frac{\hbar}{4m}\left(\frac{1}{\omega_{+}}+\frac{1}{\omega_{-}}\right)$ and $\langle p_{1}^{2}\rangle=\frac{\hbar m}{4}\left(\omega_{+}+\omega_{-}\right)$, giving $\nu=\frac{1}{4}\frac{\omega_{+}+\omega_{-}}{\sqrt{\omega_{+}\omega_{-}}}$.

- **Needs computation**: No
- **Reasoning**: The simplification is elementary algebra; no symbolic engine is needed.

---

### Step 6

**Description**: Insert $\nu$ into the one-mode Gaussian entropy formula $S=\left(\nu+\frac{1}{2}\right)\ln\left(\nu+\frac{1}{2}\right)-\left(\nu-\frac{1}{2}\right)\ln\left(\nu-\frac{1}{2}\right)$ and express the result in terms of $k$, $g$, and $m$, noting that $m$ cancels through the ratio $\omega_{-}/\omega_{+}=\sqrt{1+2g/k}$.

- **Needs computation**: No
- **Reasoning**: The final substitution is analytic and compact; Mathematica is unnecessary unless one wants alternative algebraic forms.

## Symmetries
- Exchange symmetry $x_{1}\leftrightarrow x_{2}$ of the Hamiltonian $H$
- Canonical preservation of commutation relations under the transformation to $x_{+}$ and $x_{-}$
- Purity of the full ground state $|\Omega\rangle$ before tracing

## Approximations
- No approximation is required; the result is exact for the quadratic Hamiltonian
- Stability requires $k>0$ and $k+2g>0$ so that $\omega_{+}$ and $\omega_{-}$ are real
- For $g=0$, $\omega_{+}=\omega_{-}$, hence $\nu=\frac{1}{2}$ and $S=0$

## Other Constraints
- Use natural logarithms in $S=-\mathrm{Tr}_{x_{1}}\left[\hat{\rho}\ln\hat{\rho}\right]$
- The trace $\mathrm{Tr}_{x_{1}}$ is over the reduced Hilbert space of oscillator $x_{1}$
- The coordinate eigenstates $|w\rangle_{x_{2}}$ are distribution-normalized, so Gaussian kernels should be interpreted in the usual continuum normalization