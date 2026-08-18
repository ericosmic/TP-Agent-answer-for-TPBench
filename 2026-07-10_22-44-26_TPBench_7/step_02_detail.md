# Step 2 — Compute the leading invariant amplitude $\mathcal{M}$ for $\phi_1(\vec{k}_1)\phi_1(-\vec{k}_1)\to\phi_2(\vec{k}_1')\phi_2(-\vec{k}_1')$ and note that accuracy to $O(\lambda^2)$ in the cross section requires only the tree amplitude, since $|\mathcal{M}_{\rm tree}|^2=O(\lambda^2)$.

## Solution Reasoning

The interaction is $\mathcal{L}_{\rm int}=-(\lambda/4)\phi_1^2\phi_2^2=-(\lambda/(2!2!))\phi_1^2\phi_2^2$, so differentiating the interaction with respect to two $\phi_1$ fields and two $\phi_2$ fields gives the four-point Feynman rule $-i\lambda$. The process has exactly two incoming $\phi_1$ particles and two outgoing $\phi_2$ particles, so the leading diagram is this contact interaction and there are no propagators or kinematic dependence at tree level. Therefore $i\mathcal{M}_{\rm tree}=-i\lambda$, i.e. $\mathcal{M}_{\rm tree}=-\lambda$. Squaring gives $|\mathcal{M}_{\rm tree}|^2=\lambda^2$, which is already $O(\lambda^2)$. Loop corrections would modify the amplitude at higher order and only affect the cross section starting at $O(\lambda^3)$ through interference with the tree amplitude.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
