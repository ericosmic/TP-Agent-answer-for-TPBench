# Step 4 — Present the final solution and identify the equilibration time scale $\tau=(C C_A)^{-1/2}$ and equilibrium value $N_{\rm eq}=\sqrt{C/C_A}$.

## Solution Reasoning

From separation of variables, the integrated equation gives $\operatorname{arctanh}(N\sqrt{C_A/C})=\sqrt{C C_A}\,t$ after applying $N(0)=0$. Taking the hyperbolic tangent gives $N\sqrt{C_A/C}=\tanh(\sqrt{C C_A}\,t)$, hence $N(t)=\sqrt{C/C_A}\,\tanh(\sqrt{C C_A}\,t)$. The equilibrium value is obtained by setting $dN/dt=0$, giving $C-C_A N^2=0$, so $N_{\rm eq}=\sqrt{C/C_A}$ for the physical positive solution. Since $\sqrt{C C_A}=1/\tau$, the same solution becomes $N(t)=N_{\rm eq}\tanh(t/\tau)$.

## Result

The solution to
$$
\frac{dN}{dt}=C-C_A N^2, \qquad N(0)=0,
$$
is
$$
N(t)=\sqrt{\frac{C}{C_A}}\,\tanh\left(\sqrt{C C_A}\,t\right).
$$
Defining the equilibration time scale
$$
\tau=\frac{1}{\sqrt{C C_A}},
$$
and the equilibrium number
$$
N_{\rm eq}=\sqrt{\frac{C}{C_A}},
$$
the solution can be written compactly as
$$
\boxed{N(t)=N_{\rm eq}\,\tanh\left(\frac{t}{\tau}\right)}.
$$
At early times, $t\ll \tau$, one has $\tanh(t/\tau)\simeq t/\tau$, so
$$
N(t)\simeq Ct,
$$
corresponding to capture-dominated growth. At late times, $t\gg \tau$, $\tanh(t/\tau)\to 1$, and therefore
$$
N(t)\to N_{\rm eq}=\sqrt{\frac{C}{C_A}}.
$$
Thus $\tau=(C C_A)^{-1/2}$ is the characteristic equilibration time scale over which capture and annihilation approach balance.

## Physical Interpretation

The solution to
$$
\frac{dN}{dt}=C-C_A N^2, \qquad N(0)=0,
$$
is
$$
N(t)=\sqrt{\frac{C}{C_A}}\,\tanh\left(\sqrt{C C_A}\,t\right).
$$
Defining the equilibration time scale
$$
\tau=\frac{1}{\sqrt{C C_A}},
$$
and the equilibrium number
$$
N_{\rm eq}=\sqrt{\frac{C}{C_A}},
$$
the solution can be written compactly as
$$
\boxed{N(t)=N_{\rm eq}\,\tanh\left(\frac{t}{\tau}\right)}.
$$
At early times, $t\ll \tau$, one has $\tanh(t/\tau)\simeq t/\tau$, so
$$
N(t)\simeq Ct,
$$
corresponding to capture-dominated growth. At late times, $t\gg \tau$, $\tanh(t/\tau)\to 1$, and therefore
$$
N(t)\to N_{\rm eq}=\sqrt{\frac{C}{C_A}}.
$$
Thus $\tau=(C C_A)^{-1/2}$ is the characteristic equilibration time scale over which capture and annihilation approach balance.

**Consistency check:** passed
