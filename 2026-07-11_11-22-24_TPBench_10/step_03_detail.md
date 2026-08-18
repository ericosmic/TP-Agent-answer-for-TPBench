# Step 3 — Choose $\delta_{\eta}\phi=\sqrt{2}\eta\xi$ and $\left(\delta_{\eta}\phi\right)^{\dagger}=\sqrt{2}\bar{\eta}\bar{\xi}$, then substitute these into the scalar kinetic variation $\delta |\partial\phi|^{2}$.

## Solution Reasoning

The scalar kinetic term varies by the product rule. The variation of $\phi$ contributes $\partial_\mu(\delta\phi)\partial^\mu\bar\phi$, while the variation of $\bar\phi$ contributes $\partial_\mu\phi\partial^\mu(\delta\bar\phi)$. With $\delta\phi=\sqrt2\eta\xi$ and $\delta\bar\phi=\sqrt2\bar\eta\bar\xi$, and with constant SUSY parameters, $\partial_\mu(\eta\xi)=\eta\partial_\mu\xi$ and $\partial^\mu(\bar\eta\bar\xi)=\bar\eta\partial^\mu\bar\xi$. This directly yields the stated expression.

## Result

Choose
$$
\delta_\eta\phi=\sqrt2\,\eta\xi,\qquad (\delta_\eta\phi)^\dagger=\delta_\eta\bar\phi=\sqrt2\,\bar\eta\bar\xi.
$$
The scalar kinetic term is
$$
|\partial\phi|^2=\partial_\mu\phi\,\partial^\mu\bar\phi.
$$
Therefore its variation is
$$
\delta_\eta |\partial\phi|^2
=\partial_\mu(\delta_\eta\phi)\partial^\mu\bar\phi
+\partial_\mu\phi\,\partial^\mu(\delta_\eta\bar\phi).
$$
Substituting the chosen transformations gives
$$
\delta_\eta |\partial\phi|^2
=\partial_\mu(\sqrt2\,\eta\xi)\partial^\mu\bar\phi
+\partial_\mu\phi\,\partial^\mu(\sqrt2\,\bar\eta\bar\xi).
$$
Since $\eta$ and $\bar\eta$ are spacetime independent,
$$
\boxed{
\delta_\eta |\partial\phi|^2
=\sqrt2\,\eta\,\partial_\mu\xi\,\partial^\mu\bar\phi
+\sqrt2\,\partial_\mu\phi\,\bar\eta\,\partial^\mu\bar\xi
}.
$$
Equivalently, using $\delta_\eta\bar\phi=\sqrt2\bar\eta\bar\xi$,
$$
\boxed{
\delta_\eta |\partial\phi|^2
=\sqrt2\,\eta\partial_\mu\xi\,\partial^\mu\bar\phi
+\sqrt2\,\bar\eta\partial^\mu\bar\xi\,\partial_\mu\phi
},
$$
where the ordering should be kept consistent with the Grassmann parity of the spinor factors.

## Physical Interpretation

Choose
$$
\delta_\eta\phi=\sqrt2\,\eta\xi,\qquad (\delta_\eta\phi)^\dagger=\delta_\eta\bar\phi=\sqrt2\,\bar\eta\bar\xi.
$$
The scalar kinetic term is
$$
|\partial\phi|^2=\partial_\mu\phi\,\partial^\mu\bar\phi.
$$
Therefore its variation is
$$
\delta_\eta |\partial\phi|^2
=\partial_\mu(\delta_\eta\phi)\partial^\mu\bar\phi
+\partial_\mu\phi\,\partial^\mu(\delta_\eta\bar\phi).
$$
Substituting the chosen transformations gives
$$
\delta_\eta |\partial\phi|^2
=\partial_\mu(\sqrt2\,\eta\xi)\partial^\mu\bar\phi
+\partial_\mu\phi\,\partial^\mu(\sqrt2\,\bar\eta\bar\xi).
$$
Since $\eta$ and $\bar\eta$ are spacetime independent,
$$
\boxed{
\delta_\eta |\partial\phi|^2
=\sqrt2\,\eta\,\partial_\mu\xi\,\partial^\mu\bar\phi
+\sqrt2\,\partial_\mu\phi\,\bar\eta\,\partial^\mu\bar\xi
}.
$$
Equivalently, using $\delta_\eta\bar\phi=\sqrt2\bar\eta\bar\xi$,
$$
\boxed{
\delta_\eta |\partial\phi|^2
=\sqrt2\,\eta\partial_\mu\xi\,\partial^\mu\bar\phi
+\sqrt2\,\bar\eta\partial^\mu\bar\xi\,\partial_\mu\phi
},
$$
where the ordering should be kept consistent with the Grassmann parity of the spinor factors.

**Consistency check:** passed
