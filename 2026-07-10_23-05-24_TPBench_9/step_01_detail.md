# Step 1 — State the Euler–Lagrange equation from $S = \int dt\, a^3(t) \left\{ \frac{1}{2} \dot{\phi}^2 - V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] \right\}$, giving $\ddot{\phi}+3H\dot{\phi}+V'(\phi)=0$, with $H=\dot a/a$ and $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$.

## Solution Reasoning

The Lagrangian is $L=a^3(t)[\frac12\dot\phi^2 - V(\phi)]$. Treating $a(t)$ as a background function for the variation with respect to $\phi$, the canonical momentum is $\partial L/\partial\dot\phi=a^3\dot\phi$. The field derivative is $\partial L/\partial\phi=-a^3V'(\phi)$. Substitution into the Euler--Lagrange equation yields $d(a^3\dot\phi)/dt+a^3V'(\phi)=0$. Expanding $d(a^3\dot\phi)/dt=a^3\ddot\phi+3a^2\dot a\dot\phi$ and dividing by $a^3$ gives the friction term $3H\dot\phi$, with $H=\dot a/a$.

## Result

Starting from
$$
S=\int dt\,L,\qquad L=a^3(t)\left\{\frac12\dot\phi^2 - V(\phi)\right\},
$$
with
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right],
$$
the Euler--Lagrange equation is
$$
\frac{d}{dt}\left(\frac{\partial L}{\partial \dot\phi}\right)-\frac{\partial L}{\partial \phi}=0.
$$
Since
$$
\frac{\partial L}{\partial \dot\phi}=a^3\dot\phi,
\qquad
\frac{\partial L}{\partial \phi}=-a^3 V'(\phi),
$$
we obtain
$$
\frac{d}{dt}\left(a^3\dot\phi\right)+a^3V'(\phi)=0.
$$
Expanding the time derivative gives
$$
a^3\ddot\phi+3a^2\dot a\dot\phi+a^3V'(\phi)=0.
$$
Dividing by $a^3$ and using $H=\dot a/a$, the scalar equation of motion is
$$
\boxed{\ddot\phi+3H\dot\phi+V'(\phi)=0.}
$$
For the given exponential potential,
$$
V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi),
$$
so equivalently
$$
\ddot\phi+3H\dot\phi-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]=0.
$$

## Physical Interpretation

Starting from
$$
S=\int dt\,L,\qquad L=a^3(t)\left\{\frac12\dot\phi^2 - V(\phi)\right\},
$$
with
$$
V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right],
$$
the Euler--Lagrange equation is
$$
\frac{d}{dt}\left(\frac{\partial L}{\partial \dot\phi}\right)-\frac{\partial L}{\partial \phi}=0.
$$
Since
$$
\frac{\partial L}{\partial \dot\phi}=a^3\dot\phi,
\qquad
\frac{\partial L}{\partial \phi}=-a^3 V'(\phi),
$$
we obtain
$$
\frac{d}{dt}\left(a^3\dot\phi\right)+a^3V'(\phi)=0.
$$
Expanding the time derivative gives
$$
a^3\ddot\phi+3a^2\dot a\dot\phi+a^3V'(\phi)=0.
$$
Dividing by $a^3$ and using $H=\dot a/a$, the scalar equation of motion is
$$
\boxed{\ddot\phi+3H\dot\phi+V'(\phi)=0.}
$$
For the given exponential potential,
$$
V'(\phi)=-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V(\phi),
$$
so equivalently
$$
\ddot\phi+3H\dot\phi-\frac{1}{M_P}\sqrt{\frac{2}{q}}\,V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]=0.
$$

**Consistency check:** passed
