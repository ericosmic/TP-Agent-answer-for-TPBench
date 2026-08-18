# Step 3 — Evaluate the mean sampled density on the retained domain using standard Gaussian moments: $\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]$ for $b\neq0$, where $\phi$ and $\Phi$ are the standard normal PDF and CDF.

## Solution Reasoning

The clipped density contributes only on the positivity domain $1+b\delta>0$. The sign-dependent retained region can be made uniform by changing variables to $z=\operatorname{sgn}(b)\delta/\sigma$, giving $z>-\alpha$ with $\alpha=1/(|b|\sigma)$. Since the Gaussian distribution is symmetric, $z$ is again a standard normal variate. In this variable the factor $b\delta$ becomes $|b|\sigma z$, so the mean is a retained-domain integral of $1+|b|\sigma z$ against the standard normal PDF. The zeroth truncated moment gives $\Phi(\alpha)$, and the first truncated moment gives $\phi(\alpha)$, yielding the stated expression.

## Result

For $b
eq0$, write the mean density as
$$
\langle n\rangle=\bar n\left\langle (1+b\delta)\Theta(1+b\delta)\right\rangle .
$$
Introduce
$$
\alpha\equiv \frac{1}{|b|\sigma}>0,\qquad z\equiv \operatorname{sgn}(b)\frac{\delta}{\sigma},
$$
so that $z\sim\mathcal{N}(0,1)$ and the retained domain is $z>-\alpha$. Also,
$$
b\delta=|b|\sigma z.
$$
Therefore
$$
\langle n\rangle
=\bar n\int_{-\alpha}^{\infty}\left(1+|b|\sigma z\right)\phi(z)\,dz .
$$
Using the standard Gaussian moments
$$
\int_{-\alpha}^{\infty}\phi(z)\,dz=\Phi(\alpha),
\qquad
\int_{-\alpha}^{\infty}z\phi(z)\,dz=\phi(\alpha),
$$
where $\phi(-\alpha)=\phi(\alpha)$, we obtain
$$
\boxed{\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]},
\qquad
\alpha=\frac{1}{|b|\sigma},\quad b
eq0.
$$
For completeness, when $b=0$, no clipping occurs and $n=\bar n$, so
$$
\langle n\rangle=\bar n.
$$

## Physical Interpretation

For $b
eq0$, write the mean density as
$$
\langle n\rangle=\bar n\left\langle (1+b\delta)\Theta(1+b\delta)\right\rangle .
$$
Introduce
$$
\alpha\equiv \frac{1}{|b|\sigma}>0,\qquad z\equiv \operatorname{sgn}(b)\frac{\delta}{\sigma},
$$
so that $z\sim\mathcal{N}(0,1)$ and the retained domain is $z>-\alpha$. Also,
$$
b\delta=|b|\sigma z.
$$
Therefore
$$
\langle n\rangle
=\bar n\int_{-\alpha}^{\infty}\left(1+|b|\sigma z\right)\phi(z)\,dz .
$$
Using the standard Gaussian moments
$$
\int_{-\alpha}^{\infty}\phi(z)\,dz=\Phi(\alpha),
\qquad
\int_{-\alpha}^{\infty}z\phi(z)\,dz=\phi(\alpha),
$$
where $\phi(-\alpha)=\phi(\alpha)$, we obtain
$$
\boxed{\langle n\rangle=\bar n\left[\Phi(\alpha)+|b|\sigma\phi(\alpha)\right]},
\qquad
\alpha=\frac{1}{|b|\sigma},\quad b
eq0.
$$
For completeness, when $b=0$, no clipping occurs and $n=\bar n$, so
$$
\langle n\rangle=\bar n.
$$

**Consistency check:** passed
