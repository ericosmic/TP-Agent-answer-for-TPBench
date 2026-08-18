# Step 5 — Compare the one-pole exponential contribution with any UV boundary or sudden-transition contribution found earlier; report the dominant UV-safe expression for $|\beta(k)|$ and explicitly state the condition under which it avoids UV catastrophe, for example exponential suppression from an analytic or sufficiently smooth transition versus unacceptable power-law behavior from the sharp $\Theta$ idealization.

## Solution Reasoning

The comparison is between the complex-plane singularity contribution and the real-axis nonanalyticity contribution. The one-pole term is exponentially small at large $k$, scaling as $\exp[-{\rm const}\, k^{3/2}]$ in the dimensionless combination $[k/(a_eH_I)] [k/(ma_e)]^{1/2}$. The sharp transition gives a boundary term because $f(\eta)=\omega_k'/(2\omega_k)$ is continuous but $f'$ jumps, producing a $k^{-4}$ contribution. Any power law dominates an exponential at sufficiently large $k$, so the literal sharp-$\Theta$ asymptotic is the boundary term, not the pole term. Nevertheless, $k^{-4}$ is soft enough to make both $\int d^3k |\beta|^2$ and $\int d^3k\,\omega_k |\beta|^2$ converge. If the transition is smoothed so that the derivative discontinuity is removed, the boundary contribution disappears and the one-pole exponential becomes the dominant UV-safe estimate.

## Result

The one-pole contribution obtained from the dominant complex turning point is
$$
|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-\alpha\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right],
\qquad
\alpha\equiv \frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}.
$$
Equivalently,
$$
|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-2\sqrt{2}\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right],
\qquad
C=\int_0^1 dx\,\sqrt{1-x^4}.
$$
However, for the exact sharp $\Theta$ scale factor, the transition is only $C^1$ in conformal time: $a$ and $a'$ are continuous, but $a''$ jumps at $\eta=0$. This produces a real-axis boundary contribution
$$
|\beta_{\rm bdry}(k)|\simeq \frac{3m^2a_e^4H_I^2}{16\left(k^2+m^2a_e^2\right)^2}
\xrightarrow{k\gg a_eH_I,\,ma_e}
\frac{3m^2a_e^4H_I^2}{16k^4}.
$$
Since a power law dominates over an exponential at asymptotically large $k$, the exact sharp-$\Theta$ model has
$$
|\beta(k)|\simeq |\beta_{\rm bdry}(k)|
$$
in the strict UV, with the exponentially small pole term subleading.

Thus there are two physically distinct statements:

1. For the literal sharp $\Theta$ transition,
$$
|\beta(k)|\simeq \frac{3m^2a_e^4H_I^2}{16\left(k^2+m^2a_e^2\right)^2}
+O\!\left(\exp\left[-\alpha\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]\right),
$$
up to phases and possible interference. This is not exponentially suppressed, because it is an artifact of the nonanalytic transition. In the present $C^1$ case the $k^{-4}$ tail is still UV convergent for both number and energy densities:
$$
\int d^3k\,|\beta|^2\sim \int^\infty dk\,k^2k^{-8}<\infty,
\qquad
\int d^3k\,\omega_k|\beta|^2\sim \int^\infty dk\,k^3k^{-8}<\infty.
$$
So this particular power law is UV safe, but it is not the one-pole exponential asymptotic.

2. If the $\Theta$ transition is understood as an idealization of an analytic or sufficiently smooth adiabatic transition, so that the derivative discontinuity at $\eta=0$ is removed, then the artificial boundary term is absent or parametrically suppressed. In that UV-consistent smoothed model, the dominant one-pole result is
$$
\boxed{
|\beta(k)|\simeq \frac{\pi}{2}\exp\left[-\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]
}
$$
for $k/(a_eH_I)\to\infty$ and $0<m\lesssim H_I$.

The condition for avoiding a UV catastrophe is that the transition be analytic or sufficiently smooth/adiabatic so that no discontinuity produces a hard high-$k$ tail. Exponential suppression is manifestly UV safe. More generally, if a residual power-law tail $|\beta|\sim k^{-p}$ remains, finite particle number requires $p>3/2$, and finite energy density requires $p>2$ for relativistic UV modes. The present sharp model gives $p=4$, so it is convergent, but a less smooth sudden transition could yield an unacceptable UV-divergent power law. Therefore, the clean one-pole expression should be quoted as the dominant UV-safe result only after smoothing the sharp $\Theta$ idealization.

## Physical Interpretation

The one-pole contribution obtained from the dominant complex turning point is
$$
|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-\alpha\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right],
\qquad
\alpha\equiv \frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}.
$$
Equivalently,
$$
|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-2\sqrt{2}\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right],
\qquad
C=\int_0^1 dx\,\sqrt{1-x^4}.
$$
However, for the exact sharp $\Theta$ scale factor, the transition is only $C^1$ in conformal time: $a$ and $a'$ are continuous, but $a''$ jumps at $\eta=0$. This produces a real-axis boundary contribution
$$
|\beta_{\rm bdry}(k)|\simeq \frac{3m^2a_e^4H_I^2}{16\left(k^2+m^2a_e^2\right)^2}
\xrightarrow{k\gg a_eH_I,\,ma_e}
\frac{3m^2a_e^4H_I^2}{16k^4}.
$$
Since a power law dominates over an exponential at asymptotically large $k$, the exact sharp-$\Theta$ model has
$$
|\beta(k)|\simeq |\beta_{\rm bdry}(k)|
$$
in the strict UV, with the exponentially small pole term subleading.

Thus there are two physically distinct statements:

1. For the literal sharp $\Theta$ transition,
$$
|\beta(k)|\simeq \frac{3m^2a_e^4H_I^2}{16\left(k^2+m^2a_e^2\right)^2}
+O\!\left(\exp\left[-\alpha\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]\right),
$$
up to phases and possible interference. This is not exponentially suppressed, because it is an artifact of the nonanalytic transition. In the present $C^1$ case the $k^{-4}$ tail is still UV convergent for both number and energy densities:
$$
\int d^3k\,|\beta|^2\sim \int^\infty dk\,k^2k^{-8}<\infty,
\qquad
\int d^3k\,\omega_k|\beta|^2\sim \int^\infty dk\,k^3k^{-8}<\infty.
$$
So this particular power law is UV safe, but it is not the one-pole exponential asymptotic.

2. If the $\Theta$ transition is understood as an idealization of an analytic or sufficiently smooth adiabatic transition, so that the derivative discontinuity at $\eta=0$ is removed, then the artificial boundary term is absent or parametrically suppressed. In that UV-consistent smoothed model, the dominant one-pole result is
$$
\boxed{
|\beta(k)|\simeq \frac{\pi}{2}\exp\left[-\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]
}
$$
for $k/(a_eH_I)\to\infty$ and $0<m\lesssim H_I$.

The condition for avoiding a UV catastrophe is that the transition be analytic or sufficiently smooth/adiabatic so that no discontinuity produces a hard high-$k$ tail. Exponential suppression is manifestly UV safe. More generally, if a residual power-law tail $|\beta|\sim k^{-p}$ remains, finite particle number requires $p>3/2$, and finite energy density requires $p>2$ for relativistic UV modes. The present sharp model gives $p=4$, so it is convergent, but a less smooth sudden transition could yield an unacceptable UV-divergent power law. Therefore, the clean one-pole expression should be quoted as the dominant UV-safe result only after smoothing the sharp $\Theta$ idealization.

**Consistency check:** passed
