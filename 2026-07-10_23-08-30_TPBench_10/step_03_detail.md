# Step 3 — Check the derivative terms proportional to $\partial_{\mu}\phi$ and $\partial_{\mu}\bar{\phi}$, using $\eta$ spacetime-independent and the identities involving $\sigma^{\mu}_{\alpha\dot{\alpha}}$ and $\bar{\sigma}^{\mu\dot{\alpha}\alpha}$, to verify that the remaining variation is a total derivative.

## Solution Reasoning

The key point is that the scalar variation contributes terms proportional to $\eta\partial_\mu\xi\partial^\mu\bar\phi$ and $\bar\eta\partial_\mu\bar\xi\partial^\mu\phi$. These cancel the symmetric metric part of the fermion-kinetic derivative variation once the two-component sigma matrix Clifford identities are used. The remaining pieces contain only $\sigma^{\mu\nu}$ or $\bar\sigma^{\mu\nu}$, which are antisymmetric Lorentz tensors. Such terms are total derivatives because differentiating the proposed current produces an additional term involving $\partial_\mu\partial_\nu\phi$ or $\partial_\mu\partial_\nu\bar\phi$, and this vanishes upon contraction with an antisymmetric matrix. The constancy of $\eta$ and $\bar\eta$ is essential because otherwise derivatives of the supersymmetry parameter would remain.

## Result

Substitute
$$
\delta_\eta\phi=\sqrt2\eta\xi,\qquad \delta_\eta\bar\phi=\sqrt2\bar\eta\bar\xi
$$
into the derivative part of the variation. Since $\eta$ and $\bar\eta$ are constant,
$$
\partial_\mu(\delta\phi)=\sqrt2\eta\partial_\mu\xi,
\qquad
\partial_\mu(\delta\bar\phi)=\sqrt2\bar\eta\partial_\mu\bar\xi.
$$
The terms involving $\partial_\mu\bar\phi$ and $\partial_\mu\xi$ are therefore
$$
\delta\mathcal L_{\eta,\partial\bar\phi}
=\sqrt2\partial_\mu\bar\phi\,\eta\sigma^\mu\bar\sigma^\nu\partial_\nu\xi
+\sqrt2\partial_\mu\bar\phi\,\eta\partial^\mu\xi.
$$
Using the Clifford identity, with the sign appropriate to the metric convention of the Lagrangian, the symmetric part of $\sigma^\mu\bar\sigma^\nu$ cancels the explicit metric term, leaving only the antisymmetric part:
$$
\delta\mathcal L_{\eta,\partial\bar\phi}
=2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\partial_\nu\xi,
$$
where $\sigma^{\mu\nu}$ is antisymmetric in $\mu,\nu$. Hence
$$
2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\partial_\nu\xi
=\partial_\nu\left(2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\xi\right),
$$
because the extra term contains $\partial_\nu\partial_\mu\bar\phi\,\sigma^{\mu\nu}=0$.

Similarly, the terms involving $\partial_\mu\phi$ and $\partial_\mu\bar\xi$ reduce, after integrating the term with $\partial_\mu\partial_\nu\phi$ by parts and using
$$
\bar\sigma^\mu\sigma^\nu+\bar\sigma^\nu\sigma^\mu=\pm2g^{\mu\nu},
$$
to the antisymmetric combination
$$
\delta\mathcal L_{\bar\eta,\partial\phi}
=2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\partial_\nu\bar\xi,
$$
up to a total derivative. Since $\bar\sigma^{\mu\nu}$ is antisymmetric, this is also a divergence:
$$
2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\partial_\nu\bar\xi
=\partial_\nu\left(2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\bar\xi\right),
$$
again because $\partial_\nu\partial_\mu\phi$ is symmetric.

Thus all remaining derivative terms are total derivatives. Consequently, after the $F$-dependent terms cancel as in Step 2, the full variation satisfies
$$
\delta_\eta\mathcal L=\partial_\mu K^\mu,
$$
so the action is invariant for fields obeying the usual boundary conditions.

## Physical Interpretation

Substitute
$$
\delta_\eta\phi=\sqrt2\eta\xi,\qquad \delta_\eta\bar\phi=\sqrt2\bar\eta\bar\xi
$$
into the derivative part of the variation. Since $\eta$ and $\bar\eta$ are constant,
$$
\partial_\mu(\delta\phi)=\sqrt2\eta\partial_\mu\xi,
\qquad
\partial_\mu(\delta\bar\phi)=\sqrt2\bar\eta\partial_\mu\bar\xi.
$$
The terms involving $\partial_\mu\bar\phi$ and $\partial_\mu\xi$ are therefore
$$
\delta\mathcal L_{\eta,\partial\bar\phi}
=\sqrt2\partial_\mu\bar\phi\,\eta\sigma^\mu\bar\sigma^\nu\partial_\nu\xi
+\sqrt2\partial_\mu\bar\phi\,\eta\partial^\mu\xi.
$$
Using the Clifford identity, with the sign appropriate to the metric convention of the Lagrangian, the symmetric part of $\sigma^\mu\bar\sigma^\nu$ cancels the explicit metric term, leaving only the antisymmetric part:
$$
\delta\mathcal L_{\eta,\partial\bar\phi}
=2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\partial_\nu\xi,
$$
where $\sigma^{\mu\nu}$ is antisymmetric in $\mu,\nu$. Hence
$$
2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\partial_\nu\xi
=\partial_\nu\left(2\sqrt2\,\partial_\mu\bar\phi\,\eta\sigma^{\mu\nu}\xi\right),
$$
because the extra term contains $\partial_\nu\partial_\mu\bar\phi\,\sigma^{\mu\nu}=0$.

Similarly, the terms involving $\partial_\mu\phi$ and $\partial_\mu\bar\xi$ reduce, after integrating the term with $\partial_\mu\partial_\nu\phi$ by parts and using
$$
\bar\sigma^\mu\sigma^\nu+\bar\sigma^\nu\sigma^\mu=\pm2g^{\mu\nu},
$$
to the antisymmetric combination
$$
\delta\mathcal L_{\bar\eta,\partial\phi}
=2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\partial_\nu\bar\xi,
$$
up to a total derivative. Since $\bar\sigma^{\mu\nu}$ is antisymmetric, this is also a divergence:
$$
2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\partial_\nu\bar\xi
=\partial_\nu\left(2\sqrt2\,\partial_\mu\phi\,\bar\eta\bar\sigma^{\mu\nu}\bar\xi\right),
$$
again because $\partial_\nu\partial_\mu\phi$ is symmetric.

Thus all remaining derivative terms are total derivatives. Consequently, after the $F$-dependent terms cancel as in Step 2, the full variation satisfies
$$
\delta_\eta\mathcal L=\partial_\mu K^\mu,
$$
so the action is invariant for fields obeying the usual boundary conditions.

**Consistency check:** passed
