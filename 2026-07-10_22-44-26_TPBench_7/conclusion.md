## Solution Plan
  1. Identify the relevant tree-level process from $\mathcal{L}=\sum_{i=1}^2\left[\frac{1}{2}(\partial_\mu\phi_i)(\partial^\mu\phi_i)-\frac{m_i^2}{2}\phi_i\phi_i\right]-\frac{\lambda}{4}\phi_1^2\phi_2^2$ and extract the quartic vertex for $\phi_1\phi_1\phi_2\phi_2$.
  2. Compute the leading invariant amplitude $\mathcal{M}$ for $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)\to\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$ and note that accuracy to $O(\lambda^2)$ in the cross section requires only the tree amplitude, since $|\mathcal{M}_{\rm tree}|^2=O(\lambda^2)$.
  3. Write the general CM-frame two-body differential cross section formula for identical final particles, including the phase-space factor $\frac{|\vec{k}_1'|}{|\vec{k}_1|}$ and the symmetry factor $\frac{1}{2!}$ for the two final $\phi_2$ particles.
  4. Express $|\vec{k}_1|$ and $|\vec{k}_1'|$ in terms of the Mandelstam variable $s$ and masses $m_1,m_2$ using $|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}$ and $|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}$, equivalently through the Källén function.
  5. Combine the amplitude and phase space to obtain $\frac{d\sigma}{d\Omega}$ to $O(\lambda^2)$, optionally indicating that the result is angle-independent and depends on Mandelstam variables through $s$ with $s+t+u=2m_1^2+2m_2^2$.

---

## Execution Step Results

### Step 1: Identify the relevant tree-level process from $\mathcal{L}=\sum_{i=1}^2\left[\frac{1}{2}(\partial_\mu\phi_i)(\partial^\mu\phi_i)-\frac{m_i^2}{2}\phi_i\phi_i\right]-\frac{\lambda}{4}\phi_1^2\phi_2^2$ and extract the quartic vertex for $\phi_1\phi_1\phi_2\phi_2$.

**Reasoning:**
The kinetic and mass terms only determine propagators and do not generate an interaction. The only interaction term is quartic and contains exactly two powers of $\phi_1$ and two powers of $\phi_2$, so it directly connects the external fields in the process $\phi_1\phi_1\to\phi_2\phi_2$. Writing the interaction as $-\lambda/(2!2!)\,\phi_1^2\phi_2^2$ makes clear that differentiating the interaction action with respect to two $\phi_1$ fields and two $\phi_2$ fields gives the vertex factor $-i\lambda$. Therefore the tree-level diagram is a single contact diagram with no internal propagator.

**Result:**
The relevant tree-level process is the single contact interaction
$$
\phi_1\phi_1 \to \phi_2\phi_2,
$$
mediated directly by the quartic term
$$
\mathcal{L}_{\rm int}=-\frac{\lambda}{4}\phi_1^2\phi_2^2.
$$
Since
$$
\frac{\lambda}{4}\phi_1^2\phi_2^2=\frac{\lambda}{2!2!}\phi_1^2\phi_2^2,
$$
the symmetry factors for two identical $\phi_1$ legs and two identical $\phi_2$ legs are already included. Therefore the four-point Feynman rule for the vertex with two $\phi_1$ lines and two $\phi_2$ lines is
$$
\boxed{-i\lambda}.
$$
Thus, at tree level, the invariant amplitude satisfies
$$
i\mathcal{M}_{\rm tree}=-i\lambda,
$$
or equivalently
$$
\boxed{\mathcal{M}_{\rm tree}=-\lambda}.
$$

**Analysis:**
The kinetic and mass terms only determine propagators and do not generate an interaction. The only interaction term is quartic and contains exactly two powers of $\phi_1$ and two powers of $\phi_2$, so it directly connects the external fields in the process $\phi_1\phi_1\to\phi_2\phi_2$. Writing the interaction as $-\lambda/(2!2!)\,\phi_1^2\phi_2^2$ makes clear that differentiating the interaction action with respect to two $\phi_1$ fields and two $\phi_2$ fields gives the vertex factor $-i\lambda$. Therefore the tree-level diagram is a single contact diagram with no internal propagator.

### Step 2: Compute the leading invariant amplitude $\mathcal{M}$ for $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)\to\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$ and note that accuracy to $O(\lambda^2)$ in the cross section requires only the tree amplitude, since $|\mathcal{M}_{\rm tree}|^2=O(\lambda^2)$.

**Reasoning:**
The interaction is $\mathcal{L}_{\rm int}=-(\lambda/4)\phi_1^2\phi_2^2=-(\lambda/(2!2!))\phi_1^2\phi_2^2$, so differentiating the interaction with respect to two $\phi_1$ fields and two $\phi_2$ fields gives the four-point Feynman rule $-i\lambda$. The process has exactly two incoming $\phi_1$ particles and two outgoing $\phi_2$ particles, so the leading diagram is this contact interaction and there are no propagators or kinematic dependence at tree level. Therefore $i\mathcal{M}_{\rm tree}=-i\lambda$, i.e. $\mathcal{M}_{\rm tree}=-\lambda$. Squaring gives $|\mathcal{M}_{\rm tree}|^2=\lambda^2$, which is already $O(\lambda^2)$. Loop corrections would modify the amplitude at higher order and only affect the cross section starting at $O(\lambda^3)$ through interference with the tree amplitude.

**Result:**
The leading contribution is the single contact diagram. With the convention that the $S$-matrix element contains $i\mathcal{M}$, the quartic vertex gives
$$
i\mathcal{M}_{\rm tree}=-i\lambda,
$$
so
$$
\boxed{\mathcal{M}_{\rm tree}=-\lambda.}
$$
Therefore
$$
\boxed{|\mathcal{M}_{\rm tree}|^2=\lambda^2.}
$$
Since the differential cross section through $O(\lambda^2)$ depends on $|\mathcal{M}|^2$, only this tree amplitude is required. If
$$
\mathcal{M}=\mathcal{M}_{\rm tree}+\mathcal{M}_{\rm loop}+\cdots,
$$
with $\mathcal{M}_{\rm tree}=O(\lambda)$ and loop corrections beginning at $O(\lambda^2)$, then
$$
|\mathcal{M}|^2=|\mathcal{M}_{\rm tree}|^2+2\operatorname{Re}(\mathcal{M}_{\rm tree}^*\mathcal{M}_{\rm loop})+\cdots
=O(\lambda^2)+O(\lambda^3)+\cdots.
$$
Thus the cross section accurate to $O(\lambda^2)$ is obtained solely from $\mathcal{M}_{\rm tree}=-\lambda$.

**Analysis:**
The interaction is $\mathcal{L}_{\rm int}=-(\lambda/4)\phi_1^2\phi_2^2=-(\lambda/(2!2!))\phi_1^2\phi_2^2$, so differentiating the interaction with respect to two $\phi_1$ fields and two $\phi_2$ fields gives the four-point Feynman rule $-i\lambda$. The process has exactly two incoming $\phi_1$ particles and two outgoing $\phi_2$ particles, so the leading diagram is this contact interaction and there are no propagators or kinematic dependence at tree level. Therefore $i\mathcal{M}_{\rm tree}=-i\lambda$, i.e. $\mathcal{M}_{\rm tree}=-\lambda$. Squaring gives $|\mathcal{M}_{\rm tree}|^2=\lambda^2$, which is already $O(\lambda^2)$. Loop corrections would modify the amplitude at higher order and only affect the cross section starting at $O(\lambda^3)$ through interference with the tree amplitude.

### Step 3: Write the general CM-frame two-body differential cross section formula for identical final particles, including the phase-space factor $\frac{|\vec{k}_1'|}{|\vec{k}_1|}$ and the symmetry factor $\frac{1}{2!}$ for the two final $\phi_2$ particles.

**Reasoning:**
The Lorentz-invariant two-body phase space in the CM frame gives the standard factor $(64\pi^2 s)^{-1}|\vec{k}_f|/|\vec{k}_i|$ multiplying $|\mathcal{M}|^2$. Here $|\vec{k}_i|=|\vec{k}_1|$ for the incoming $\phi_1\phi_1$ pair and $|\vec{k}_f|=|\vec{k}_1'|$ for the outgoing $\phi_2\phi_2$ pair. Because the two outgoing particles are identical, integrating over final phase space without a symmetry factor would double count physically identical final states, so one includes a factor $1/2!$.

**Result:**
For a general $2\to 2$ process in the CM frame, the differential cross section is
$$
\frac{d\sigma}{d\Omega}
= \frac{1}{64\pi^2 s}\frac{|\vec{k}_1'|}{|\vec{k}_1|}\,|\mathcal{M}|^2.
$$
Since the two final particles are identical $\phi_2$ particles, the final-state phase space must be divided by $2!$. Therefore
$$
\boxed{
\frac{d\sigma}{d\Omega}
= \frac{1}{2!}\frac{1}{64\pi^2 s}\frac{|\vec{k}_1'|}{|\vec{k}_1|}\,|\mathcal{M}|^2
}
$$
or equivalently
$$
\boxed{
\frac{d\sigma}{d\Omega}
= \frac{1}{128\pi^2 s}\frac{|\vec{k}_1'|}{|\vec{k}_1|}\,|\mathcal{M}|^2.
}
$$

**Analysis:**
The Lorentz-invariant two-body phase space in the CM frame gives the standard factor $(64\pi^2 s)^{-1}|\vec{k}_f|/|\vec{k}_i|$ multiplying $|\mathcal{M}|^2$. Here $|\vec{k}_i|=|\vec{k}_1|$ for the incoming $\phi_1\phi_1$ pair and $|\vec{k}_f|=|\vec{k}_1'|$ for the outgoing $\phi_2\phi_2$ pair. Because the two outgoing particles are identical, integrating over final phase space without a symmetry factor would double count physically identical final states, so one includes a factor $1/2!$.

### Step 4: Express $|\vec{k}_1|$ and $|\vec{k}_1'|$ in terms of the Mandelstam variable $s$ and masses $m_1,m_2$ using $|\vec{k}_1|=\frac{1}{2}\sqrt{s-4m_1^2}$ and $|\vec{k}_1'|=\frac{1}{2}\sqrt{s-4m_2^2}$, equivalently through the Källén function.

**Reasoning:**
In the CM frame, the two incoming three-momenta are equal and opposite, so the total spatial momentum vanishes and $\sqrt{s}$ is the total CM energy. Since the initial particles have equal mass $m_1$, their energies are equal, giving $\sqrt{s}=2\sqrt{|\vec{k}_1|^2+m_1^2}$. Solving this equation yields $|\vec{k}_1|=\frac12\sqrt{s-4m_1^2}$. The same argument applies to the final particles of equal mass $m_2$, giving $|\vec{k}_1'|=\frac12\sqrt{s-4m_2^2}$. These are the equal-mass special cases of the standard Källén-function expression $|\vec{p}|=\sqrt{\lambda_K(s,m_a^2,m_b^2)}/(2\sqrt{s})$.

**Result:**
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

**Analysis:**
In the CM frame, the two incoming three-momenta are equal and opposite, so the total spatial momentum vanishes and $\sqrt{s}$ is the total CM energy. Since the initial particles have equal mass $m_1$, their energies are equal, giving $\sqrt{s}=2\sqrt{|\vec{k}_1|^2+m_1^2}$. Solving this equation yields $|\vec{k}_1|=\frac12\sqrt{s-4m_1^2}$. The same argument applies to the final particles of equal mass $m_2$, giving $|\vec{k}_1'|=\frac12\sqrt{s-4m_2^2}$. These are the equal-mass special cases of the standard Källén-function expression $|\vec{p}|=\sqrt{\lambda_K(s,m_a^2,m_b^2)}/(2\sqrt{s})$.

### Step 5: Combine the amplitude and phase space to obtain $\frac{d\sigma}{d\Omega}$ to $O(\lambda^2)$, optionally indicating that the result is angle-independent and depends on Mandelstam variables through $s$ with $s+t+u=2m_1^2+2m_2^2$.

**Reasoning:**
The interaction $-\lambda \phi_1^2\phi_2^2/4$ gives a single four-point contact vertex $-i\lambda$, so with the convention $i\mathcal{M}$ for the scattering amplitude one has $\mathcal{M}_{\rm tree}=-\lambda$ and therefore $|\mathcal{M}_{\rm tree}|^2=\lambda^2$. Since loop corrections start at higher order in the amplitude, their interference contributes only at $O(\lambda^3)$ to the cross section, so the tree amplitude is sufficient for a result through $O(\lambda^2)$. The standard CM two-body formula is $d\sigma/d\Omega=(64\pi^2s)^{-1}(|\vec k_f|/|\vec k_i|)|\mathcal{M}|^2$. The final particles are two identical $\phi_2$ quanta, so the full phase space is divided by $2!$, giving the prefactor $1/(128\pi^2s)$. In the CM frame, $|\vec k_i|=\frac12\sqrt{s-4m_1^2}$ and $|\vec k_f|=\frac12\sqrt{s-4m_2^2}$, leading directly to the displayed expression. Because the contact amplitude is momentum-independent, the result has no angular dependence and no separate $t$ or $u$ dependence at this order.

**Result:**
Combining the tree-level result $|\mathcal{M}|^2=\lambda^2$ with the CM two-body phase space, including the $1/2!$ symmetry factor for the two identical final $\phi_2$ particles, gives
$$
\frac{d\sigma}{d\Omega}
=\frac{1}{2!}\frac{1}{64\pi^2 s}\frac{|\vec k_1'|}{|\vec k_1|}\,|\mathcal{M}|^2+O(\lambda^3).
$$
Thus
$$
\boxed{
\frac{d\sigma}{d\Omega}
=\frac{\lambda^2}{128\pi^2 s}
\sqrt{\frac{s-4m_2^2}{s-4m_1^2}}
+O(\lambda^3)
}
$$
for $s\ge 4m_2^2$, with the initial state requiring $s\ge 4m_1^2$. Equivalently, using the Källén function $\lambda_K(x,y,z)=x^2+y^2+z^2-2xy-2xz-2yz$,
$$
\boxed{
\frac{d\sigma}{d\Omega}
=\frac{\lambda^2}{128\pi^2 s}
\sqrt{\frac{\lambda_K(s,m_2^2,m_2^2)}{\lambda_K(s,m_1^2,m_1^2)}}
+O(\lambda^3)
}.
$$
The result is angle-independent at this order because the amplitude comes only from a contact interaction. Hence the dependence on Mandelstam variables is only through $s$, with
$$
s+t+u=2m_1^2+2m_2^2.
$$

**Analysis:**
The interaction $-\lambda \phi_1^2\phi_2^2/4$ gives a single four-point contact vertex $-i\lambda$, so with the convention $i\mathcal{M}$ for the scattering amplitude one has $\mathcal{M}_{\rm tree}=-\lambda$ and therefore $|\mathcal{M}_{\rm tree}|^2=\lambda^2$. Since loop corrections start at higher order in the amplitude, their interference contributes only at $O(\lambda^3)$ to the cross section, so the tree amplitude is sufficient for a result through $O(\lambda^2)$. The standard CM two-body formula is $d\sigma/d\Omega=(64\pi^2s)^{-1}(|\vec k_f|/|\vec k_i|)|\mathcal{M}|^2$. The final particles are two identical $\phi_2$ quanta, so the full phase space is divided by $2!$, giving the prefactor $1/(128\pi^2s)$. In the CM frame, $|\vec k_i|=\frac12\sqrt{s-4m_1^2}$ and $|\vec k_f|=\frac12\sqrt{s-4m_2^2}$, leading directly to the displayed expression. Because the contact amplitude is momentum-independent, the result has no angular dependence and no separate $t$ or $u$ dependence at this order.

---

## Final Result
(no final result)