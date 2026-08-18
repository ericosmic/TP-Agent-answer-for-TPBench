## Execution Step Results

### Step 1: Integrate Eq. $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$; choose the convenient origin/branch so that the post-transition scale factor $a(\eta)$ is explicitly available for complex $\eta$ and has the analytic structure needed by $\omega_k(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$.

**Reasoning:**
The differential equation is piecewise because of the step functions. For $t<t_e$, $d\ln a/dt=H_I$, so integration relative to $t_e$ gives $a=a_e e^{H_I(t-t_e)}$. For $t>t_e$, integrating $d\ln a/dt=H_I/[1+\frac32H_I(t-t_e)]$ gives $\ln(a/a_e)=\frac23\ln[1+\frac32H_I(t-t_e)]$, hence the matter-like power law $a=a_e[1+\frac32H_I(t-t_e)]^{2/3}$. Conformal time follows from $d\eta=dt/a(t)$. In the post-transition era the substitution $u=1+\frac32H_I(t-t_e)$ makes the integral elementary and produces $\eta-\eta_e=2(a_eH_I)^{-1}(u^{1/3}-1)$. Choosing the branch $u^{1/3}=1$ at $t=t_e$ removes the fractional-power ambiguity in conformal time and makes $a(\eta)$ a simple quadratic polynomial. This is precisely the form needed to continue $\omega_k(\eta)=\sqrt{k^2+m^2a^2(\eta)}$ into complex $\eta$ and locate its square-root singularities.

**Result:**
For $t<t_e$ the Hubble rate is constant, while for $t>t_e$ it is $H_I/[1+\frac32H_I(t-t_e)]$. Integrating with $a(t_e)=a_e$ gives

$$
a(t)=
\begin{cases}
a_e\exp\!\left[H_I(t-t_e)\right], & t\le t_e,\\[4pt]
a_e\left[1+\dfrac32H_I(t-t_e)\right]^{2/3}, & t\ge t_e.
\end{cases}
$$

Now use $dt=a(\eta)d\eta$ and choose the conformal-time origin so that $\eta_e=0$. For the pre-transition de Sitter branch,

$$
\eta=\int_{t_e}^{t}\frac{dt'}{a(t')}=\frac{1}{a_eH_I}\left(1-e^{-H_I(t-t_e)}\right),
$$
so

$$
e^{-H_I(t-t_e)}=1-a_eH_I\eta,
\qquad
\boxed{a(\eta)=\frac{a_e}{1-a_eH_I\eta}},\qquad \eta\le 0.
$$

For the post-transition branch define

$$
u\equiv 1+\frac32H_I(t-t_e).
$$

Then $a=a_eu^{2/3}$ and

$$
\eta=\int_{t_e}^{t}\frac{dt'}{a(t')}=
rac{2}{a_eH_I}\left(u^{1/3}-1\right).
$$

Choosing the branch with $u^{1/3}=1$ at $\eta=0$ gives

$$
u^{1/3}=1+\frac{a_eH_I}{2}\eta,
$$
therefore

$$
\boxed{a(\eta)=a_e\left(1+\frac{a_eH_I}{2}\eta\right)^2},\qquad \eta\ge 0.
$$

Equivalently, without setting $\eta_e=0$,

$$
\boxed{a(\eta)=a_e\left[1+\frac{a_eH_I}{2}(\eta-\eta_e)\right]^2},\qquad \eta\ge\eta_e.
$$

This is the convenient post-transition analytic continuation: $a(\eta)$ is an entire quadratic polynomial in complex $\eta$, with a double zero at

$$
\eta_0=\eta_e-\frac{2}{a_eH_I}.
$$

Thus the relevant post-transition frequency is

$$
\omega_k(\eta)=\sqrt{k^2+m^2a_e^2\left[1+\frac{a_eH_I}{2}(\eta-\eta_e)\right]^4},
$$
with the square-root branch chosen so that $\omega_k>0$ on the real post-transition contour. The singularities relevant for the later one-pole approximation are the complex zeros of $\omega_k^2$, namely

$$
1+\frac{a_eH_I}{2}(\eta-\eta_e)
=\left(\frac{k}{ma_e}\right)^{1/2}
\exp\left[i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right],
\qquad n=0,1,2,3.
$$

Hence

$$
\eta_n=\eta_e+\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}
\exp\left(i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right)-1\right].
$$

These branch points/poles of $\omega_k'/2\omega_k$ provide the analytic structure needed for the later steepest-descent one-pole estimate.

### Step 2: Using the analytic $a(\eta)$ from Step 1, determine the singularities of $\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}$ relevant to Eq. $|\beta(k)|\approx\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{e}}^{\eta}d\eta'\omega_{k}(\eta')}\right|$; impose $\omega_k(\tilde{\eta})=0$ and select the dominant pole/turning point $\tilde{\eta}$ with $\Re\tilde{\eta}>0$ and minimal positive imaginary contribution in the large-$k/(a_eH_I)$ limit.

**Reasoning:**
The steepest-descent singularities relevant to the one-pole approximation are determined by zeros of the adiabatic frequency $\omega_k$, because the prefactor can be written as $\omega_k'/(2\omega_k)=(1/4)(\omega_k^2)'/\omega_k^2$. With the Step 1 post-transition analytic scale factor, $a(\eta)$ is a quadratic polynomial in $z=1+\frac{a_eH_I}{2}(\eta-\eta_e)$, so $a^2=a_e^2z^4$. The equation $\omega_k^2=0$ is therefore the algebraic equation $z^4=-(k/(ma_e))^2$, giving four complex turning points separated by phases $\pi/2$. In the large-$k$ limit, their real and imaginary parts are controlled by $\rho=(k/(ma_e))^{1/2}$. The root with phase $\pi/4$ lies in the first quadrant after the real offset $-2/(a_eH_I)$ and has $\Re\eta>0$ for sufficiently large $\rho$. It is the only upper-half-plane root with positive real part; hence it is the dominant pole/turning point requested for the later one-pole approximation.

**Result:**
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

### Step 3: Expand $\omega_k(\eta)$ locally around the selected $\tilde{\eta}$ and replace $\frac{\omega_k'}{2\omega_k}$ by its leading one-pole form; deform the real-$\eta$ contour to the steepest-descent contour through $\tilde{\eta}$, retaining only the residue/phase contribution from this pole and discarding subdominant poles according to Step 2.

**Reasoning:**
The zero of $\omega_k^2$ at $\tilde\eta$ is simple because $Q'(\tilde\eta)
eq0$. Therefore $\omega_k$ has a square-root branch point, $\omega_k\sim[Q'(\tilde\eta)]^{1/2}(\eta-\tilde\eta)^{1/2}$. Since $\omega_k'/(2\omega_k)=\frac14 Q'/Q$, this branch point appears in the logarithmic derivative as a simple pole with residue $1/4$. In the steepest-descent deformation the fast exponential is evaluated at the turning point to leading one-pole order, while the local $(\eta-\tilde\eta)^{3/2}$ correction controls the steepest direction but does not change the residue. All other poles/turning points are farther away or lie on subdominant contours according to Step 2, so they are discarded. The remaining contribution is thus the residue of the pole multiplied by the WKB phase evaluated at $\tilde\eta$, up to an orientation/Stokes sign irrelevant to $|\beta|$.

**Result:**
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

### Step 4: Evaluate the WKB phase integral $S(k)=\int_{\eta_e}^{\tilde{\eta}}d\eta\,\omega_k(\eta)$ using the large-$k/(a_eH_I)$ expansion with $0<m\lesssim H_I$, keeping the leading non-analytic/exponential contribution that controls $|\beta(k)|$ and retaining only prefactors that survive the requested approximation accuracy.

**Reasoning:**
The relevant phase integral lies entirely on the post-transition analytic continuation because the dominant turning point has positive real part. The natural variable $z=1+(a_eH_I/2)(\eta-\eta_e)$ maps the lower endpoint to $z=1$ and the turning point to $z=\rho e^{i\pi/4}$, where $\rho=(k/(ma_e))^{1/2}$. After the rescaling $z=\rho s$, the large-$k/(a_eH_I)$, $0<m\lesssim H_I$ limit corresponds to $\rho\gg1$ for the nonanalytic turning-point contribution. The integral from $0$ to $e^{i\pi/4}$ gives the complex nonanalytic contribution proportional to $k\rho/(a_eH_I)\sim k^{3/2}m^{-1/2}$, while the correction from replacing the lower limit $1/\rho$ by $0$ is real at leading order and hence does not contribute to the magnitude of $\beta(k)$. Evaluating the universal constant by the beta function gives $C=(1/4)B(1/4,3/2)=\sqrt\pi\Gamma(1/4)/(6\Gamma(3/4))$. Therefore only the imaginary part of the $e^{i\pi/4}C$ term controls the exponential suppression in the Bogoliubov coefficient.

**Result:**
Introduce
$$z=1+\frac{a_eH_I}{2}(\eta-\eta_e),\qquad \rho=\left(\frac{k}{ma_e}\right)^{1/2}.$$
Then $z(\eta_e)=1$ and the dominant turning point has
$$\tilde z=z(\tilde\eta)=\rho e^{i\pi/4}.$$
Since
$$\omega_k(\eta)=\sqrt{k^2+m^2a_e^2z^4}=k\sqrt{1+\frac{z^4}{\rho^4}},\qquad d\eta=\frac{2\,dz}{a_eH_I},$$
the WKB phase is
$$S(k)=\frac{2k}{a_eH_I}\int_1^{\rho e^{i\pi/4}}dz\,\sqrt{1+\frac{z^4}{\rho^4}}.$$
Rescale $z=\rho s$:
$$S(k)=\frac{2k\rho}{a_eH_I}\int_{1/\rho}^{e^{i\pi/4}}ds\,\sqrt{1+s^4}.$$
For $\rho\gg1$, the lower limit may be expanded as
$$\int_{1/\rho}^{e^{i\pi/4}}ds\sqrt{1+s^4}=\int_0^{e^{i\pi/4}}ds\sqrt{1+s^4}-\int_0^{1/\rho}ds\sqrt{1+s^4}.$$
Along $s=e^{i\pi/4}y$, $0\le y\le1$, one has $s^4=-y^4$ and therefore
$$\int_0^{e^{i\pi/4}}ds\sqrt{1+s^4}=e^{i\pi/4}\int_0^1dy\sqrt{1-y^4}.$$
The constant integral is
$$C\equiv\int_0^1dy\sqrt{1-y^4}=\frac14B\!\left(\frac14,\frac32\right)=\frac{\sqrt\pi\,\Gamma(1/4)}{6\Gamma(3/4)}.$$
The subtracted lower-limit integral is real,
$$\int_0^{1/\rho}ds\sqrt{1+s^4}=\frac1\rho+O(\rho^{-5}),$$
so it contributes only a real phase at leading order. Thus
$$\boxed{S(k)=\frac{2k\rho}{a_eH_I}C e^{i\pi/4}-\frac{2k}{a_eH_I}+O\!\left(\frac{k}{a_eH_I}\rho^{-4}\right)}.$$
Equivalently,
$$\boxed{S(k)=\frac{\sqrt{2\pi}\,\Gamma(1/4)}{6\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}(1+i)-\frac{2k}{a_eH_I}+\cdots}.$$
The term $-2k/(a_eH_I)$ is real and affects only the oscillatory phase of $\beta(k)$, not its magnitude. The leading imaginary part controlling the exponential magnitude is therefore
$$\boxed{\operatorname{Im}S(k)=\frac{\sqrt{2\pi}\,\Gamma(1/4)}{6\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}+\cdots}.$$
Thus the one-pole exponential factor is governed by
$$\boxed{2|\operatorname{Im}S(k)|=\frac{\sqrt{2\pi}\,\Gamma(1/4)}{3\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}+\cdots}.$$
With the physical steepest-descent/Stokes prescription this enters $|\beta(k)|$ as an exponential suppression, i.e. $|\beta(k)|\propto\exp[-2|\operatorname{Im}S(k)|]$, up to the one-pole residue prefactor fixed in the previous step.

### Step 5: Assemble the asymptotic one-pole result for $|\beta(k)|$ from the pole factor of Step 3 and the imaginary part of $S(k)$ from Step 4, and express the answer explicitly in terms of $k$, $a_e$, $H_I$, and $m$, together with the validity conditions $k/(a_eH_I)\to\infty$ and $0<m\lesssim H_I$.

**Reasoning:**
Step 3 reduces the original oscillatory integral to a residue contribution at the dominant pole/turning point: $\beta\simeq (i\pi/2)e^{-2iS}$ up to an irrelevant sign. Taking the magnitude gives a factor $\pi/2$ times the exponential governed by the imaginary part of $S$. The physically relevant steepest-descent contour gives suppression, hence $\exp[-2|\operatorname{Im}S|]$ rather than exponential growth. Step 4 supplies $2|\operatorname{Im}S|$ explicitly as $[\sqrt{2\pi}\Gamma(1/4)/(3\Gamma(3/4))][k/(a_eH_I)](k/(ma_e))^{1/2}$ at leading order. Combining these two pieces directly yields the boxed formula.

**Result:**
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

---
