# Step 2 — Separate variables as $\frac{dN}{C-C_A N^2}=dt$ and integrate both sides, using the substitution $x=N\sqrt{C_A/C}$ to obtain an inverse hyperbolic tangent relation.

## Solution Reasoning

The ODE is separable because $C$ and $C_A$ are constants. Factoring $C$ from the denominator gives a standard integral of the form $\int dx/(1-x^2)$ after the dimensionless substitution $x=N\sqrt{C_A/C}$. This integral is $\operatorname{arctanh}x$, leading directly to the relation between $N$ and $t$. The initial condition $N(0)=0$ fixes the integration constant to zero.

## Result

Starting from
$$
\frac{dN}{C-C_A N^2}=dt,
$$
write the denominator as
$$
C-C_A N^2=C\left(1-\frac{C_A}{C}N^2\right).
$$
Define
$$
x=N\sqrt{\frac{C_A}{C}},
$$
so that
$$
dx=\sqrt{\frac{C_A}{C}}\,dN,
\qquad dN=\sqrt{\frac{C}{C_A}}\,dx.
$$
Then
$$
\int \frac{dN}{C-C_A N^2}
=\int \frac{\sqrt{C/C_A}\,dx}{C(1-x^2)}
=\frac{1}{\sqrt{C C_A}}\int \frac{dx}{1-x^2}.
$$
Using
$$
\int \frac{dx}{1-x^2}=\operatorname{arctanh}x,
$$
we obtain
$$
\frac{1}{\sqrt{C C_A}}\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=t+K.
$$
Equivalently,
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,(t+K).
$$
Applying $N(0)=0$ gives
$$
\operatorname{arctanh}(0)=\sqrt{C C_A}\,K,
$$
so $K=0$. Therefore the inverse hyperbolic tangent relation is
$$
\boxed{\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,t.}
$$

## Physical Interpretation

Starting from
$$
\frac{dN}{C-C_A N^2}=dt,
$$
write the denominator as
$$
C-C_A N^2=C\left(1-\frac{C_A}{C}N^2\right).
$$
Define
$$
x=N\sqrt{\frac{C_A}{C}},
$$
so that
$$
dx=\sqrt{\frac{C_A}{C}}\,dN,
\qquad dN=\sqrt{\frac{C}{C_A}}\,dx.
$$
Then
$$
\int \frac{dN}{C-C_A N^2}
=\int \frac{\sqrt{C/C_A}\,dx}{C(1-x^2)}
=\frac{1}{\sqrt{C C_A}}\int \frac{dx}{1-x^2}.
$$
Using
$$
\int \frac{dx}{1-x^2}=\operatorname{arctanh}x,
$$
we obtain
$$
\frac{1}{\sqrt{C C_A}}\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=t+K.
$$
Equivalently,
$$
\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,(t+K).
$$
Applying $N(0)=0$ gives
$$
\operatorname{arctanh}(0)=\sqrt{C C_A}\,K,
$$
so $K=0$. Therefore the inverse hyperbolic tangent relation is
$$
\boxed{\operatorname{arctanh}\left(N\sqrt{\frac{C_A}{C}}\right)=\sqrt{C C_A}\,t.}
$$

**Consistency check:** passed
