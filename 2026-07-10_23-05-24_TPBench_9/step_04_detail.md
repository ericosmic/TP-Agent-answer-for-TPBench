# Step 4 — Separate variables and integrate the first-order slow-roll ODE using the initial condition $\phi(t=0)=\phi_0$ to solve explicitly for $\phi(t)$.

## Solution Reasoning

The Step 3 ODE has the separable form $\dot\phi=Ae^{-B\phi}$. Multiplying both sides by $e^{B\phi}$ gives $e^{B\phi}d\phi=A dt$. The integral over $\phi$ is elementary, $\int e^{B\phi}d\phi=e^{B\phi}/B$. Applying the definite limits imposed by $\phi(0)=\phi_0$ fixes the integration constant uniquely. Solving the resulting exponential equation for $\phi(t)$ gives the logarithmic expression. Substituting $B=1/(\sqrt{2q}M_P)$ and $AB=\sqrt{V_0/3}/(qM_P)$ yields the explicit solution.

## Result

Starting from the slow-roll ODE
$$
\frac{d\phi}{dt}\simeq \sqrt{\frac{2V_0}{3q}}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
define
$$
A\equiv \sqrt{\frac{2V_0}{3q}},\qquad B\equiv \frac{1}{2M_P}\sqrt{\frac{2}{q}}=\frac{1}{\sqrt{2q}\,M_P}.
$$
Then the equation is
$$
\frac{d\phi}{dt}=A e^{-B\phi}.
$$
Separating variables gives
$$
e^{B\phi}\,d\phi=A\,dt.
$$
Integrating from $t=0$ to $t$ and from $\phi_0$ to $\phi(t)$,
$$
\int_{\phi_0}^{\phi(t)} e^{B\phi}\,d\phi=A\int_0^t dt'.
$$
Thus
$$
\frac{1}{B}\left[e^{B\phi(t)}-e^{B\phi_0}\right]=At.
$$
Therefore
$$
e^{B\phi(t)}=e^{B\phi_0}+ABt.
$$
Using
$$
AB=\sqrt{\frac{2V_0}{3q}}\frac{1}{\sqrt{2q}\,M_P}=\frac{1}{qM_P}\sqrt{\frac{V_0}{3}},
$$
we obtain
$$
e^{\phi(t)/(\sqrt{2q}\,M_P)}=e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t.
$$
Taking the logarithm,
$$
\boxed{\phi(t)\simeq \sqrt{2q}\,M_P\ln\left[e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t\right].}
$$
Equivalently,
$$
\boxed{\phi(t)\simeq \phi_0+\sqrt{2q}\,M_P\ln\left[1+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,e^{-\phi_0/(\sqrt{2q}\,M_P)}t\right].}
$$

## Physical Interpretation

Starting from the slow-roll ODE
$$
\frac{d\phi}{dt}\simeq \sqrt{\frac{2V_0}{3q}}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
define
$$
A\equiv \sqrt{\frac{2V_0}{3q}},\qquad B\equiv \frac{1}{2M_P}\sqrt{\frac{2}{q}}=\frac{1}{\sqrt{2q}\,M_P}.
$$
Then the equation is
$$
\frac{d\phi}{dt}=A e^{-B\phi}.
$$
Separating variables gives
$$
e^{B\phi}\,d\phi=A\,dt.
$$
Integrating from $t=0$ to $t$ and from $\phi_0$ to $\phi(t)$,
$$
\int_{\phi_0}^{\phi(t)} e^{B\phi}\,d\phi=A\int_0^t dt'.
$$
Thus
$$
\frac{1}{B}\left[e^{B\phi(t)}-e^{B\phi_0}\right]=At.
$$
Therefore
$$
e^{B\phi(t)}=e^{B\phi_0}+ABt.
$$
Using
$$
AB=\sqrt{\frac{2V_0}{3q}}\frac{1}{\sqrt{2q}\,M_P}=\frac{1}{qM_P}\sqrt{\frac{V_0}{3}},
$$
we obtain
$$
e^{\phi(t)/(\sqrt{2q}\,M_P)}=e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t.
$$
Taking the logarithm,
$$
\boxed{\phi(t)\simeq \sqrt{2q}\,M_P\ln\left[e^{\phi_0/(\sqrt{2q}\,M_P)}+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,t\right].}
$$
Equivalently,
$$
\boxed{\phi(t)\simeq \phi_0+\sqrt{2q}\,M_P\ln\left[1+\frac{1}{qM_P}\sqrt{\frac{V_0}{3}}\,e^{-\phi_0/(\sqrt{2q}\,M_P)}t\right].}
$$

**Consistency check:** passed
