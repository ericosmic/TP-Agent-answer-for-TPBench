# Step 3 — Apply $N(0)=0$ to fix the integration constant and solve for $N(t)$ explicitly in terms of $\tanh$.

## Solution Reasoning

The separated and integrated ODE gives an inverse hyperbolic tangent relation between $N$ and $t$. The initial condition $N(0)=0$ forces the integration constant to vanish because $\operatorname{arctanh}(0)=0$. Inverting the relation with the hyperbolic tangent then yields the explicit solution. The prefactor $\sqrt{C/C_A}$ is the equilibrium particle number, while the argument $\sqrt{C C_A}\,t$ sets the equilibration timescale.

## Result

Starting from
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,(t+K),
$$
impose $N(0)=0$:
$$
\operatorname{arctanh}(0)=\sqrt{C C_A}\,K.
$$
Since $\operatorname{arctanh}(0)=0$, we get
$$
K=0.
$$
Thus
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,t.
$$
Taking $\tanh$ of both sides gives
$$
N\sqrt{\frac{C_A}{C}}=\tanh\left(\sqrt{C C_A}\,t\right).
$$
Therefore,
$$
\boxed{N(t)=\sqrt{\frac{C}{C_A}}\,\tanh\left(\sqrt{C C_A}\,t\right)}.
$$

## Physical Interpretation

Starting from
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,(t+K),
$$
impose $N(0)=0$:
$$
\operatorname{arctanh}(0)=\sqrt{C C_A}\,K.
$$
Since $\operatorname{arctanh}(0)=0$, we get
$$
K=0.
$$
Thus
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,t.
$$
Taking $\tanh$ of both sides gives
$$
N\sqrt{\frac{C_A}{C}}=\tanh\left(\sqrt{C C_A}\,t\right).
$$
Therefore,
$$
\boxed{N(t)=\sqrt{\frac{C}{C_A}}\,\tanh\left(\sqrt{C C_A}\,t\right)}.
$$

**Consistency check:** passed
