# Step 2 — Write the ground-state wavefunction $\Omega(x_{1},x_{2})=\langle x_{1},x_{2}|\Omega\rangle$ as a product of Gaussian normal-mode vacua, then express it in the original coordinates $x_{1},x_{2}$.

## Solution Reasoning

After diagonalization, the Hamiltonian is a sum of two independent harmonic oscillator Hamiltonians, one in $x_+$ and one in $x_-$. Therefore its ground state is the tensor product of the individual oscillator ground states. Each oscillator ground state is a normalized Gaussian with width set by $m\omega_\pm/\hbar$. Since the transformation from $(x_1,x_2)$ to $(x_+,x_-)$ is orthogonal with unit Jacobian, no additional Jacobian factor is introduced in the normalized wavefunction. Substituting $x_+=(x_1+x_2)/\sqrt{2}$ and $x_-=(x_1-x_2)/\sqrt{2}$ gives the original-coordinate form.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
