# Step 4 — Express $|\vec{k}_1|$ and $|\vec{k}_1'|$ in terms of the Mandelstam variable $s$ and masses $m_1,m_2$ using $|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}$ and $|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}$, equivalently through the Källén function.

## Solution Reasoning

In the CM frame, the two incoming three-momenta are equal and opposite, so the total spatial momentum vanishes and $\sqrt{s}$ is the total CM energy. Since the initial particles have equal mass $m_1$, their energies are equal, giving $\sqrt{s}=2\sqrt{|\vec{k}_1|^2+m_1^2}$. Solving this equation yields $|\vec{k}_1|=\frac12\sqrt{s-4m_1^2}$. The same argument applies to the final particles of equal mass $m_2$, giving $|\vec{k}_1'|=\frac12\sqrt{s-4m_2^2}$. These are the equal-mass special cases of the standard Källén-function expression $|\vec{p}|=\sqrt{\lambda_K(s,m_a^2,m_b^2)}/(2\sqrt{s})$.

## Result

In the CM frame, the total four-momentum satisfies
$$
s=(p_1+p_2)^2=E_{\rm cm}^2.
$$
For the initial state $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)$, each particle has energy
$$
E_1=\sqrt{|\vec{k}_1|^2+m_1^2},
$$
and therefore
$$
\sqrt{s}=2E_1=2\sqrt{|\vec{k}_1|^2+m_1^2}.
$$
Solving gives
$$
\boxed{|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}}.
$$
Similarly, for the final state $\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$,
$$
\sqrt{s}=2E_2'=2\sqrt{|\vec{k}_1'|^2+m_2^2},
$$
so
$$
\boxed{|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}}.
$$
Equivalently, using the Källén function
$$
\lambda_K(x,y,z)=x^2+y^2+z^2-2xy-2xz-2yz,
$$
the general two-body CM momentum is
$$
|\vec{p}\,|=\frac{\sqrt{\lambda_K(s,m_a^2,m_b^2)}}{2\sqrt{s}}.
$$
Thus for equal masses in each pair,
$$
|\vec{k}_1|=\frac{\sqrt{\lambda_K(s,m_1^2,m_1^2)}}{2\sqrt{s}}
=\frac{1}{2}\sqrt{s-4m_1^2},
$$
and
$$
|\vec{k}_1'|=\frac{\sqrt{\lambda_K(s,m_2^2,m_2^2)}}{2\sqrt{s}}
=\frac{1}{2}\sqrt{s-4m_2^2}.
$$
Consequently,
$$
\boxed{\frac{|\vec{k}_1'|}{|\vec{k}_1|}
=\sqrt{\frac{s-4m_2^2}{s-4m_1^2}}
=\sqrt{\frac{\lambda_K(s,m_2^2,m_2^2)}{\lambda_K(s,m_1^2,m_1^2)}}.}
$$

## Physical Interpretation

In the CM frame, the total four-momentum satisfies
$$
s=(p_1+p_2)^2=E_{\rm cm}^2.
$$
For the initial state $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)$, each particle has energy
$$
E_1=\sqrt{|\vec{k}_1|^2+m_1^2},
$$
and therefore
$$
\sqrt{s}=2E_1=2\sqrt{|\vec{k}_1|^2+m_1^2}.
$$
Solving gives
$$
\boxed{|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}}.
$$
Similarly, for the final state $\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$,
$$
\sqrt{s}=2E_2'=2\sqrt{|\vec{k}_1'|^2+m_2^2},
$$
so
$$
\boxed{|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}}.
$$
Equivalently, using the Källén function
$$
\lambda_K(x,y,z)=x^2+y^2+z^2-2xy-2xz-2yz,
$$
the general two-body CM momentum is
$$
|\vec{p}\,|=\frac{\sqrt{\lambda_K(s,m_a^2,m_b^2)}}{2\sqrt{s}}.
$$
Thus for equal masses in each pair,
$$
|\vec{k}_1|=\frac{\sqrt{\lambda_K(s,m_1^2,m_1^2)}}{2\sqrt{s}}
=\frac{1}{2}\sqrt{s-4m_1^2},
$$
and
$$
|\vec{k}_1'|=\frac{\sqrt{\lambda_K(s,m_2^2,m_2^2)}}{2\sqrt{s}}
=\frac{1}{2}\sqrt{s-4m_2^2}.
$$
Consequently,
$$
\boxed{\frac{|\vec{k}_1'|}{|\vec{k}_1|}
=\sqrt{\frac{s-4m_2^2}{s-4m_1^2}}
=\sqrt{\frac{\lambda_K(s,m_2^2,m_2^2)}{\lambda_K(s,m_1^2,m_1^2)}}.}
$$

**Consistency check:** passed
