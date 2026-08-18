# Analyse Step 5 Iteration 1

**Description:** Assemble the asymptotic one-pole result for $|\beta(k)|$ from the pole factor of Step 3 and the imaginary part of $S(k)$ from Step 4, and express the answer explicitly in terms of $k$, $a_e$, $H_I$, and $m$, together with the validity conditions $k/(a_eH_I)\to\infty$ and $0<m\lesssim H_I$.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The needed prior results are complete: Step 3 gives the one-pole residue prefactor $\pi/2$ in $|\beta|$, and Step 4 gives the leading imaginary WKB action $|\operatorname{Im}S(k)|$ at the dominant turning point.

## Critical Rubrics

A correct answer must include: (i) the one-pole prefactor $\pi/2$ from the residue of $\omega_k'/(2\omega_k)\sim 1/[4(\eta-\tilde\eta)]$; (ii) the exponential suppression with a minus sign, $\exp[-2|\operatorname{Im}S|]$; (iii) the explicit coefficient $\sqrt{2\pi}\Gamma(1/4)/(3\Gamma(3/4))$; (iv) the dependence $[k/(a_eH_I)](k/(ma_e))^{1/2}$ or equivalently $k^{3/2}/(a_eH_I\sqrt{ma_e})$; and (v) the validity conditions $k/(a_eH_I)\to\infty$, $0<m\lesssim H_I$, and dominance of the selected upper-half-plane pole.

## Candidate Result

From Step 3, the one-pole approximation gives
$$
\beta(k)\simeq \operatorname{sgn}(\mathcal C)\frac{i\pi}{2}\exp[-2iS(k)],
\qquad
S(k)=\int_{\eta_e}^{\tilde\eta}d\eta\,\omega_k(\eta),
$$
so the magnitude is determined by the imaginary part of the complex WKB action. With the physical Stokes prescription the contribution is exponentially suppressed:
$$
|\beta(k)|_{\rm 1\ pole}\simeq \frac{\pi}{2}\exp[-2|\operatorname{Im}S(k)|].
$$
Using Step 4,
$$
2|\operatorname{Im}S(k)|=
\frac{\sqrt{2\pi}\,\Gamma(1/4)}{3\Gamma(3/4)}
\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}
+\cdots .
$$
Therefore the assembled asymptotic one-pole result is
$$
\boxed{
|\beta(k)|\simeq
\frac{\pi}{2}
\exp\!\left[-\frac{\sqrt{2\pi}\,\Gamma(1/4)}{3\Gamma(3/4)}
\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]
}
$$
up to subleading corrections in the large-$k$ expansion and up to the usual Stokes/orientation phase, which does not affect the magnitude. Equivalently,
$$
|\beta(k)|\simeq
\frac{\pi}{2}
\exp\!\left[-\frac{\sqrt{2\pi}\,\Gamma(1/4)}{3\Gamma(3/4)}
\frac{k^{3/2}}{a_eH_I\sqrt{ma_e}}\right].
$$
This result is valid in the asymptotic regime
$$
\frac{k}{a_eH_I}\to\infty,
\qquad
0<m\lesssim H_I,
$$
with the one-pole approximation dominated by the upper-half-plane turning point with $\Re\tilde\eta>0$. More precisely, the expansion also assumes
$$
\rho=\left(\frac{k}{ma_e}\right)^{1/2}\gg 1,
$$
which is automatically compatible with the stated high-momentum limit for fixed $0<m\lesssim H_I$.

## Reasoning

Step 3 reduces the original oscillatory integral to a residue contribution at the dominant pole/turning point: $\beta\simeq (i\pi/2)e^{-2iS}$ up to an irrelevant sign. Taking the magnitude gives a factor $\pi/2$ times the exponential governed by the imaginary part of $S$. The physically relevant steepest-descent contour gives suppression, hence $\exp[-2|\operatorname{Im}S|]$ rather than exponential growth. Step 4 supplies $2|\operatorname{Im}S|$ explicitly as $[\sqrt{2\pi}\Gamma(1/4)/(3\Gamma(3/4))][k/(a_eH_I)](k/(ma_e))^{1/2}$ at leading order. Combining these two pieces directly yields the boxed formula.
