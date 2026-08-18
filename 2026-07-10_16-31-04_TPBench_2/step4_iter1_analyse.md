# Analyse Step 4 Iteration 1

**Description:** Define the effective large-scale bias of the normalized sampled field by the cross-correlation response $b_{\rm eff}=\langle\delta_h\delta_m\rangle/\langle\delta_m^2\rangle=\langle n\delta_m\rangle/(\sigma^2\langle n\rangle)$, using the result of the previous step for the normalization.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The needed prior results are: the normalized halo overdensity $\delta_h=n/\langle n\rangle-1$, the Gaussian one-pixel model $\delta\sim\mathcal{N}(0,\sigma^2)$, the clipped density $n=\bar n(1+b\delta)\Theta(1+b\delta)$, and the previous-step normalization $\langle n\rangle=\bar n[\Phi(\alpha)+|b|\sigma\phi(\alpha)]$ with $\alpha=1/(|b|\sigma)$ for $b\ne0$.

## Critical Rubrics

A correct result must: (i) define $b_{\rm eff}$ through $\langle\delta_h\delta_m\rangle/\sigma^2$; (ii) use $\delta_h=n/\langle n\rangle-1$ and the Gaussian condition $\langle\delta_m\rangle=0$ to obtain $b_{\rm eff}=\langle n\delta_m\rangle/(\sigma^2\langle n\rangle)$; (iii) insert the previous normalization $\langle n\rangle=\bar n[\Phi(\alpha)+|b|\sigma\phi(\alpha)]$ with $\alpha=1/(|b|\sigma)$; (iv) handle both signs of $b$ consistently through $|b|$ or $\operatorname{sgn}(b)$; (v) note the special case $b=0$ gives zero sampled bias; and (vi) cancel the unphysical dependence on $\bar n$.

## Candidate Result

The effective large-scale bias is defined by the cross-correlation response
$$
b_{\rm eff}\equiv \frac{\langle \delta_h\delta_m\rangle}{\langle \delta_m^2\rangle}.
$$
Writing $\delta_m\equiv\delta$ and using $\delta_h=n/\langle n\rangle-1$, we have
$$
\langle\delta_h\delta\rangle
=\left\langle \left(\frac{n}{\langle n\rangle}-1\right)\delta\right\rangle
=\frac{\langle n\delta\rangle}{\langle n\rangle}-\langle\delta\rangle.
$$
Since $\langle\delta\rangle=0$ and $\langle\delta^2\rangle=\sigma^2$,
$$
\boxed{b_{\rm eff}=\frac{\langle n\delta\rangle}{\sigma^2\langle n\rangle}}.
$$
Using the previous normalization, for $b\ne0$,
$$
\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right],
\qquad \alpha=\frac{1}{|b|\sigma}.
$$
Therefore
$$
\boxed{
b_{\rm eff}
=\frac{\left\langle \bar n(1+b\delta)\Theta(1+b\delta)\,\delta\right\rangle}{\sigma^2\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]}
=\frac{\left\langle (1+b\delta)\Theta(1+b\delta)\,\delta\right\rangle}{\sigma^2\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]}
}.
$$
Equivalently, after the change of variables $z=\operatorname{sgn}(b)\delta/\sigma$, so that the retained domain is $z>-\alpha$,
$$
\boxed{
b_{\rm eff}
=\frac{\operatorname{sgn}(b)}{\sigma\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]}
\int_{-\alpha}^{\infty} z\left(1+|b|\sigma z\right)\phi(z)\,dz
}.
$$
Evaluating the remaining Gaussian moment gives
$$
\int_{-\alpha}^{\infty} z(1+|b|\sigma z)\phi(z)\,dz
=|b|\sigma\Phi(\alpha),
$$
so one may also write the closed form
$$
\boxed{
b_{\rm eff}(b,\sigma)
=\frac{b\,\Phi(\alpha)}{\Phi(\alpha)+|b|\sigma\phi(\alpha)},
\qquad \alpha=\frac{1}{|b|\sigma},\quad b\ne0.
}
$$
For $b=0$, $n=\bar n$ is spatially constant, so $\delta_h=0$ and
$$
\boxed{b_{\rm eff}=0.}
$$

## Reasoning

The normalized overdensity is $\delta_h=n/\langle n\rangle-1$. Its cross-correlation with the Gaussian matter fluctuation is $\langle\delta_h\delta\rangle=\langle n\delta\rangle/\langle n\rangle-\langle\delta\rangle$. The Gaussian has zero mean, so the second term vanishes. Dividing by $\sigma^2=\langle\delta^2\rangle$ gives $b_{\rm eff}=\langle n\delta\rangle/(\sigma^2\langle n\rangle)$. Substituting the previous-step result for $\langle n\rangle$ yields the desired expression depending only on $b$ and the pixel variance $\sigma^2$. If desired, the numerator is evaluated by using $z=\operatorname{sgn}(b)\delta/\sigma$, under which $b\delta=|b|\sigma z$ and the clipping condition is $z>-\alpha$. The standard moments $\int_{-\alpha}^{\infty}z\phi(z)dz=\phi(\alpha)$ and $\int_{-\alpha}^{\infty}z^2\phi(z)dz=\Phi(\alpha)-\alpha\phi(\alpha)$ imply cancellation of the boundary terms because $|b|\sigma\alpha=1$, leaving $\langle n\delta\rangle=\bar n b\sigma^2\Phi(\alpha)$.
