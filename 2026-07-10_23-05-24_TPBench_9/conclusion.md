## Solution Plan
  1. State the Euler–Lagrange equation from $S = \int dt\, a^3(t) \left\{ \frac{1}{2} \dot{\phi}^2 - V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] \right\}$, giving $\ddot{\phi}+3H\dot{\phi}+V'(\phi)=0$, with $H=\dot a/a$ and $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$.
  2. Apply the slow-roll assumptions $\ddot{\phi}\ll 3H\dot{\phi}$ and $\dot{\phi}^2/2\ll V(\phi)$, together with the Friedmann equation $H^2\simeq V(\phi)/(3M_P^2)$, to reduce the equation to $3H\dot{\phi}\simeq -V'(\phi)$.
  3. Compute $V'(\phi)$ for $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$ and substitute into the slow-roll equation to obtain a first-order ODE for $\phi(t)$.
  4. Separate variables and integrate the first-order slow-roll ODE using the initial condition $\phi(t=0)=\phi_0$ to solve explicitly for $\phi(t)$.
  5. Present the final integrated slow-roll solution $\phi(t)$, check that it satisfies $\phi(0)=\phi_0$, and optionally express the validity condition through the slow-roll parameter $\epsilon_V=\frac{M_P^2}{2}\left(V'/V\right)^2=1/q$, requiring $q\gg 1$ for slow roll.

---

## Execution Step Results

### Step 1: State the Euler–Lagrange equation from $S = \int dt\, a^3(t) \left\{ \frac{1}{2} \dot{\phi}^2 - V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] \right\}$, giving $\ddot{\phi}+3H\dot{\phi}+V'(\phi)=0$, with $H=\dot a/a$ and $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$.

**Reasoning:**
The Lagrangian is $L=a^3(t)[\frac12\dot\phi^2 - V(\phi)]$. Treating $a(t)$ as a background function for the variation with respect to $\phi$, the canonical momentum is $\partial L/\partial\dot\phi=a^3\dot\phi$. The field derivative is $\partial L/\partial\phi=-a^3V'(\phi)$. Substitution into the Euler--Lagrange equation yields $d(a^3\dot\phi)/dt+a^3V'(\phi)=0$. Expanding $d(a^3\dot\phi)/dt=a^3\ddot\phi+3a^2\dot a\dot\phi$ and dividing by $a^3$ gives the friction term $3H\dot\phi$, with $H=\dot a/a$.

**Result:**
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

**Analysis:**
The Lagrangian is $L=a^3(t)[\frac12\dot\phi^2 - V(\phi)]$. Treating $a(t)$ as a background function for the variation with respect to $\phi$, the canonical momentum is $\partial L/\partial\dot\phi=a^3\dot\phi$. The field derivative is $\partial L/\partial\phi=-a^3V'(\phi)$. Substitution into the Euler--Lagrange equation yields $d(a^3\dot\phi)/dt+a^3V'(\phi)=0$. Expanding $d(a^3\dot\phi)/dt=a^3\ddot\phi+3a^2\dot a\dot\phi$ and dividing by $a^3$ gives the friction term $3H\dot\phi$, with $H=\dot a/a$.

### Step 2: Apply the slow-roll assumptions $\ddot{\phi}\ll 3H\dot{\phi}$ and $\dot{\phi}^2/2\ll V(\phi)$, together with the Friedmann equation $H^2\simeq V(\phi)/(3M_P^2)$, to reduce the equation to $3H\dot{\phi}\simeq -V'(\phi)$.

**Reasoning:**
The exact equation from the action contains three terms: scalar acceleration $\ddot\phi$, Hubble friction $3H\dot\phi$, and the potential force $V'(\phi)$. In slow-roll inflation the acceleration term is assumed small compared with the friction term, so it is dropped. This leaves $3H\dot\phi+V'(\phi)\simeq 0$. Separately, the condition $\dot\phi^2/2\ll V(\phi)$ implies that the inflaton energy density is approximately $\rho_\phi\simeq V(\phi)$, so the Friedmann equation reduces to $H^2\simeq V/(3M_P^2)$. For the given exponential potential, differentiating with respect to $\phi$ gives a negative derivative, $V'=-(1/M_P)\sqrt{2/q}\,V$, so the field rolls toward larger $\phi$ and $\dot\phi$ is positive in this convention.

**Result:**
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

**Analysis:**
The exact equation from the action contains three terms: scalar acceleration $\ddot\phi$, Hubble friction $3H\dot\phi$, and the potential force $V'(\phi)$. In slow-roll inflation the acceleration term is assumed small compared with the friction term, so it is dropped. This leaves $3H\dot\phi+V'(\phi)\simeq 0$. Separately, the condition $\dot\phi^2/2\ll V(\phi)$ implies that the inflaton energy density is approximately $\rho_\phi\simeq V(\phi)$, so the Friedmann equation reduces to $H^2\simeq V/(3M_P^2)$. For the given exponential potential, differentiating with respect to $\phi$ gives a negative derivative, $V'=-(1/M_P)\sqrt{2/q}\,V$, so the field rolls toward larger $\phi$ and $\dot\phi$ is positive in this convention.

### Step 3: Compute $V'(\phi)$ for $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$ and substitute into the slow-roll equation to obtain a first-order ODE for $\phi(t)$.

**Reasoning:**
The derivative follows by the chain rule: the exponential factor is unchanged and multiplied by the derivative of its argument, $-\sqrt{2/q}/M_P$. Since $V'(\phi)<0$ for positive $V_0$ and $q>0$, the slow-roll equation $3H\dot\phi\simeq -V'(\phi)$ gives $\dot\phi>0$, meaning the field rolls toward larger $\phi$ down the decreasing exponential potential. Substituting the potential-dominated Friedmann equation eliminates $H$ and yields a first-order ODE purely for $\phi(t)$.

**Result:**
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

**Analysis:**
The derivative follows by the chain rule: the exponential factor is unchanged and multiplied by the derivative of its argument, $-\sqrt{2/q}/M_P$. Since $V'(\phi)<0$ for positive $V_0$ and $q>0$, the slow-roll equation $3H\dot\phi\simeq -V'(\phi)$ gives $\dot\phi>0$, meaning the field rolls toward larger $\phi$ down the decreasing exponential potential. Substituting the potential-dominated Friedmann equation eliminates $H$ and yields a first-order ODE purely for $\phi(t)$.

### Step 4: Separate variables and integrate the first-order slow-roll ODE using the initial condition $\phi(t=0)=\phi_0$ to solve explicitly for $\phi(t)$.

**Reasoning:**
The Step 3 ODE has the separable form $\dot\phi=Ae^{-B\phi}$. Multiplying both sides by $e^{B\phi}$ gives $e^{B\phi}d\phi=A dt$. The integral over $\phi$ is elementary, $\int e^{B\phi}d\phi=e^{B\phi}/B$. Applying the definite limits imposed by $\phi(0)=\phi_0$ fixes the integration constant uniquely. Solving the resulting exponential equation for $\phi(t)$ gives the logarithmic expression. Substituting $B=1/(\sqrt{2q}M_P)$ and $AB=\sqrt{V_0/3}/(qM_P)$ yields the explicit solution.

**Result:**
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

**Analysis:**
The Step 3 ODE has the separable form $\dot\phi=Ae^{-B\phi}$. Multiplying both sides by $e^{B\phi}$ gives $e^{B\phi}d\phi=A dt$. The integral over $\phi$ is elementary, $\int e^{B\phi}d\phi=e^{B\phi}/B$. Applying the definite limits imposed by $\phi(0)=\phi_0$ fixes the integration constant uniquely. Solving the resulting exponential equation for $\phi(t)$ gives the logarithmic expression. Substituting $B=1/(\sqrt{2q}M_P)$ and $AB=\sqrt{V_0/3}/(qM_P)$ yields the explicit solution.

### Step 5: Present the final integrated slow-roll solution $\phi(t)$, check that it satisfies $\phi(0)=\phi_0$, and optionally express the validity condition through the slow-roll parameter $\epsilon_V=\frac{M_P^2}{2}\left(V'/V\right)^2=1/q$, requiring $q\gg 1$ for slow roll.

**Reasoning:**
Starting from the previously integrated relation, one simply solves for $\phi(t)$ by taking the logarithm. The equivalent shifted form is obtained by factoring $e^{\phi_0/(\sqrt{2q}M_P)}$ inside the logarithm, which makes the initial condition explicit. Substitution of $t=0$ gives the logarithm of unity in the shifted form, hence $\phi(0)=\phi_0$. The slow-roll validity condition follows from differentiating the exponential potential: $V'/V=-\sqrt{2/q}/M_P$, giving $\epsilon_V=1/q$, so slow roll requires $q\gg 1$.

**Result:**
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

**Analysis:**
Starting from the previously integrated relation, one simply solves for $\phi(t)$ by taking the logarithm. The equivalent shifted form is obtained by factoring $e^{\phi_0/(\sqrt{2q}M_P)}$ inside the logarithm, which makes the initial condition explicit. Substitution of $t=0$ gives the logarithm of unity in the shifted form, hence $\phi(0)=\phi_0$. The slow-roll validity condition follows from differentiating the exponential potential: $V'/V=-\sqrt{2/q}/M_P$, giving $\epsilon_V=1/q$, so slow roll requires $q\gg 1$.

---

## Final Result
(no final result)