# Step 3 — Expand $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ near $\tilde{\eta}$ and determine the one-pole prefactor entering the contour approximation to $|\beta(k)|\approx\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{e}}^{\eta}d\eta'\omega_{k}(\eta')}\right|$.

## Solution Reasoning

The dominant singularity is a simple zero of $F=\omega_k^2$, not a pole of $\omega_k$ itself. Near a simple zero, $F\sim F'(\tilde\eta)(\eta-\tilde\eta)$, so $\omega\sim \sqrt{F'(\tilde\eta)}(\eta-\tilde\eta)^{1/2}$. Since $\omega'/(2\omega)=F'/(4F)$, the singular part is universal and equals $1/[4(\eta-\tilde\eta)]$. For the selected lower-half-plane turning point, the denominator factor is $1-a_eH_I(\tilde\eta-\eta_e)=i ma_e/k$, which gives $F'(\tilde\eta)=+2i k^3H_I/m$. The local phase is obtained by integrating the square-root behavior of $\omega$, giving the $z^{3/2}$ exponent. Changing variables to $u=-(4i/3)\sqrt{F'(\tilde\eta)}z^{3/2}$ converts the singular measure as $(1/4)dz/z=(1/6)du/u$. The full Hankel/Stokes contour gives a magnitude $2\pi$ for $\int_{\mathcal H}e^u du/u$, hence the prefactor is $2\pi/6=\pi/3$.

## Result

Let
$$F(\eta)\equiv \omega_k^2(\eta)=k^2+m^2a^2(\eta).$$
On the dominant inflationary branch,
$$a(\eta)=\frac{a_e}{1-a_eH_I(\eta-\eta_e)},$$
so
$$F(\eta)=k^2+\frac{m^2a_e^2}{[1-a_eH_I(\eta-\eta_e)]^2}.$$
The selected lower-half-plane turning point is
$$\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I},$$
for which
$$1-a_eH_I(\tilde\eta-\eta_e)=i\frac{ma_e}{k}.$$
Therefore
$$F'(\eta)=\frac{2a_eH_I m^2a_e^2}{[1-a_eH_I(\eta-\eta_e)]^3},$$
and hence
$$F'(\tilde\eta)=+2i\frac{k^3H_I}{m}.$$
Writing
$$z\equiv \eta-\tilde\eta,$$
the local expansion near the simple turning point is
$$F(\eta)=F'(\tilde\eta)z+O(z^2),$$
so
$$\omega_k(\eta)=\sqrt{F'(\tilde\eta)}\,z^{1/2}\left[1+O(z)\right].$$
Since
$$\frac{\omega_k'}{2\omega_k}=\frac{F'}{4F},$$
one obtains the universal simple-turning-point behavior
$$\boxed{\frac{\omega_k'(\eta)}{2\omega_k(\eta)}=\frac{1}{4(\eta-\tilde\eta)}+O(1).}$$
The phase also has the local form
$$-2i\int_{\eta_e}^{\eta}\omega_k(\eta')d\eta'=-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'-\frac{4i}{3}\sqrt{F'(\tilde\eta)}\,z^{3/2}+O(z^{5/2}).$$
Introduce the steepest-descent variable
$$u=-\frac{4i}{3}\sqrt{F'(\tilde\eta)}\,z^{3/2}.$$
Then
$$\frac14\frac{dz}{z}=\frac16\frac{du}{u}.$$
Thus the local contour contribution is
$$\int d\eta\frac{\omega_k'}{2\omega_k}e^{-2i\int_{\eta_e}^{\eta}\omega_k d\eta'}
\simeq e^{-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta'}\frac16\int_{\mathcal H}\frac{du}{u}e^u,$$
where $\mathcal H$ is the appropriate Hankel/Stokes contour around the simple turning point. With the standard full Hankel prescription,
$$\left|\frac16\int_{\mathcal H}\frac{du}{u}e^u\right|=\frac{\pi}{3}.$$
Therefore the one-pole prefactor entering the Bogoliubov coefficient is
$$\boxed{|\beta(k)|_{\text{1-pole}}\simeq \frac{\pi}{3}\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'\right]\right|.}$$
Equivalently,
$$\boxed{|\beta(k)|_{\text{1-pole}}\simeq \frac{\pi}{3}\exp\left[2\,\operatorname{Im}\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'\right],}$$
with the sign of the imaginary part fixed by the chosen steepest-descent contour so that the physical contribution is exponentially suppressed.

## Physical Interpretation

Let
$$F(\eta)\equiv \omega_k^2(\eta)=k^2+m^2a^2(\eta).$$
On the dominant inflationary branch,
$$a(\eta)=\frac{a_e}{1-a_eH_I(\eta-\eta_e)},$$
so
$$F(\eta)=k^2+\frac{m^2a_e^2}{[1-a_eH_I(\eta-\eta_e)]^2}.$$
The selected lower-half-plane turning point is
$$\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I},$$
for which
$$1-a_eH_I(\tilde\eta-\eta_e)=i\frac{ma_e}{k}.$$
Therefore
$$F'(\eta)=\frac{2a_eH_I m^2a_e^2}{[1-a_eH_I(\eta-\eta_e)]^3},$$
and hence
$$F'(\tilde\eta)=+2i\frac{k^3H_I}{m}.$$
Writing
$$z\equiv \eta-\tilde\eta,$$
the local expansion near the simple turning point is
$$F(\eta)=F'(\tilde\eta)z+O(z^2),$$
so
$$\omega_k(\eta)=\sqrt{F'(\tilde\eta)}\,z^{1/2}\left[1+O(z)\right].$$
Since
$$\frac{\omega_k'}{2\omega_k}=\frac{F'}{4F},$$
one obtains the universal simple-turning-point behavior
$$\boxed{\frac{\omega_k'(\eta)}{2\omega_k(\eta)}=\frac{1}{4(\eta-\tilde\eta)}+O(1).}$$
The phase also has the local form
$$-2i\int_{\eta_e}^{\eta}\omega_k(\eta')d\eta'=-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'-\frac{4i}{3}\sqrt{F'(\tilde\eta)}\,z^{3/2}+O(z^{5/2}).$$
Introduce the steepest-descent variable
$$u=-\frac{4i}{3}\sqrt{F'(\tilde\eta)}\,z^{3/2}.$$
Then
$$\frac14\frac{dz}{z}=\frac16\frac{du}{u}.$$
Thus the local contour contribution is
$$\int d\eta\frac{\omega_k'}{2\omega_k}e^{-2i\int_{\eta_e}^{\eta}\omega_k d\eta'}
\simeq e^{-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta'}\frac16\int_{\mathcal H}\frac{du}{u}e^u,$$
where $\mathcal H$ is the appropriate Hankel/Stokes contour around the simple turning point. With the standard full Hankel prescription,
$$\left|\frac16\int_{\mathcal H}\frac{du}{u}e^u\right|=\frac{\pi}{3}.$$
Therefore the one-pole prefactor entering the Bogoliubov coefficient is
$$\boxed{|\beta(k)|_{\text{1-pole}}\simeq \frac{\pi}{3}\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'\right]\right|.}$$
Equivalently,
$$\boxed{|\beta(k)|_{\text{1-pole}}\simeq \frac{\pi}{3}\exp\left[2\,\operatorname{Im}\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'\right],}$$
with the sign of the imaginary part fixed by the chosen steepest-descent contour so that the physical contribution is exponentially suppressed.

**Consistency check:** passed
