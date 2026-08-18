# Session Queries

## 2026-07-10 23:08:30

Topic:
SUSY-Symmetry

Problem:
Consider the theory
$$
\begin{equation}
\mathcal{L}=i\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}\xi+|\partial\phi|^{2}-|F|^{2}
\end{equation}
$$
where $\xi$ is a 2-component Weyl spinor while $\phi$ and $F$ are
complex scalar fields. Suppose you want to make the following infinitesimal
transformation a symmetry of this theory:
$$
\begin{equation}
\delta_{\eta}\xi_{\alpha}=i\sqrt{2}\sigma_{\alpha\dot{\alpha}}^{\mu}\bar{\eta}^{\dot{\alpha}}\partial_{\mu}\phi+\sqrt{2}\eta_{\alpha}F
\end{equation}
$$

$$
\begin{align*}
\delta_{\eta}\bar{\xi}_{\dot{\beta}} & = [i\sqrt{2}\sigma_{\beta\dot{\alpha}}^{\mu}\bar{\eta}^{\dot{\alpha}}\partial_{\mu}\phi+\sqrt{2}\eta_{\beta}F]^{\dagger}\\
 & = -i\sqrt{2}(\bar{\eta}^{\dot{\alpha}}\sigma_{\dot{\alpha}\beta}^{\mu*})^{*}\partial_{\mu}\bar{\phi}+\sqrt{2}\bar{\eta}_{\dot{\beta}}\bar{F}\\
 & = -i\sqrt{2}\eta^{\alpha}\sigma_{\alpha\dot{\beta}}^{\mu}\partial_{\mu}\bar{\phi}+\sqrt{2}\bar{\eta}_{\dot{\beta}}\bar{F}
umberthis
\end{align*}
$$

$$
\begin{equation}
\delta_{\eta}F=i\sqrt{2}\bar{\eta}_{\dot{\alpha}}\bar{\sigma}^{\mu\dot{\alpha}\alpha}\partial_{\mu}\xi_{\alpha}=i\sqrt{2}\bar{\eta}\bar{\sigma}^{\mu}\partial_{\mu}\xi
\end{equation}
$$

$$
\begin{align*}
\delta_{\eta}\bar{F} & = -i\sqrt{2}(\bar{\eta}\bar{\sigma}^{\mu}\partial_{\mu}\xi)^{\dagger}\\
 & = -i\sqrt{2}(\partial_{\mu}\xi)^{\dagger}(\bar{\sigma}^{\mu})^{\dagger}(\bar{\eta})^{\dagger}\\
 & = -i\sqrt{2}\partial_{\mu}\bar{\xi}\bar{\sigma}^{\mu}\eta
umberthis
\end{align*}
$$
along with $\delta_{\eta}\phi$ and $\left(\delta_{\eta}\phi\right)^{\dagger}$
where $\eta$ is a spacetime-independent infinitesimal fermionic parameter
inducing the transformation. Find the transformation rule $\delta_{\eta}\phi$
and $\left(\delta_{\eta}\phi\right)^{\dagger}$ for the action associated
with $\mathcal{L}$ to remain invariant.

Domain:
HET
