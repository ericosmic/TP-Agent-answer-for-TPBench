# Step 2 — Before applying the one-pole contour estimate, impose a UV-consistent prescription: verify whether the sharp $\Theta$ transition produces a power-law high-$k$ tail in $|\beta(k)|$ from discontinuities of derivatives of $a(\eta)$, and either include the corresponding boundary contribution or state that a smoothed/adiabatic transition is assumed so that the one-pole exponential result is meaningful and avoids a UV catastrophe in $\int d^{3}k\,|\beta(k)|^{2}$ or $\int d^{3}k\,\omega_{k}|\beta(k)|^{2}$.

## Solution Reasoning

The sudden transition found in Step 1 makes $a$ and $a'$ continuous but $a''$ discontinuous. Since $\omega^2=k^2+m^2a^2$, $\omega$ and $\omega'$ are continuous, so the integrand prefactor $f=\omega'/(2\omega)$ is continuous. However $f'$ contains the term $m^2aa''/(2\omega^2)$ and therefore inherits a finite jump proportional to $[a'']$. For an oscillatory integral with a continuous amplitude but a jump in its first derivative, the first nonzero boundary contribution appears after two integrations by parts and scales as $[f']/(2\omega)^2$. Evaluating this at the transition gives $|\beta_{\rm bdry}|\sim k^{-4}$. This is a real-axis nonanalyticity contribution, independent of the complex pole contribution, and must be included unless one assumes the physical transition is smoothed. Although this particular $k^{-4}$ tail is UV-convergent in both number and energy density, it still dominates over any exponentially suppressed one-pole estimate at asymptotically high $k$.

## Result

Before using a complex one-pole saddle/pole estimate, the real-axis nonanalyticity at the sudden transition must be accounted for. With $\eta_e=0$, define
$$
f(\eta)\equiv {\omega_k'(\eta)\over 2\omega_k(\eta)}={m^2a(\eta)a'(\eta)\over 2\omega_k^2(\eta)},\qquad \omega_k^2=k^2+m^2a^2.
$$
Since $a$ and $a'$ are continuous at $\eta=0$, both $\omega_k$ and $f$ are continuous. However $a''$ jumps, so $f'$ jumps. The jump is
$$
[f']_{0}\equiv f'(0^+)-f'(0^-)
={m^2a_e\over 2\omega_e^2}\,[a'']_0,
\qquad \omega_e^2=k^2+m^2a_e^2,
$$
where
$$
[a'']_0=a''(0^+)-a''(0^-)=\frac12a_e^3H_I^2-2a_e^3H_I^2=-\frac32a_e^3H_I^2.
$$
Thus
$$
[f']_0=-{3m^2a_e^4H_I^2\over 4\left(k^2+m^2a_e^2\right)}.
$$
A repeated integration-by-parts/high-$k$ Fourier estimate of
$$
\beta(k)\simeq \int d\eta\, f(\eta)\exp\left[-2i\int_0^\eta \omega_k(\eta')d\eta'\right]
$$
therefore gives the boundary contribution
$$
\beta_{\rm bdry}(k)\simeq { [f']_0\over (2i\omega_e)^2}
=-{[f']_0\over 4\omega_e^2},
$$
up to an irrelevant phase convention. Hence
$$
|\beta_{\rm bdry}(k)|\simeq {3m^2a_e^4H_I^2\over 16\left(k^2+m^2a_e^2\right)^2}
\xrightarrow{k\gg a_eH_I,\,ma_e} {3m^2a_e^4H_I^2\over 16k^4}.
$$
Therefore the sharp $\Theta$ transition produces a power-law high-$k$ tail, $|\beta(k)|\propto k^{-4}$, originating from the jump in $a''$. This tail is not exponentially small and will dominate over the complex one-pole exponential at sufficiently large $k$ if the transition is treated as exactly sudden.

For the present $C^1$ scale factor the induced tail is sufficiently soft that
$$
\int d^3k\,|\beta|^2\sim \int^\infty dk\,k^2 k^{-8}
$$
and
$$
\int d^3k\,\omega_k|\beta|^2\sim \int^\infty dk\,k^3 k^{-8}
$$
are UV convergent. Nevertheless, the one-pole exponential is not the true leading asymptotic of the exactly sharp model. Thus there are two consistent prescriptions:

1. Include the real-axis boundary term above together with the one-pole contribution, in which case the high-$k$ asymptotic is power-law rather than exponential.

2. Declare that the $\Theta$ transition is an idealization of a sufficiently smooth/adiabatic transition, with $a(\eta)$ smoothed near $\eta=0$ so that the derivative discontinuity is removed. Then the artificial boundary tail is absent or pushed beyond the regime of interest, and the subsequent one-pole exponential estimate is meaningful as the leading contribution.

## Physical Interpretation

Before using a complex one-pole saddle/pole estimate, the real-axis nonanalyticity at the sudden transition must be accounted for. With $\eta_e=0$, define
$$
f(\eta)\equiv {\omega_k'(\eta)\over 2\omega_k(\eta)}={m^2a(\eta)a'(\eta)\over 2\omega_k^2(\eta)},\qquad \omega_k^2=k^2+m^2a^2.
$$
Since $a$ and $a'$ are continuous at $\eta=0$, both $\omega_k$ and $f$ are continuous. However $a''$ jumps, so $f'$ jumps. The jump is
$$
[f']_{0}\equiv f'(0^+)-f'(0^-)
={m^2a_e\over 2\omega_e^2}\,[a'']_0,
\qquad \omega_e^2=k^2+m^2a_e^2,
$$
where
$$
[a'']_0=a''(0^+)-a''(0^-)=\frac12a_e^3H_I^2-2a_e^3H_I^2=-\frac32a_e^3H_I^2.
$$
Thus
$$
[f']_0=-{3m^2a_e^4H_I^2\over 4\left(k^2+m^2a_e^2\right)}.
$$
A repeated integration-by-parts/high-$k$ Fourier estimate of
$$
\beta(k)\simeq \int d\eta\, f(\eta)\exp\left[-2i\int_0^\eta \omega_k(\eta')d\eta'\right]
$$
therefore gives the boundary contribution
$$
\beta_{\rm bdry}(k)\simeq { [f']_0\over (2i\omega_e)^2}
=-{[f']_0\over 4\omega_e^2},
$$
up to an irrelevant phase convention. Hence
$$
|\beta_{\rm bdry}(k)|\simeq {3m^2a_e^4H_I^2\over 16\left(k^2+m^2a_e^2\right)^2}
\xrightarrow{k\gg a_eH_I,\,ma_e} {3m^2a_e^4H_I^2\over 16k^4}.
$$
Therefore the sharp $\Theta$ transition produces a power-law high-$k$ tail, $|\beta(k)|\propto k^{-4}$, originating from the jump in $a''$. This tail is not exponentially small and will dominate over the complex one-pole exponential at sufficiently large $k$ if the transition is treated as exactly sudden.

For the present $C^1$ scale factor the induced tail is sufficiently soft that
$$
\int d^3k\,|\beta|^2\sim \int^\infty dk\,k^2 k^{-8}
$$
and
$$
\int d^3k\,\omega_k|\beta|^2\sim \int^\infty dk\,k^3 k^{-8}
$$
are UV convergent. Nevertheless, the one-pole exponential is not the true leading asymptotic of the exactly sharp model. Thus there are two consistent prescriptions:

1. Include the real-axis boundary term above together with the one-pole contribution, in which case the high-$k$ asymptotic is power-law rather than exponential.

2. Declare that the $\Theta$ transition is an idealization of a sufficiently smooth/adiabatic transition, with $a(\eta)$ smoothed near $\eta=0$ so that the derivative discontinuity is removed. Then the artificial boundary tail is absent or pushed beyond the regime of interest, and the subsequent one-pole exponential estimate is meaningful as the leading contribution.

**Consistency check:** passed
