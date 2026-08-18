# Step 5 — Evaluate the retained-domain moment $\langle n\delta_m\rangle$ with the same sign-aware variable choice, obtaining $\langle n\delta_m\rangle=\bar n\,b\sigma^2\Phi(\alpha)$, and combine it with the preceding expression for $\langle n\rangle$ to give the final equation $$b_{\rm eff}(b,\sigma)=\frac{b\Phi\!\left(\frac{1}{|b|\sigma}\right)}{\Phi\!\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi\!\left(\frac{1}{|b|\sigma}\right)}$$ for $b\neq0$, with $b_{\rm eff}=0$ for $b=0$.

## Solution Reasoning

The sign-aware substitution $z=\operatorname{sgn}(b)\delta/\sigma$ makes the positivity condition $1+b\delta>0$ identical for positive and negative bare bias: $z>-\alpha$. In this variable, $b\delta=|b|\sigma z$ while the extra factor of $\delta$ in $\langle n\delta\rangle$ contributes $\operatorname{sgn}(b)\sigma z$. The retained-domain integral is therefore reduced to standard truncated-normal moments. The $z\phi(z)$ term produces $\phi(\alpha)$ and the $z^2\phi(z)$ term produces $\Phi(\alpha)-\alpha\phi(\alpha)$. Because $\alpha=1/(|b|\sigma)$, the boundary contributions cancel exactly, leaving only $|b|\sigma\Phi(\alpha)$. Multiplying by $\operatorname{sgn}(b)\sigma$ gives $b\sigma^2\Phi(\alpha)$, and the factor $\bar n$ is restored. The effective bias follows by dividing $\langle n\delta_m\rangle$ by $\sigma^2\langle n\rangle$, using the previously obtained normalization. The $b=0$ case must be handled separately because $\alpha$ is undefined and the field is constant.

## Result

For $b
eq0$, define $\alpha=1/(|b|\sigma)$ and $z=\operatorname{sgn}(b)\delta/\sigma$, so that $z\sim\mathcal{N}(0,1)$, the retained domain is $z>-\alpha$, and $b\delta=|b|\sigma z$. Also $\delta=\operatorname{sgn}(b)\sigma z$. Then
$$
\langle n\delta\rangle
=\bar n\int_{1+b\delta>0}(1+b\delta)\delta\,p(\delta)\,d\delta
=\bar n\,\operatorname{sgn}(b)\sigma\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz.
$$
Using
$$
\int_{-\alpha}^{\infty}z\phi(z)\,dz=\phi(\alpha),
\qquad
\int_{-\alpha}^{\infty}z^2\phi(z)\,dz=\Phi(\alpha)-\alpha\phi(\alpha),
$$
we find
$$
\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz
=\phi(\alpha)+|b|\sigma[\Phi(\alpha)-\alpha\phi(\alpha)].
$$
Since $|b|\sigma\alpha=1$, the two boundary terms cancel:
$$
\phi(\alpha)-|b|\sigma\alpha\phi(\alpha)=0,
$$
leaving
$$
\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz=|b|\sigma\Phi(\alpha).
$$
Therefore
$$
\boxed{\langle n\delta_m\rangle=\bar n\,\operatorname{sgn}(b)\sigma\,|b|\sigma\Phi(\alpha)=\bar n\,b\sigma^2\Phi(\alpha)}.
$$
Combining with
$$
\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]
$$
and
$$
b_{\rm eff}=\frac{\langle n\delta_m\rangle}{\sigma^2\langle n\rangle},
$$
gives
$$
\boxed{
b_{\rm eff}(b,\sigma)=\frac{b\Phi(\alpha)}{\Phi(\alpha)+|b|\sigma\phi(\alpha)},
\qquad \alpha=\frac{1}{|b|\sigma},\quad b
eq0.
}
$$
Equivalently,
$$
\boxed{
b_{\rm eff}(b,\sigma)=\frac{b\Phi\!\left(\frac{1}{|b|\sigma}\right)}{\Phi\!\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi\!\left(\frac{1}{|b|\sigma}\right)},\quad b
eq0.
}
$$
For $b=0$, $n=\bar n$ is spatially constant, so $\delta_h=0$ and
$$
\boxed{b_{\rm eff}=0.}
$$

## Physical Interpretation

For $b
eq0$, define $\alpha=1/(|b|\sigma)$ and $z=\operatorname{sgn}(b)\delta/\sigma$, so that $z\sim\mathcal{N}(0,1)$, the retained domain is $z>-\alpha$, and $b\delta=|b|\sigma z$. Also $\delta=\operatorname{sgn}(b)\sigma z$. Then
$$
\langle n\delta\rangle
=\bar n\int_{1+b\delta>0}(1+b\delta)\delta\,p(\delta)\,d\delta
=\bar n\,\operatorname{sgn}(b)\sigma\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz.
$$
Using
$$
\int_{-\alpha}^{\infty}z\phi(z)\,dz=\phi(\alpha),
\qquad
\int_{-\alpha}^{\infty}z^2\phi(z)\,dz=\Phi(\alpha)-\alpha\phi(\alpha),
$$
we find
$$
\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz
=\phi(\alpha)+|b|\sigma[\Phi(\alpha)-\alpha\phi(\alpha)].
$$
Since $|b|\sigma\alpha=1$, the two boundary terms cancel:
$$
\phi(\alpha)-|b|\sigma\alpha\phi(\alpha)=0,
$$
leaving
$$
\int_{-\alpha}^{\infty}z(1+|b|\sigma z)\phi(z)\,dz=|b|\sigma\Phi(\alpha).
$$
Therefore
$$
\boxed{\langle n\delta_m\rangle=\bar n\,\operatorname{sgn}(b)\sigma\,|b|\sigma\Phi(\alpha)=\bar n\,b\sigma^2\Phi(\alpha)}.
$$
Combining with
$$
\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]
$$
and
$$
b_{\rm eff}=\frac{\langle n\delta_m\rangle}{\sigma^2\langle n\rangle},
$$
gives
$$
\boxed{
b_{\rm eff}(b,\sigma)=\frac{b\Phi(\alpha)}{\Phi(\alpha)+|b|\sigma\phi(\alpha)},
\qquad \alpha=\frac{1}{|b|\sigma},\quad b
eq0.
}
$$
Equivalently,
$$
\boxed{
b_{\rm eff}(b,\sigma)=\frac{b\Phi\!\left(\frac{1}{|b|\sigma}\right)}{\Phi\!\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi\!\left(\frac{1}{|b|\sigma}\right)},\quad b
eq0.
}
$$
For $b=0$, $n=\bar n$ is spatially constant, so $\delta_h=0$ and
$$
\boxed{b_{\rm eff}=0.}
$$

**Consistency check:** passed
