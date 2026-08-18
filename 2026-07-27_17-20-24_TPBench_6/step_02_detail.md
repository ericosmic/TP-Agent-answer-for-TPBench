# Step 2 — Using the analytic $a(\eta)$ from Step 1, determine the singularities of $\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}$ relevant to Eq. $|\beta(k)|\approx\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{e}}^{\eta}d\eta'\omega_{k}(\eta')}\right|$; impose $\omega_k(\tilde{\eta})=0$ and select the dominant pole/turning point $\tilde{\eta}$ with $\Re\tilde{\eta}>0$ and minimal positive imaginary contribution in the large-$k/(a_eH_I)$ limit.

## Solution Reasoning

The steepest-descent singularities relevant to the one-pole approximation are determined by zeros of the adiabatic frequency $\omega_k$, because the prefactor can be written as $\omega_k'/(2\omega_k)=(1/4)(\omega_k^2)'/\omega_k^2$. With the Step 1 post-transition analytic scale factor, $a(\eta)$ is a quadratic polynomial in $z=1+\frac{a_eH_I}{2}(\eta-\eta_e)$, so $a^2=a_e^2z^4$. The equation $\omega_k^2=0$ is therefore the algebraic equation $z^4=-(k/(ma_e))^2$, giving four complex turning points separated by phases $\pi/2$. In the large-$k$ limit, their real and imaginary parts are controlled by $\rho=(k/(ma_e))^{1/2}$. The root with phase $\pi/4$ lies in the first quadrant after the real offset $-2/(a_eH_I)$ and has $\Re\eta>0$ for sufficiently large $\rho$. It is the only upper-half-plane root with positive real part; hence it is the dominant pole/turning point requested for the later one-pole approximation.

## Result

Using the post-transition analytic continuation from Step 1,
$$
a(\eta)=a_e\left[1+\frac{a_eH_I}{2}(\eta-\eta_e)\right]^2,
$$
write
$$
z(\eta)\equiv 1+\frac{a_eH_I}{2}(\eta-\eta_e).
$$
Then
$$
\omega_k^2(\eta)=k^2+m^2a_e^2 z^4.
$$
The singularities of $\omega_k'/(2\omega_k)$ occur at the zeros of $\omega_k^2$, because
$$
\frac{\omega_k'}{2\omega_k}=\frac{1}{4}\frac{(\omega_k^2)'}{\omega_k^2}.
$$
Thus the relevant turning points satisfy
$$
k^2+m^2a_e^2z^4=0,
$$
or
$$
z^4=-\left(\frac{k}{ma_e}\right)^2.
$$
Hence
$$
z_n=\left(\frac{k}{ma_e}\right)^{1/2}\exp\left[i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right],\qquad n=0,1,2,3,
$$
and therefore
$$
\eta_n=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}\exp\left(i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right)-1\right].
$$
These are square-root branch points of $\omega_k$ and appear as simple poles of $\omega_k'/(2\omega_k)$; locally,
$$
\frac{\omega_k'}{2\omega_k}\sim \frac{1}{4(\eta-\eta_n)}.
$$
Let
$$
\rho\equiv \left(\frac{k}{ma_e}\right)^{1/2}.
$$
For $n=0$,
$$
\eta_0=\eta_e+\frac{2}{a_eH_I}\left(\frac{\rho}{\sqrt2}-1+i\frac{\rho}{\sqrt2}\right),
$$
so in the large-$k/(a_eH_I)$ regime it has $\Re\eta_0>0$ and positive imaginary part. The $n=1$ root is in the upper half-plane but has negative real part, while $n=2$ and $n=3$ lie in the lower half-plane, with $n=3$ being the complex conjugate of $n=0$ up to the same real offset. Therefore, the dominant upper-half-plane turning point with $\Re\tilde\eta>0$ and minimal positive imaginary contribution is
$$
\boxed{\tilde\eta=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{i\pi/4}-1\right]}.
$$
If one sets $\eta_e=0$, this becomes
$$
\boxed{\tilde\eta=\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{i\pi/4}-1\right]}.
$$

**Consistency check:** passed
