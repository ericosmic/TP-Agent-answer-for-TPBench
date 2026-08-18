# Step 3 — Compute $V'(\phi)$ for $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$ and substitute into the slow-roll equation to obtain a first-order ODE for $\phi(t)$.

## Solution Reasoning

The derivative follows by the chain rule: the exponential factor is unchanged and multiplied by the derivative of its argument, $-\sqrt{2/q}/M_P$. Since $V'(\phi)<0$ for positive $V_0$ and $q>0$, the slow-roll equation $3H\dot\phi\simeq -V'(\phi)$ gives $\dot\phi>0$, meaning the field rolls toward larger $\phi$ down the decreasing exponential potential. Substituting the potential-dominated Friedmann equation eliminates $H$ and yields a first-order ODE purely for $\phi(t)$.

## Result

For
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
we differentiate with respect to $\phi$:
$$
V'(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]\left(-\frac{1}{M_P}\sqrt{\frac{2}{q}}\right).
$$
Thus
$$
\boxed{V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi)}.
$$
The slow-roll equation is
$$
3H\dot\phi\simeq -V'(\phi).
$$
Substituting $V'(\phi)$ gives
$$
3H\dot\phi\simeq \frac{1}{M_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right].
$$
Equivalently,
$$
\boxed{\dot\phi\simeq \frac{1}{3HM_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]}.
$$
Using the slow-roll Friedmann equation
$$
H\simeq \sqrt{\frac{V(\phi)}{3M_P^2}},
$$
this becomes an autonomous first-order ODE for $\phi(t)$:
$$
\dot\phi\simeq \sqrt{\frac{2}{3q}}\sqrt{V(\phi)}.
$$
Since
$$
\sqrt{V(\phi)}=\sqrt{V_0}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
the ODE is
$$
\boxed{\frac{d\phi}{dt}\simeq \sqrt{\frac{2V_0}{3q}}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]}.
$$

## Physical Interpretation

For
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
we differentiate with respect to $\phi$:
$$
V'(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]\left(-\frac{1}{M_P}\sqrt{\frac{2}{q}}\right).
$$
Thus
$$
\boxed{V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi)}.
$$
The slow-roll equation is
$$
3H\dot\phi\simeq -V'(\phi).
$$
Substituting $V'(\phi)$ gives
$$
3H\dot\phi\simeq \frac{1}{M_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right].
$$
Equivalently,
$$
\boxed{\dot\phi\simeq \frac{1}{3HM_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]}.
$$
Using the slow-roll Friedmann equation
$$
H\simeq \sqrt{\frac{V(\phi)}{3M_P^2}},
$$
this becomes an autonomous first-order ODE for $\phi(t)$:
$$
\dot\phi\simeq \sqrt{\frac{2}{3q}}\sqrt{V(\phi)}.
$$
Since
$$
\sqrt{V(\phi)}=\sqrt{V_0}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
the ODE is
$$
\boxed{\frac{d\phi}{dt}\simeq \sqrt{\frac{2V_0}{3q}}\exp\left[-\frac{1}{2}\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right]}.
$$

**Consistency check:** passed
