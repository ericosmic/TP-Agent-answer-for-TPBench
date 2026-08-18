# Step 4 — Identify $\rho(x_{1}'',x_{1}')$ with the thermal density matrix of an effective single oscillator, or equivalently compute the symplectic eigenvalue $\nu=\sqrt{\langle x_{1}^{2}\rangle\langle p_{1}^{2}\rangle}/\hbar$ of the reduced Gaussian state.

## Solution Reasoning

Because the total ground state factorizes in normal-mode coordinates, all covariances in the original oscillator variables can be computed by the linear canonical transformation. The reduced state of oscillator 1 is Gaussian since tracing out one oscillator from a pure Gaussian state leaves a Gaussian state. For a one-mode Gaussian state with zero first moments and no $xp$ covariance, the only invariant needed for the entropy is the symplectic eigenvalue $\nu=\sqrt{\langle x_1^2\rangle\langle p_1^2\rangle}/\hbar$. The variances of each independent normal-mode ground state are those of an ordinary harmonic oscillator. Substituting $x_1=(x_++x_-)/\sqrt{2}$ and $p_1=(p_++p_-)/\sqrt{2}$ gives the stated $\langle x_1^2\rangle$ and $\langle p_1^2\rangle$. Their product gives $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Since any one-mode Gaussian state with covariance proportional to a thermal oscillator covariance is unitarily equivalent to a thermal state, this also identifies the reduced density matrix with a thermal density matrix with occupation number $\bar n=\nu-1/2$ and Boltzmann ratio $q=(\nu-1/2)/(\nu+1/2)$.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
