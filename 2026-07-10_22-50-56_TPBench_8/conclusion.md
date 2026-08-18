## Solution Plan
  1. Diagonalize the Hamiltonian $H=\sum_{i=1}^{2}\frac{1}{2}\left(\frac{p_{i}^{2}}{m}+kx_{i}^{2}\right)+g\frac{(x_{1}-x_{2})^{2}}{2}$ by introducing normal coordinates $x_{+}=\frac{x_{1}+x_{2}}{\sqrt{2}}$, $x_{-}=\frac{x_{1}-x_{2}}{\sqrt{2}}$ and their conjugate momenta, giving frequencies $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.
  2. Write the ground-state wavefunction $\Omega(x_{1},x_{2})=\langle x_{1},x_{2}|\Omega\rangle$ as a product of Gaussian normal-mode vacua, then express it in the original coordinates $x_{1},x_{2}$.
  3. Use the definition of $\hat{\rho}$ to form the reduced density-matrix kernel $\rho(x_{1}'',x_{1}')=\int dw\,\Omega(x_{1}'',w)\Omega^{*}(x_{1}',w)$ after tracing over the $|w\rangle_{x_{2}}$ components satisfying $\hat{x}_{2}|w\rangle_{x_{2}}=w|w\rangle_{x_{2}}$.
  4. Identify $\rho(x_{1}'',x_{1}')$ with the thermal density matrix of an effective single oscillator, or equivalently compute the symplectic eigenvalue $\nu=\sqrt{\langle x_{1}^{2}\rangle\langle p_{1}^{2}\rangle}/\hbar$ of the reduced Gaussian state.
  5. Evaluate $\nu$ explicitly using $\langle x_{1}^{2}\rangle=\frac{\hbar}{4m}\left(\frac{1}{\omega_{+}}+\frac{1}{\omega_{-}}\right)$ and $\langle p_{1}^{2}\rangle=\frac{\hbar m}{4}\left(\omega_{+}+\omega_{-}\right)$, giving $\nu=\frac{1}{4}\frac{\omega_{+}+\omega_{-}}{\sqrt{\omega_{+}\omega_{-}}}$.
  6. Insert $\nu$ into the one-mode Gaussian entropy formula $S=\left(\nu+\frac{1}{2}\right)\ln\left(\nu+\frac{1}{2}\right)-\left(\nu-\frac{1}{2}\right)\ln\left(\nu-\frac{1}{2}\right)$ and express the result in terms of $k$, $g$, and $m$, noting that $m$ cancels through the ratio $\omega_{-}/\omega_{+}=\sqrt{1+2g/k}$.

---

## Execution Step Results

### Step 1: Diagonalize the Hamiltonian $H=\sum_{i=1}^{2}\frac{1}{2}\left(\frac{p_{i}^{2}}{m}+kx_{i}^{2}\right)+g\frac{(x_{1}-x_{2})^{2}}{2}$ by introducing normal coordinates $x_{+}=\frac{x_{1}+x_{2}}{\sqrt{2}}$, $x_{-}=\frac{x_{1}-x_{2}}{\sqrt{2}}$ and their conjugate momenta, giving frequencies $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

**Reasoning:**
The transformation to $x_{+}$ and $x_{-}$ is an orthogonal rotation in the two-dimensional coordinate space, so it preserves quadratic sums such as $x_1^2+x_2^2$ and, with the same transformation applied to the momenta, preserves $p_1^2+p_2^2$ and the canonical commutation relations. The coupling depends only on the relative displacement $x_1-x_2$, which becomes $\sqrt{2}x_{-}$. Hence the coupling contributes $g(x_1-x_2)^2/2=g x_{-}^2$, modifying only the spring constant of the antisymmetric mode. The symmetric mode retains spring constant $k$, while the antisymmetric mode has effective spring constant $k+2g$. Comparing each quadratic potential term to $m\omega^2x^2/2$ gives $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

**Result:**
Introduce the orthogonal canonical transformation
$$
x_{+}=\frac{x_1+x_2}{\sqrt{2}},\qquad x_{-}=\frac{x_1-x_2}{\sqrt{2}},
$$
with inverse
$$
x_1=\frac{x_{+}+x_{-}}{\sqrt{2}},\qquad x_2=\frac{x_{+}-x_{-}}{\sqrt{2}}.
$$
The conjugate momenta are
$$
p_{+}=\frac{p_1+p_2}{\sqrt{2}},\qquad p_{-}=\frac{p_1-p_2}{\sqrt{2}},
$$
so that
$$
p_1=\frac{p_{+}+p_{-}}{\sqrt{2}},\qquad p_2=\frac{p_{+}-p_{-}}{\sqrt{2}}.
$$
Because this transformation is orthogonal and canonical,
$$
p_1^2+p_2^2=p_{+}^2+p_{-}^2,
$$
while
$$
x_1^2+x_2^2=x_{+}^2+x_{-}^2,
$$
and
$$
x_1-x_2=\sqrt{2}\,x_{-}.
$$
Therefore the Hamiltonian becomes
$$
H=\frac{p_{+}^2}{2m}+\frac{1}{2}k x_{+}^2+\frac{p_{-}^2}{2m}+\frac{1}{2}(k+2g)x_{-}^2.
$$
Equivalently,
$$
H=\left[\frac{p_{+}^2}{2m}+\frac{1}{2}m\omega_{+}^2x_{+}^2\right]+\left[\frac{p_{-}^2}{2m}+\frac{1}{2}m\omega_{-}^2x_{-}^2\right],
$$
with normal-mode frequencies
$$
\omega_{+}=\sqrt{\frac{k}{m}},\qquad \omega_{-}=\sqrt{\frac{k+2g}{m}}.
$$
Thus the Hamiltonian diagonalizes into two independent harmonic oscillators: the symmetric mode $x_{+}$ with frequency $\omega_{+}$ and the antisymmetric mode $x_{-}$ with frequency $\omega_{-}$.

**Analysis:**
The transformation to $x_{+}$ and $x_{-}$ is an orthogonal rotation in the two-dimensional coordinate space, so it preserves quadratic sums such as $x_1^2+x_2^2$ and, with the same transformation applied to the momenta, preserves $p_1^2+p_2^2$ and the canonical commutation relations. The coupling depends only on the relative displacement $x_1-x_2$, which becomes $\sqrt{2}x_{-}$. Hence the coupling contributes $g(x_1-x_2)^2/2=g x_{-}^2$, modifying only the spring constant of the antisymmetric mode. The symmetric mode retains spring constant $k$, while the antisymmetric mode has effective spring constant $k+2g$. Comparing each quadratic potential term to $m\omega^2x^2/2$ gives $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

### Step 2: Write the ground-state wavefunction $\Omega(x_{1},x_{2})=\langle x_{1},x_{2}|\Omega\rangle$ as a product of Gaussian normal-mode vacua, then express it in the original coordinates $x_{1},x_{2}$.

**Reasoning:**
After diagonalization, the Hamiltonian is a sum of two independent harmonic oscillator Hamiltonians, one in $x_+$ and one in $x_-$. Therefore its ground state is the tensor product of the individual oscillator ground states. Each oscillator ground state is a normalized Gaussian with width set by $m\omega_\pm/\hbar$. Since the transformation from $(x_1,x_2)$ to $(x_+,x_-)$ is orthogonal with unit Jacobian, no additional Jacobian factor is introduced in the normalized wavefunction. Substituting $x_+=(x_1+x_2)/\sqrt{2}$ and $x_-=(x_1-x_2)/\sqrt{2}$ gives the original-coordinate form.

**Result:**
Since the Hamiltonian is diagonal in the normal coordinates, the ground state factorizes into the product of the two normal-mode oscillator vacua:

$$
\Omega(x_+,x_-)=\left(\frac{m\omega_+}{\pi\hbar}\right)^{1/4}
\left(\frac{m\omega_-}{\pi\hbar}\right)^{1/4}
\exp\left[-\frac{m}{2\hbar}\left(\omega_+ x_+^2+\omega_- x_-^2\right)\right].
$$

Equivalently,

$$
\Omega(x_+,x_-)=\left(\frac{m^2\omega_+\omega_-}{\pi^2\hbar^2}\right)^{1/4}
\exp\left[-\frac{m}{2\hbar}\left(\omega_+ x_+^2+\omega_- x_-^2\right)\right].
$$

Using

$$
x_+=\frac{x_1+x_2}{\sqrt{2}},\qquad x_- = \frac{x_1-x_2}{\sqrt{2}},
$$

the wavefunction in the original coordinates is

$$
\boxed{
\Omega(x_1,x_2)=\left(\frac{m^2\omega_+\omega_-}{\pi^2\hbar^2}\right)^{1/4}
\exp\left[-\frac{m}{4\hbar}\left\{\omega_+(x_1+x_2)^2+\omega_-(x_1-x_2)^2\right\}\right]
}
$$

with

$$
\omega_+=\sqrt{\frac{k}{m}},\qquad \omega_- = \sqrt{\frac{k+2g}{m}}.
$$

Expanding the exponent gives

$$
\Omega(x_1,x_2)=\left(\frac{m^2\omega_+\omega_-}{\pi^2\hbar^2}\right)^{1/4}
\exp\left[-\frac{m}{4\hbar}\left((\omega_+ + \omega_-)(x_1^2+x_2^2)+2(\omega_+-\omega_-)x_1x_2\right)\right].
$$

**Analysis:**
After diagonalization, the Hamiltonian is a sum of two independent harmonic oscillator Hamiltonians, one in $x_+$ and one in $x_-$. Therefore its ground state is the tensor product of the individual oscillator ground states. Each oscillator ground state is a normalized Gaussian with width set by $m\omega_\pm/\hbar$. Since the transformation from $(x_1,x_2)$ to $(x_+,x_-)$ is orthogonal with unit Jacobian, no additional Jacobian factor is introduced in the normalized wavefunction. Substituting $x_+=(x_1+x_2)/\sqrt{2}$ and $x_-=(x_1-x_2)/\sqrt{2}$ gives the original-coordinate form.

### Step 3: Use the definition of $\hat{\rho}$ to form the reduced density-matrix kernel $\rho(x_{1}'',x_{1}')=\int dw\,\Omega(x_{1}'',w)\Omega^{*}(x_{1}',w)$ after tracing over the $|w\rangle_{x_{2}}$ components satisfying $\hat{x}_{2}|w\rangle_{x_{2}}=w|w\rangle_{x_{2}}$.

**Reasoning:**
Insert coordinate-basis resolutions into \(|\Omega\rangle\langle\Omega|\). The matrix element over the traced oscillator is \(\langle x_1'',w|\Omega\rangle\langle\Omega|x_1',w\rangle=\Omega(x_1'',w)\Omega^*(x_1',w)\). The partial trace therefore integrates only over \(w=x_2\). Using the real Gaussian ground state from Step 2 reduces the trace to a one-dimensional Gaussian integral. Completing the square gives the exponential term proportional to \((x_1''+x_1')^2\), and the normalization follows from \(N^2\sqrt{2\pi\hbar/(mA)}=(2m\omega_+\omega_-/[\pi\hbar A])^{1/2}\).

**Result:**
Let \(A\equiv \omega_++\omega_-\), \(B\equiv \omega_+-\omega_-\), and \(N=(m^2\omega_+\omega_-/\pi^2\hbar^2)^{1/4}\). From Step 2,

$$
\Omega(x_1,x_2)=N\exp\left[-\frac{m}{4\hbar}\left(A(x_1^2+x_2^2)+2Bx_1x_2\right)\right].
$$

The wavefunction is real, so \(\Omega^*=\Omega\). Tracing over the coordinate eigenstates \(|w\rangle_{x_2}\) gives

$$
\rho(x_1'',x_1')=\int_{-\infty}^{\infty}dw\,\Omega(x_1'',w)\Omega^*(x_1',w).
$$

Substitution gives

$$
\rho(x_1'',x_1')=N^2\exp\left[-\frac{mA}{4\hbar}\left((x_1'')^2+(x_1')^2\right)\right]\int_{-\infty}^{\infty}dw\,\exp\left[-\frac{mA}{2\hbar}w^2-\frac{mB}{2\hbar}(x_1''+x_1')w\right].
$$

Evaluating the Gaussian integral,

$$
\boxed{\rho(x_1'',x_1')=\left(\frac{2m\omega_+\omega_-}{\pi\hbar(\omega_++\omega_-)}\right)^{1/2}\exp\left[-\frac{m(\omega_++\omega_-)}{4\hbar}\left((x_1'')^2+(x_1')^2\right)+\frac{m(\omega_+-\omega_-)^2}{8\hbar(\omega_++\omega_-)}(x_1''+x_1')^2\right]}.
$$

Equivalently,

$$
\rho(x_1'',x_1')=\left(\frac{2m\omega_+\omega_-}{\pi\hbar A}\right)^{1/2}\exp\left[-\frac{mA}{4\hbar}\left((x_1'')^2+(x_1')^2\right)+\frac{mB^2}{8\hbar A}(x_1''+x_1')^2\right].
$$

**Analysis:**
Insert coordinate-basis resolutions into \(|\Omega\rangle\langle\Omega|\). The matrix element over the traced oscillator is \(\langle x_1'',w|\Omega\rangle\langle\Omega|x_1',w\rangle=\Omega(x_1'',w)\Omega^*(x_1',w)\). The partial trace therefore integrates only over \(w=x_2\). Using the real Gaussian ground state from Step 2 reduces the trace to a one-dimensional Gaussian integral. Completing the square gives the exponential term proportional to \((x_1''+x_1')^2\), and the normalization follows from \(N^2\sqrt{2\pi\hbar/(mA)}=(2m\omega_+\omega_-/[\pi\hbar A])^{1/2}\).

### Step 4: Identify $\rho(x_{1}'',x_{1}')$ with the thermal density matrix of an effective single oscillator, or equivalently compute the symplectic eigenvalue $\nu=\sqrt{\langle x_{1}^{2}\rangle\langle p_{1}^{2}\rangle}/\hbar$ of the reduced Gaussian state.

**Reasoning:**
Because the total ground state factorizes in normal-mode coordinates, all covariances in the original oscillator variables can be computed by the linear canonical transformation. The reduced state of oscillator 1 is Gaussian since tracing out one oscillator from a pure Gaussian state leaves a Gaussian state. For a one-mode Gaussian state with zero first moments and no $xp$ covariance, the only invariant needed for the entropy is the symplectic eigenvalue $\nu=\sqrt{\langle x_1^2\rangle\langle p_1^2\rangle}/\hbar$. The variances of each independent normal-mode ground state are those of an ordinary harmonic oscillator. Substituting $x_1=(x_++x_-)/\sqrt{2}$ and $p_1=(p_++p_-)/\sqrt{2}$ gives the stated $\langle x_1^2\rangle$ and $\langle p_1^2\rangle$. Their product gives $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Since any one-mode Gaussian state with covariance proportional to a thermal oscillator covariance is unitarily equivalent to a thermal state, this also identifies the reduced density matrix with a thermal density matrix with occupation number $\bar n=\nu-1/2$ and Boltzmann ratio $q=(\nu-1/2)/(\nu+1/2)$.

**Result:**
The reduced density matrix $\rho(x_1'',x_1')$ is a one-mode Gaussian density matrix. It can therefore be identified with the thermal density matrix of an effective oscillator. The simplest way to extract the relevant thermal parameter is through the symplectic eigenvalue
$$
\nu=\frac{1}{\hbar}\sqrt{\langle x_1^2\rangle\langle p_1^2\rangle},
$$
where the mixed covariance vanishes, $\langle \{x_1,p_1\}\rangle/2=0$.

Using
$$
x_1=\frac{x_++x_-}{\sqrt{2}},\qquad p_1=\frac{p_++p_-}{\sqrt{2}},
$$
and the ground-state variances
$$
\langle x_\pm^2\rangle=\frac{\hbar}{2m\omega_\pm},\qquad \langle p_\pm^2\rangle=\frac{\hbar m\omega_\pm}{2},
$$
with no cross-correlations between the $+$ and $-$ modes, one obtains
$$
\langle x_1^2\rangle=\frac{1}{2}\left(\langle x_+^2\rangle+\langle x_-^2\rangle\right)
=\frac{\hbar}{4m}\left(\frac{1}{\omega_+}+\frac{1}{\omega_-}\right),
$$
and
$$
\langle p_1^2\rangle=\frac{1}{2}\left(\langle p_+^2\rangle+\langle p_-^2\rangle\right)
=\frac{\hbar m}{4}\left(\omega_++\omega_-\right).
$$
Therefore
$$
\boxed{\nu=\frac{\omega_++\omega_-}{4\sqrt{\omega_+\omega_-}}.}
$$
This satisfies $\nu\geq 1/2$, with equality only when $\omega_+=\omega_-$, i.e. when $g=0$ and the reduced state is pure.

Equivalently, the reduced state is thermal with mean occupation number
$$
\bar n=\nu-\frac{1}{2}
=\frac{\omega_++\omega_- -2\sqrt{\omega_+\omega_-}}{4\sqrt{\omega_+\omega_-}}
=\frac{\left(\sqrt{\omega_-}-\sqrt{\omega_+}\right)^2}{4\sqrt{\omega_+\omega_-}}.
$$
If one writes the thermal eigenvalues as
$$
p_n=(1-q)q^n,
$$
then
$$
q=\frac{\bar n}{\bar n+1}=\frac{\nu-1/2}{\nu+1/2}
=\left(\frac{\sqrt{\omega_-}-\sqrt{\omega_+}}{\sqrt{\omega_-}+\sqrt{\omega_+}}\right)^2.
$$
The effective oscillator frequency may be chosen, for mass $m$, as
$$
\omega_{\mathrm{eff}}=\sqrt{\frac{\langle p_1^2\rangle}{m^2\langle x_1^2\rangle}}=\sqrt{\omega_+\omega_-},
$$
with an effective inverse temperature determined by
$$
e^{-\beta\hbar\omega_{\mathrm{eff}}}=q
=\left(\frac{\sqrt{\omega_-}-\sqrt{\omega_+}}{\sqrt{\omega_-}+\sqrt{\omega_+}}\right)^2.
$$

**Analysis:**
Because the total ground state factorizes in normal-mode coordinates, all covariances in the original oscillator variables can be computed by the linear canonical transformation. The reduced state of oscillator 1 is Gaussian since tracing out one oscillator from a pure Gaussian state leaves a Gaussian state. For a one-mode Gaussian state with zero first moments and no $xp$ covariance, the only invariant needed for the entropy is the symplectic eigenvalue $\nu=\sqrt{\langle x_1^2\rangle\langle p_1^2\rangle}/\hbar$. The variances of each independent normal-mode ground state are those of an ordinary harmonic oscillator. Substituting $x_1=(x_++x_-)/\sqrt{2}$ and $p_1=(p_++p_-)/\sqrt{2}$ gives the stated $\langle x_1^2\rangle$ and $\langle p_1^2\rangle$. Their product gives $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Since any one-mode Gaussian state with covariance proportional to a thermal oscillator covariance is unitarily equivalent to a thermal state, this also identifies the reduced density matrix with a thermal density matrix with occupation number $\bar n=\nu-1/2$ and Boltzmann ratio $q=(\nu-1/2)/(\nu+1/2)$.

### Step 5: Evaluate $\nu$ explicitly using $\langle x_{1}^{2}\rangle=\frac{\hbar}{4m}\left(\frac{1}{\omega_{+}}+\frac{1}{\omega_{-}}\right)$ and $\langle p_{1}^{2}\rangle=\frac{\hbar m}{4}\left(\omega_{+}+\omega_{-}\right)$, giving $\nu=\frac{1}{4}\frac{\omega_{+}+\omega_{-}}{\sqrt{\omega_{+}\omega_{-}}}$.

**Reasoning:**
The symplectic eigenvalue for a single Gaussian mode with vanishing mixed covariance is determined by the dimensionless uncertainty product. Multiplying the supplied variances cancels the mass $m$ and produces a factor $\hbar^2/16$. The remaining frequency factor simplifies as $(1/\omega_+ + 1/\omega_-)(\omega_+ + \omega_-)= (\omega_+ + \omega_-)^2/(\omega_+\omega_-)$. Taking the square root and dividing by $\hbar$ gives $\nu=(\omega_+ + \omega_-)/(4\sqrt{\omega_+\omega_-})$. Positivity of the frequencies ensures the square root is unambiguous. By AM-GM, $(\omega_+ + \omega_-)/\sqrt{\omega_+\omega_-}\geq 2$, so $\nu\geq 1/2$, consistent with the uncertainty principle.

**Result:**
Starting from
$$
\nu=\frac{1}{\hbar}\sqrt{\langle x_1^2\rangle\langle p_1^2\rangle},
$$
insert
$$
\langle x_1^2\rangle=\frac{\hbar}{4m}\left(\frac{1}{\omega_+}+\frac{1}{\omega_-}\right),\qquad
\langle p_1^2\rangle=\frac{\hbar m}{4}(\omega_++\omega_-).
$$
Then
$$
\langle x_1^2\rangle\langle p_1^2\rangle
=\frac{\hbar^2}{16}\left(\frac{1}{\omega_+}+\frac{1}{\omega_-}\right)(\omega_++\omega_-).
$$
Since
$$
\frac{1}{\omega_+}+\frac{1}{\omega_-}=\frac{\omega_++\omega_-}{\omega_+\omega_-},
$$
one obtains
$$
\langle x_1^2\rangle\langle p_1^2\rangle
=\frac{\hbar^2}{16}\frac{(\omega_++\omega_-)^2}{\omega_+\omega_-}.
$$
Therefore
$$
\boxed{\nu=\frac{1}{4}\frac{\omega_++\omega_-}{\sqrt{\omega_+\omega_-}}.}
$$
Equivalently, using $\omega_+=\sqrt{k/m}$ and $\omega_-=\sqrt{(k+2g)/m}$,
$$
\nu=\frac{1}{4}\frac{\sqrt{k/m}+\sqrt{(k+2g)/m}}{\left[(k/m)((k+2g)/m)\right]^{1/4}}.
$$
This satisfies $\nu\geq 1/2$, with equality when $\omega_+=\omega_-$, i.e. for $g=0$.

**Analysis:**
The symplectic eigenvalue for a single Gaussian mode with vanishing mixed covariance is determined by the dimensionless uncertainty product. Multiplying the supplied variances cancels the mass $m$ and produces a factor $\hbar^2/16$. The remaining frequency factor simplifies as $(1/\omega_+ + 1/\omega_-)(\omega_+ + \omega_-)= (\omega_+ + \omega_-)^2/(\omega_+\omega_-)$. Taking the square root and dividing by $\hbar$ gives $\nu=(\omega_+ + \omega_-)/(4\sqrt{\omega_+\omega_-})$. Positivity of the frequencies ensures the square root is unambiguous. By AM-GM, $(\omega_+ + \omega_-)/\sqrt{\omega_+\omega_-}\geq 2$, so $\nu\geq 1/2$, consistent with the uncertainty principle.

### Step 6: Insert $\nu$ into the one-mode Gaussian entropy formula $S=\left(\nu+\frac{1}{2}\right)\ln\left(\nu+\frac{1}{2}\right)-\left(\nu-\frac{1}{2}\right)\ln\left(\nu-\frac{1}{2}\right)$ and express the result in terms of $k$, $g$, and $m$, noting that $m$ cancels through the ratio $\omega_{-}/\omega_{+}=\sqrt{1+2g/k}$.

**Reasoning:**
The entropy of a single-mode Gaussian state depends only on the symplectic eigenvalue $\nu$. From the covariance calculation, $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Dividing numerator and denominator by $\omega_+$ shows that only the ratio $r=\omega_-/\omega_+$ enters: $\nu=(1+r)/(4\sqrt r)$. Since $\omega_+=\sqrt{k/m}$ and $\omega_- = \sqrt{(k+2g)/m}$, their ratio is $r=\sqrt{(k+2g)/k}=\sqrt{1+2g/k}$, so $m$ cancels. Then $\nu\pm 1/2$ simplify to $((\sqrt r\pm 1)^2)/(4\sqrt r)$, and substitution into $S=(\nu+1/2)\ln(\nu+1/2)-(\nu-1/2)\ln(\nu-1/2)$ yields the final expression.

**Result:**
Let
$$r\equiv \frac{\omega_-}{\omega_+}=\sqrt{1+\frac{2g}{k}}.$$
Then
$$\nu=\frac{1}{4}\frac{\omega_++\omega_-}{\sqrt{\omega_+\omega_-}}=\frac{1}{4}\frac{1+r}{\sqrt r}=\frac{1}{4}\left(\sqrt r+\frac{1}{\sqrt r}\right).$$
Therefore
$$\nu+\frac{1}{2}=\frac{(\sqrt r+1)^2}{4\sqrt r},\qquad \nu-\frac{1}{2}=\frac{(\sqrt r-1)^2}{4\sqrt r}.$$
Inserting into the one-mode Gaussian entropy formula gives
$$\boxed{S=\frac{(\sqrt r+1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r+1)^2}{4\sqrt r}\right]-\frac{(\sqrt r-1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r-1)^2}{4\sqrt r}\right]}$$
with
$$r=\sqrt{1+\frac{2g}{k}}.$$
Equivalently, defining
$$a\equiv \sqrt r=\left(1+\frac{2g}{k}\right)^{1/4},$$
one may write
$$\boxed{S=\frac{(a+1)^2}{4a}\ln\left[\frac{(a+1)^2}{4a}\right]-\frac{(a-1)^2}{4a}\ln\left[\frac{(a-1)^2}{4a}\right],\qquad a=\left(1+\frac{2g}{k}\right)^{1/4}.}$$
The mass $m$ has cancelled, as expected. For $g=0$, $a=1$, so $\nu=1/2$ and $S=0$, corresponding to an unentangled product vacuum.

**Analysis:**
The entropy of a single-mode Gaussian state depends only on the symplectic eigenvalue $\nu$. From the covariance calculation, $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Dividing numerator and denominator by $\omega_+$ shows that only the ratio $r=\omega_-/\omega_+$ enters: $\nu=(1+r)/(4\sqrt r)$. Since $\omega_+=\sqrt{k/m}$ and $\omega_- = \sqrt{(k+2g)/m}$, their ratio is $r=\sqrt{(k+2g)/k}=\sqrt{1+2g/k}$, so $m$ cancels. Then $\nu\pm 1/2$ simplify to $((\sqrt r\pm 1)^2)/(4\sqrt r)$, and substitution into $S=(\nu+1/2)\ln(\nu+1/2)-(\nu-1/2)\ln(\nu-1/2)$ yields the final expression.

---

## Final Result
(no final result)