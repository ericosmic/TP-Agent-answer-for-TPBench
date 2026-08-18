# Step 2 — Insert $a(\eta)$ into $\omega_{k}(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$ and locate the singularities of $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ from $\omega_{k}^{2}(\eta)=0$, selecting the dominant pole or turning point $\tilde{\eta}$ with $\Re\tilde{\eta}>0$ for $k/(a_{e}H_{I})\rightarrow\infty$.

## Solution Reasoning

The singularities of $\omega_k'/(2\omega_k)$ relevant for particle production are WKB turning points where $\omega_k^2=0$. Substituting the meromorphic inflationary branch gives a quadratic equation in $1-A\Delta\eta$, whose two solutions sit just above and below the pole of the scale factor. Their imaginary displacement from the real axis is $m/(kH_I)$, which tends to zero as $k\to\infty$. Substituting the post-transition polynomial branch gives a quartic equation. Its four roots scale as $(k/(ma_e))^{1/2}/(a_eH_I)$ away from the transition point, so they are much farther from the real axis in the large-$k$ limit. Since steepest-descent contributions are dominated by the nearest complex singularity, the inflationary-branch root near $\eta_e+1/(a_eH_I)$ dominates. With the exponential convention $e^{-2i\int\omega}$, the lower-half-plane root gives the exponentially suppressed physical contribution, so $\tilde\eta=\eta_e+1/(a_eH_I)-i m/(kH_I)$.

## Result

Let $A\equiv a_eH_I$ and $\Delta\eta\equiv\eta-\eta_e$. On the inflationary analytic branch,
$$
a_-(\eta)=\frac{a_e}{1-A\Delta\eta},
$$
so
$$
\omega_{k,-}^2(\eta)=k^2+\frac{m^2a_e^2}{\left[1-A(\eta-\eta_e)\right]^2}.
$$
The turning points are determined by $\omega_{k,-}^2=0$, hence
$$
\left[1-A(\eta-\eta_e)\right]^2=-\frac{m^2a_e^2}{k^2},
$$
which gives
$$
\eta_{\pm}^{(-)}=\eta_e+\frac{1}{a_eH_I}\left(1\mp i\frac{ma_e}{k}\right)
=\eta_e+\frac{1}{a_eH_I}\mp i\frac{m}{kH_I}.
$$
These are simple zeros of $\omega_k^2$, and therefore $\omega_k'/(2\omega_k)$ has simple pole-type WKB singularities there.

On the post-transition branch,
$$
a_+(\eta)=a_e\left[1+\frac{A}{2}(\eta-\eta_e)\right]^2,
$$
so
$$
\omega_{k,+}^2(\eta)=k^2+m^2a_e^2\left[1+\frac{A}{2}(\eta-\eta_e)\right]^4.
$$
The zeros obey
$$
\left[1+\frac{A}{2}(\eta-\eta_e)\right]^4=-\frac{k^2}{m^2a_e^2}.
$$
Thus
$$
\eta_n^{(+)}=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{i(\pi/4+n\pi/2)}-1\right],\qquad n=0,1,2,3.
$$
For $k/(a_eH_I)\to\infty$ with $0<m\lesssim H_I$, these post-transition turning points lie parametrically far from the real axis, with imaginary parts of order
$$
|\Im\eta_n^{(+)}|\sim \frac{1}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2},
$$
whereas the inflationary-branch turning points lie exponentially closer to the real axis, at distance
$$
|\Im\eta_{\pm}^{(-)}|=\frac{m}{kH_I}.
$$
Therefore the dominant one-pole/turning-point contribution in the large-$k/(a_eH_I)$ limit comes from the inflationary-branch turning point near the pole of $a_-(\eta)$ at $\eta=\eta_e+1/(a_eH_I)$.

For the phase convention in
$$
\exp\left[-2i\int^{\eta}\omega_k(\eta')d\eta'\right],
$$
the steepest-descent contour relevant for a suppressed contribution is taken into the lower half-plane. Hence the dominant turning point is
$$
\boxed{\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I}}
$$
with
$$
\Re\tilde\eta=\eta_e+\frac{1}{a_eH_I}>0
$$
for the usual choice of origin, or more generally whenever the transition point is chosen so that this real part is positive.

## Physical Interpretation

Let $A\equiv a_eH_I$ and $\Delta\eta\equiv\eta-\eta_e$. On the inflationary analytic branch,
$$
a_-(\eta)=\frac{a_e}{1-A\Delta\eta},
$$
so
$$
\omega_{k,-}^2(\eta)=k^2+\frac{m^2a_e^2}{\left[1-A(\eta-\eta_e)\right]^2}.
$$
The turning points are determined by $\omega_{k,-}^2=0$, hence
$$
\left[1-A(\eta-\eta_e)\right]^2=-\frac{m^2a_e^2}{k^2},
$$
which gives
$$
\eta_{\pm}^{(-)}=\eta_e+\frac{1}{a_eH_I}\left(1\mp i\frac{ma_e}{k}\right)
=\eta_e+\frac{1}{a_eH_I}\mp i\frac{m}{kH_I}.
$$
These are simple zeros of $\omega_k^2$, and therefore $\omega_k'/(2\omega_k)$ has simple pole-type WKB singularities there.

On the post-transition branch,
$$
a_+(\eta)=a_e\left[1+\frac{A}{2}(\eta-\eta_e)\right]^2,
$$
so
$$
\omega_{k,+}^2(\eta)=k^2+m^2a_e^2\left[1+\frac{A}{2}(\eta-\eta_e)\right]^4.
$$
The zeros obey
$$
\left[1+\frac{A}{2}(\eta-\eta_e)\right]^4=-\frac{k^2}{m^2a_e^2}.
$$
Thus
$$
\eta_n^{(+)}=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{i(\pi/4+n\pi/2)}-1\right],\qquad n=0,1,2,3.
$$
For $k/(a_eH_I)\to\infty$ with $0<m\lesssim H_I$, these post-transition turning points lie parametrically far from the real axis, with imaginary parts of order
$$
|\Im\eta_n^{(+)}|\sim \frac{1}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2},
$$
whereas the inflationary-branch turning points lie exponentially closer to the real axis, at distance
$$
|\Im\eta_{\pm}^{(-)}|=\frac{m}{kH_I}.
$$
Therefore the dominant one-pole/turning-point contribution in the large-$k/(a_eH_I)$ limit comes from the inflationary-branch turning point near the pole of $a_-(\eta)$ at $\eta=\eta_e+1/(a_eH_I)$.

For the phase convention in
$$
\exp\left[-2i\int^{\eta}\omega_k(\eta')d\eta'\right],
$$
the steepest-descent contour relevant for a suppressed contribution is taken into the lower half-plane. Hence the dominant turning point is
$$
\boxed{\tilde\eta=\eta_e+\frac{1}{a_eH_I}-i\frac{m}{kH_I}}
$$
with
$$
\Re\tilde\eta=\eta_e+\frac{1}{a_eH_I}>0
$$
for the usual choice of origin, or more generally whenever the transition point is chosen so that this real part is positive.

**Consistency check:** passed
