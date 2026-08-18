# Step 2 — Apply the slow-roll assumptions $\ddot{\phi}\ll 3H\dot{\phi}$ and $\dot{\phi}^2/2\ll V(\phi)$, together with the Friedmann equation $H^2\simeq V(\phi)/(3M_P^2)$, to reduce the equation to $3H\dot{\phi}\simeq -V'(\phi)$.

## Solution Reasoning

The exact equation from the action contains three terms: scalar acceleration $\ddot\phi$, Hubble friction $3H\dot\phi$, and the potential force $V'(\phi)$. In slow-roll inflation the acceleration term is assumed small compared with the friction term, so it is dropped. This leaves $3H\dot\phi+V'(\phi)\simeq 0$. Separately, the condition $\dot\phi^2/2\ll V(\phi)$ implies that the inflaton energy density is approximately $\rho_\phi\simeq V(\phi)$, so the Friedmann equation reduces to $H^2\simeq V/(3M_P^2)$. For the given exponential potential, differentiating with respect to $\phi$ gives a negative derivative, $V'=-(1/M_P)\sqrt{2/q}\,V$, so the field rolls toward larger $\phi$ and $\dot\phi$ is positive in this convention.

## Result

Starting from the exact scalar field equation obtained in Step 1,
$$
\ddot\phi+3H\dot\phi+V'(\phi)=0,
$$
the slow-roll approximation neglects the acceleration term relative to Hubble friction,
$$
\ddot\phi\ll 3H\dot\phi.
$$
Therefore the equation of motion reduces to
$$
3H\dot\phi+V'(\phi)\simeq 0,
$$
or equivalently
$$
\boxed{3H\dot\phi\simeq -V'(\phi).}
$$
The second slow-roll condition,
$$
\frac12\dot\phi^2\ll V(\phi),
$$
ensures that the energy density is potential-dominated, so the Friedmann equation becomes
$$
H^2\simeq \frac{V(\phi)}{3M_P^2}.
$$
For the exponential potential
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
we have
$$
V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi).
$$
Thus the slow-roll equation may also be written as
$$
3H\dot\phi\simeq \frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi),
$$
with
$$
H\simeq \sqrt{\frac{V(\phi)}{3M_P^2}}.
$$

## Physical Interpretation

Starting from the exact scalar field equation obtained in Step 1,
$$
\ddot\phi+3H\dot\phi+V'(\phi)=0,
$$
the slow-roll approximation neglects the acceleration term relative to Hubble friction,
$$
\ddot\phi\ll 3H\dot\phi.
$$
Therefore the equation of motion reduces to
$$
3H\dot\phi+V'(\phi)\simeq 0,
$$
or equivalently
$$
\boxed{3H\dot\phi\simeq -V'(\phi).}
$$
The second slow-roll condition,
$$
\frac12\dot\phi^2\ll V(\phi),
$$
ensures that the energy density is potential-dominated, so the Friedmann equation becomes
$$
H^2\simeq \frac{V(\phi)}{3M_P^2}.
$$
For the exponential potential
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\frac{\phi}{M_P}\right],
$$
we have
$$
V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi).
$$
Thus the slow-roll equation may also be written as
$$
3H\dot\phi\simeq \frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi),
$$
with
$$
H\simeq \sqrt{\frac{V(\phi)}{3M_P^2}}.
$$

**Consistency check:** passed
