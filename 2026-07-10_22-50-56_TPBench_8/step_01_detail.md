# Step 1 — Diagonalize the Hamiltonian $H=\sum_{i=1}^{2}\frac{1}{2}\left(\frac{p_{i}^{2}}{m}+kx_{i}^{2}\right)+g\frac{(x_{1}-x_{2})^{2}}{2}$ by introducing normal coordinates $x_{+}=\frac{x_{1}+x_{2}}{\sqrt{2}}$, $x_{-}=\frac{x_{1}-x_{2}}{\sqrt{2}}$ and their conjugate momenta, giving frequencies $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

## Solution Reasoning

The transformation to $x_{+}$ and $x_{-}$ is an orthogonal rotation in the two-dimensional coordinate space, so it preserves quadratic sums such as $x_1^2+x_2^2$ and, with the same transformation applied to the momenta, preserves $p_1^2+p_2^2$ and the canonical commutation relations. The coupling depends only on the relative displacement $x_1-x_2$, which becomes $\sqrt{2}x_{-}$. Hence the coupling contributes $g(x_1-x_2)^2/2=g x_{-}^2$, modifying only the spring constant of the antisymmetric mode. The symmetric mode retains spring constant $k$, while the antisymmetric mode has effective spring constant $k+2g$. Comparing each quadratic potential term to $m\omega^2x^2/2$ gives $\omega_{+}=\sqrt{k/m}$ and $\omega_{-}=\sqrt{(k+2g)/m}$.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
