# Plan

**步骤数：5**

---

### Step 1

**Description**: State the Euler–Lagrange equation from $S = \int dt\, a^3(t) \left\{ \frac{1}{2} \dot{\phi}^2 - V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] \right\}$, giving $\ddot{\phi}+3H\dot{\phi}+V'(\phi)=0$, with $H=\dot a/a$ and $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$.

- **Needs computation**: No
- **Reasoning**: This is a standard variational derivation for a homogeneous scalar in an FRW background and can be done analytically by hand.

---

### Step 2

**Description**: Apply the slow-roll assumptions $\ddot{\phi}\ll 3H\dot{\phi}$ and $\dot{\phi}^2/2\ll V(\phi)$, together with the Friedmann equation $H^2\simeq V(\phi)/(3M_P^2)$, to reduce the equation to $3H\dot{\phi}\simeq -V'(\phi)$.

- **Needs computation**: No
- **Reasoning**: This step uses standard slow-roll approximations and algebraic substitution, not requiring symbolic software.

---

### Step 3

**Description**: Compute $V'(\phi)$ for $V(\phi)=V_0\exp\left[-\sqrt{\frac{2}{q}}\left(\frac{\phi}{M_P}\right)\right]$ and substitute into the slow-roll equation to obtain a first-order ODE for $\phi(t)$.

- **Needs computation**: No
- **Reasoning**: The derivative of the exponential potential and simplification of the ODE are straightforward analytic operations.

---

### Step 4

**Description**: Separate variables and integrate the first-order slow-roll ODE using the initial condition $\phi(t=0)=\phi_0$ to solve explicitly for $\phi(t)$.

- **Needs computation**: No
- **Reasoning**: The resulting ODE is separable and has an elementary exponential integral, so Mathematica is unnecessary.

---

### Step 5

**Description**: Present the final integrated slow-roll solution $\phi(t)$, check that it satisfies $\phi(0)=\phi_0$, and optionally express the validity condition through the slow-roll parameter $\epsilon_V=\frac{M_P^2}{2}\left(V'/V\right)^2=1/q$, requiring $q\gg 1$ for slow roll.

- **Needs computation**: No
- **Reasoning**: The final check and slow-roll consistency condition are analytic and conceptual.

## Symmetries
- Spatial homogeneity of $\phi(t)$
- Isotropy and homogeneity of the FRW background
- Energy conservation encoded in the scalar equation of motion

## Approximations
- Slow-roll regime requires $\epsilon_V=1/q\ll 1$, hence $q\gg 1$
- Neglect $\ddot{\phi}$ relative to $3H\dot{\phi}$
- Neglect kinetic energy $\dot{\phi}^2/2$ relative to $V(\phi)$

## Other Constraints
- Assume $V_0>0$ so that $H$ is real during inflation
- Assume $M_P$ is the reduced Planck mass
- Use the expanding branch $H>0$