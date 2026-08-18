# Step 4 — Evaluate the complex WKB action $-2i\int_{\eta_{e}}^{\tilde{\eta}}\omega_{k}(\eta')d\eta'$ along the steepest-descent contour, retaining the leading contribution in $k/(a_{e}H_{I})\rightarrow\infty$ that controls $|\beta(k)|$.

## Solution Reasoning

The dominant singularity is the lower-half-plane turning point of the inflationary branch, because in the limit $k/(a_eH_I)\to\infty$ it lies parametrically closer to the real axis than the post-transition turning points. The conformal-time pole variable $y=1-a_eH_I(\eta-\eta_e)$ converts the integral into an elementary contour integral. The endpoint $y=i\mu$ is precisely where $\omega_k^2=0$. The imaginary part of the action arises from the logarithm evaluated at $y=i\mu$, giving $\ln i=i\pi/2$ on the steepest-descent branch. Multiplying by $-2i$ converts this imaginary part into the real exponential suppression $-\pi m/H_I$. The remaining real part of the WKB integral gives only a rapidly oscillatory phase, whose leading term is $-2ik/(a_eH_I)$ and which does not affect $|\beta(k)|$.

## Result

Let $A\equiv a_eH_I$ and $\mu\equiv ma_e/k\ll 1$. On the dominant inflationary branch,
$$
a(\eta)=\frac{a_e}{1-A(\eta-\eta_e)},
$$
so introduce
$$
y\equiv 1-A(\eta-\eta_e),\qquad d\eta=-\frac{dy}{A}.
$$
At the initial point $\eta=\eta_e$, $y=1$, while at the dominant lower-half-plane turning point
$$
\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I},
$$
one has
$$
\tilde y=1-A(\tilde\eta-\eta_e)=i\mu.
$$
The WKB integral is therefore
$$
I\equiv \int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'
=-\frac{k}{A}\int_1^{i\mu}dy\,\frac{\sqrt{y^2+\mu^2}}{y}.
$$
Using
$$
\int dy\,\frac{\sqrt{y^2+\mu^2}}{y}
=\sqrt{y^2+\mu^2}+\mu\ln\left(\frac{y}{\mu+\sqrt{y^2+\mu^2}}\right),
$$
and taking the branch appropriate to the steepest-descent contour ending at $y=i\mu$, where $\sqrt{y^2+\mu^2}=0$, gives
$$
I=\frac{k}{a_eH_I}\left[\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)-i\frac{\pi\mu}{2}\right].
$$
Thus
$$
-2iI
=-2i\frac{k}{a_eH_I}\left[\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)\right]
-\frac{\pi m}{H_I}.
$$
In the large-momentum limit $\mu=ma_e/k\to0$,
$$
\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)
=1+O(\mu^2),
$$
so the leading complex WKB action is
$$
\boxed{
-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'
= -2i\frac{k}{a_eH_I}-\frac{\pi m}{H_I}
+O\left(\frac{m^2a_e}{kH_I}\right)
}.
$$
Therefore the factor controlling the magnitude is
$$
\boxed{
\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta\right]\right|
\simeq e^{-\pi m/H_I}
}.
$$

## Physical Interpretation

Let $A\equiv a_eH_I$ and $\mu\equiv ma_e/k\ll 1$. On the dominant inflationary branch,
$$
a(\eta)=\frac{a_e}{1-A(\eta-\eta_e)},
$$
so introduce
$$
y\equiv 1-A(\eta-\eta_e),\qquad d\eta=-\frac{dy}{A}.
$$
At the initial point $\eta=\eta_e$, $y=1$, while at the dominant lower-half-plane turning point
$$
\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I},
$$
one has
$$
\tilde y=1-A(\tilde\eta-\eta_e)=i\mu.
$$
The WKB integral is therefore
$$
I\equiv \int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'
=-\frac{k}{A}\int_1^{i\mu}dy\,\frac{\sqrt{y^2+\mu^2}}{y}.
$$
Using
$$
\int dy\,\frac{\sqrt{y^2+\mu^2}}{y}
=\sqrt{y^2+\mu^2}+\mu\ln\left(\frac{y}{\mu+\sqrt{y^2+\mu^2}}\right),
$$
and taking the branch appropriate to the steepest-descent contour ending at $y=i\mu$, where $\sqrt{y^2+\mu^2}=0$, gives
$$
I=\frac{k}{a_eH_I}\left[\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)-i\frac{\pi\mu}{2}\right].
$$
Thus
$$
-2iI
=-2i\frac{k}{a_eH_I}\left[\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)\right]
-\frac{\pi m}{H_I}.
$$
In the large-momentum limit $\mu=ma_e/k\to0$,
$$
\sqrt{1+\mu^2}-\mu\ln\left(\mu+\sqrt{1+\mu^2}\right)
=1+O(\mu^2),
$$
so the leading complex WKB action is
$$
\boxed{
-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta')d\eta'
= -2i\frac{k}{a_eH_I}-\frac{\pi m}{H_I}
+O\left(\frac{m^2a_e}{kH_I}\right)
}.
$$
Therefore the factor controlling the magnitude is
$$
\boxed{
\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta\right]\right|
\simeq e^{-\pi m/H_I}
}.
$$

**Consistency check:** passed
