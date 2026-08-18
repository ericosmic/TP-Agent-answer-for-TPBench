# Analyse Step 2 Iteration 1

**Description:** Vary the scalar kinetic term $|\partial\phi|^{2}=\partial_{\mu}\bar{\phi}\,\partial^{\mu}\phi$ using the ansatz from Step 1, integrate by parts in the action, and isolate the terms proportional to $\eta\,\partial\xi\,\partial\bar{\phi}$ and $\bar{\eta}\,\partial\bar{\xi}\,\partial\phi$ that must cancel against corresponding pieces from the fermion kinetic variation.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The relevant prior result is Step 1: $\delta_\eta\phi=a\,\eta^\alpha\xi_\alpha\equiv a\,\eta\xi$ and $(\delta_\eta\phi)^\dagger=a^*\,\bar\eta_{\dot\alpha}\bar\xi^{\dot\alpha}\equiv a^*\,\bar\eta\bar\xi$, with $\eta$ spacetime independent. No further information is missing.

## Critical Rubrics

A correct solution must: use the Step 1 ansatz for $\delta\phi$ and $\delta\bar\phi$; use $\partial_\mu\eta=0$; vary $\partial_\mu\bar\phi\partial^\mu\phi$ by the product rule; integrate by parts only up to discarded surface terms in the action; and isolate with correct coefficients and signs the terms $a\,\eta^\alpha(\partial_\mu\xi_\alpha)\partial^\mu\bar\phi$ and $a^*\,\bar\eta_{\dot\alpha}(\partial_\mu\bar\xi^{\dot\alpha})\partial^\mu\phi$.

## Candidate Result

Using
$$
\delta_\eta\phi=a\,\eta^\alpha\xi_\alpha,\qquad \delta_\eta\bar\phi=a^*\,\bar\eta_{\dot\alpha}\bar\xi^{\dot\alpha},
$$
and $\partial_\mu\eta=\partial_\mu\bar\eta=0$, the scalar kinetic term varies as
$$
\delta_\eta\mathcal L_{\phi}
=\delta_\eta\left(\partial_\mu\bar\phi\,\partial^\mu\phi\right)
=\partial_\mu(\delta_\eta\bar\phi)\,\partial^\mu\phi
+\partial_\mu\bar\phi\,\partial^\mu(\delta_\eta\phi).
$$
Substituting the ansatz gives
$$
\delta_\eta\mathcal L_{\phi}
=a^*\,\bar\eta_{\dot\alpha}\,\partial_\mu\bar\xi^{\dot\alpha}\,\partial^\mu\phi
+a\,\partial_\mu\bar\phi\,\eta^\alpha\partial^\mu\xi_\alpha.
$$
Equivalently, in the action one may first integrate by parts:
$$
\delta_\eta S_\phi
=\int d^4x\left[\partial_\mu(\delta\bar\phi)\partial^\mu\phi+\partial_\mu\bar\phi\partial^\mu(\delta\phi)\right]
=-\int d^4x\left[\delta\bar\phi\,\Box\phi+(\Box\bar\phi)\delta\phi\right],
$$
up to a surface term. Inserting the ansatz and integrating by parts back onto the fermions yields the same non-boundary contribution
$$
\delta_\eta S_\phi
=\int d^4x\left[
a\,\eta^\alpha(\partial_\mu\xi_\alpha)\partial^\mu\bar\phi
+a^*\,\bar\eta_{\dot\alpha}(\partial_\mu\bar\xi^{\dot\alpha})\partial^\mu\phi
\right].
$$
Thus the isolated terms that must cancel the corresponding fermion-kinetic variation are
$$
\boxed{a\,\eta^\alpha(\partial_\mu\xi_\alpha)\partial^\mu\bar\phi}
\qquad\text{and}\qquad
\boxed{a^*\,\bar\eta_{\dot\alpha}(\partial_\mu\bar\xi^{\dot\alpha})\partial^\mu\phi}.
$$

## Reasoning

The scalar kinetic term depends only on derivatives of $\phi$ and $\bar\phi$, so its variation is obtained by the product rule. Since $\eta$ and $\bar\eta$ are constant infinitesimal parameters, derivatives act only on $\xi$ and $\bar\xi$ after inserting the Step 1 ansatz. In the action, integration by parts permits dropping total derivatives and rewriting the variation either in terms of $\delta\phi\,\Box\bar\phi$ and $\delta\bar\phi\,\Box\phi$, or equivalently in the first-derivative form. The latter directly displays the two structures relevant for cancellation with the derivative-dependent pieces of the fermion kinetic variation: one proportional to $\eta\,\partial\xi\,\partial\bar\phi$ with coefficient $a$, and its conjugate proportional to $\bar\eta\,\partial\bar\xi\,\partial\phi$ with coefficient $a^*$.
