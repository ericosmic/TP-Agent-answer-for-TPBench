# Step 5 — Present the final integrated slow-roll solution $\phi(t)$, check that it satisfies $\phi(0)=\phi_0$, and optionally express the validity condition through the slow-roll parameter $\epsilon_V=\frac{M_P^2}{2}\left(V'/V\right)^2=1/q$, requiring $q\gg 1$ for slow roll.

## Solution Reasoning

Starting from the previously integrated relation, one simply solves for $\phi(t)$ by taking the logarithm. The equivalent shifted form is obtained by factoring $e^{\phi_0/(\sqrt{2q}M_P)}$ inside the logarithm, which makes the initial condition explicit. Substitution of $t=0$ gives the logarithm of unity in the shifted form, hence $\phi(0)=\phi_0$. The slow-roll validity condition follows from differentiating the exponential potential: $V'/V=-\sqrt{2/q}/M_P$, giving $\epsilon_V=1/q$, so slow roll requires $q\gg 1$.

## Result

The integrated slow-roll solution is
$$
e^{\phi(t)/(\sqrt{2q}\,M_P)}=e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t.
$$
Equivalently,
$$
\boxed{\phi(t)\simeq \sqrt{2q}\,M_P\ln\left[e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t\right]}.
$$
A form in which the initial condition is manifest is
$$
\boxed{\phi(t)\simeq \phi_0+\sqrt{2q}\,M_P\ln\left[1+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,e^{-\phi_0/(\sqrt{2q}\,M_P)}t\right]}.
$$
Checking the initial condition, at $t=0$,
$$
\phi(0)=\phi_0+\sqrt{2q}\,M_P\ln(1)=\phi_0,
$$
so the solution satisfies $\phi(0)=\phi_0$.

For the exponential potential,
$$
\frac{V'}{V}=-\frac{1}{M_P}\sqrt{\frac{2}{q}},
$$
so
$$
\epsilon_V=\frac{M_P^2}{2}\left(\frac{V'}{V}\right)^2=\frac{M_P^2}{2}\frac{2}{qM_P^2}=\frac{1}{q}.
$$
Thus the slow-roll regime requires
$$
\boxed{\epsilon_V\ll 1 \quad \Longleftrightarrow \quad q\gg 1.}
$$

## Physical Interpretation

The integrated slow-roll solution is
$$
e^{\phi(t)/(\sqrt{2q}\,M_P)}=e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t.
$$
Equivalently,
$$
\boxed{\phi(t)\simeq \sqrt{2q}\,M_P\ln\left[e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t\right]}.
$$
A form in which the initial condition is manifest is
$$
\boxed{\phi(t)\simeq \phi_0+\sqrt{2q}\,M_P\ln\left[1+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,e^{-\phi_0/(\sqrt{2q}\,M_P)}t\right]}.
$$
Checking the initial condition, at $t=0$,
$$
\phi(0)=\phi_0+\sqrt{2q}\,M_P\ln(1)=\phi_0,
$$
so the solution satisfies $\phi(0)=\phi_0$.

For the exponential potential,
$$
\frac{V'}{V}=-\frac{1}{M_P}\sqrt{\frac{2}{q}},
$$
so
$$
\epsilon_V=\frac{M_P^2}{2}\left(\frac{V'}{V}\right)^2=\frac{M_P^2}{2}\frac{2}{qM_P^2}=\frac{1}{q}.
$$
Thus the slow-roll regime requires
$$
\boxed{\epsilon_V\ll 1 \quad \Longleftrightarrow \quad q\gg 1.}
$$

**Consistency check:** passed
