# Analyse Step 3 Iteration 1

**Description:** Expand $\omega_k(\eta)$ locally around the selected $\tilde{\eta}$ and replace $\frac{\omega_k'}{2\omega_k}$ by its leading one-pole form; deform the real-$\eta$ contour to the steepest-descent contour through $\tilde{\eta}$, retaining only the residue/phase contribution from this pole and discarding subdominant poles according to Step 2.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The required prior information is complete. The needed inputs are the post-transition analytic continuation $a(\eta)=a_e[1+\frac{a_eH_I}{2}(\eta-\eta_e)]^2$, the definition $z(\eta)=1+\frac{a_eH_I}{2}(\eta-\eta_e)$, the frequency $\omega_k^2=k^2+m^2a_e^2z^4$, and the selected dominant turning point/pole $\tilde\eta=\eta_e+\frac{2}{a_eH_I}[(k/(ma_e))^{1/2}e^{i\pi/4}-1]$ from Step 2.

## Critical Rubrics

A correct answer must: (i) use the dominant turning point $\tilde\eta$ selected in Step 2; (ii) expand $\omega_k^2$ linearly as $Q'(\tilde\eta)(\eta-\tilde\eta)$ and hence $\omega_k\sim(\eta-\tilde\eta)^{1/2}$; (iii) obtain the leading pole $\omega_k'/(2\omega_k)\sim1/[4(\eta-\tilde\eta)]$ with residue $1/4$; (iv) state that the contour is deformed to the steepest-descent path through $\tilde\eta$; (v) keep only the residue/phase factor from this pole and discard subdominant poles; and (vi) present the resulting one-pole contribution proportional to $\exp[-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta]$, with only an orientation/Stokes sign ambiguity irrelevant for the magnitude.

## Candidate Result

Let
$$
z(\eta)=1+\frac{a_eH_I}{2}(\eta-\eta_e),\qquad \omega_k^2(\eta)=Q(\eta)=k^2+m^2a_e^2z^4.
$$
The selected pole/turning point is
$$
\tilde\eta=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{i\pi/4}-1\right],
\qquad \tilde z=z(\tilde\eta)=\left(\frac{k}{ma_e}\right)^{1/2}e^{i\pi/4}.
$$
Near $\eta=\tilde\eta$, write $\xi=\eta-\tilde\eta$. Since $Q(\tilde\eta)=0$ and the zero is simple,
$$
Q(\eta)=Q'(\tilde\eta)\xi+O(\xi^2),
$$
with
$$
Q'(\tilde\eta)=4m^2a_e^2\tilde z^3\frac{a_eH_I}{2}=2m^2a_e^3H_I\tilde z^3.
$$
Thus, on the chosen square-root branch,
$$
\omega_k(\eta)=\left[Q'(\tilde\eta)\right]^{1/2}\xi^{1/2}\left[1+O(\xi)\right].
$$
Consequently
$$
\frac{\omega_k'}{2\omega_k}
=\frac14\frac{Q'}{Q}
=\frac{1}{4(\eta-\tilde\eta)}+O(1).
$$
The phase integral is locally
$$
\int_{\eta_e}^{\eta}d\eta'\,\omega_k(\eta')
=S_{\tilde\eta}+\frac{2}{3}\left[Q'(\tilde\eta)\right]^{1/2}(\eta-\tilde\eta)^{3/2}+\cdots,
$$
where
$$
S_{\tilde\eta}\equiv\int_{\eta_e}^{\tilde\eta}d\eta\,\omega_k(\eta).
$$
The real-$\eta$ contour is then deformed to the steepest-descent contour through $\tilde\eta$. Keeping only this dominant pole and discarding the other turning points from Step 2 gives the one-pole approximation
$$
\beta(k)\simeq \operatorname{sgn}(\mathcal C)\,2\pi i\,\underset{\eta=\tilde\eta}{\mathrm{Res}}\left[\frac{1}{4(\eta-\tilde\eta)}e^{-2i\int_{\eta_e}^{\eta}d\eta'\,\omega_k(\eta')}\right],
$$
so
$$
\boxed{\beta(k)\simeq \operatorname{sgn}(\mathcal C)\,\frac{i\pi}{2}\exp\left[-2i\int_{\eta_e}^{\tilde\eta}d\eta\,\omega_k(\eta)\right]}.
$$
Here $\operatorname{sgn}(\mathcal C)=\pm1$ depends on the orientation/Stokes prescription of the deformed contour and is irrelevant for the magnitude. Therefore, at this stage,
$$
\boxed{|\beta(k)|_{\rm 1\ pole}\simeq \frac{\pi}{2}\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}d\eta\,\omega_k(\eta)\right]\right|}
$$
or equivalently
$$
|\beta(k)|_{\rm 1\ pole}\simeq \frac{\pi}{2}\exp\left[2\,\operatorname{Im}\int_{\eta_e}^{\tilde\eta}d\eta\,\omega_k(\eta)\right]
$$
with the sign of the imaginary part fixed by the chosen branch/steepest-descent prescription in the subsequent evaluation of the phase. The essential result of this step is the replacement
$$
\frac{\omega_k'}{2\omega_k}\longrightarrow \frac{1}{4(\eta-\tilde\eta)}
$$
and the retention of only the residue times the exponential phase evaluated at $\tilde\eta$.

## Reasoning

The zero of $\omega_k^2$ at $\tilde\eta$ is simple because $Q'(\tilde\eta)
eq0$. Therefore $\omega_k$ has a square-root branch point, $\omega_k\sim[Q'(\tilde\eta)]^{1/2}(\eta-\tilde\eta)^{1/2}$. Since $\omega_k'/(2\omega_k)=\frac14 Q'/Q$, this branch point appears in the logarithmic derivative as a simple pole with residue $1/4$. In the steepest-descent deformation the fast exponential is evaluated at the turning point to leading one-pole order, while the local $(\eta-\tilde\eta)^{3/2}$ correction controls the steepest direction but does not change the residue. All other poles/turning points are farther away or lie on subdominant contours according to Step 2, so they are discarded. The remaining contribution is thus the residue of the pole multiplied by the WKB phase evaluated at $\tilde\eta$, up to an orientation/Stokes sign irrelevant to $|\beta|$.
