# Analyse Step 1 Iteration 1

**Description:** Integrate Eq. $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$; choose the convenient origin/branch so that the post-transition scale factor $a(\eta)$ is explicitly available for complex $\eta$ and has the analytic structure needed by $\omega_k(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The relevant information is the scale-factor differential equation in cosmic proper time, the boundary condition $a(t_e)=a_e$, the relation $dt=a(\eta)d\eta$, and the need to choose a conformal-time origin/branch convenient for analytic continuation into complex $\eta$. No additional prior result is needed.

## Critical Rubrics

A correct answer must: (i) integrate the scale-factor equation separately for $t<t_e$ and $t>t_e$ using $a(t_e)=a_e$; (ii) correctly use $dt=a\,d\eta$; (iii) choose a clear conformal-time origin, preferably $\eta_e=0$; (iv) derive the post-transition expression $a(\eta)=a_e[1+(a_eH_I/2)(\eta-\eta_e)]^2$; (v) specify the branch choice $u^{1/3}=1$ at the transition; and (vi) identify the resulting analytic structure of $\omega_k(\eta)$ in complex conformal time.

## Candidate Result

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
\eta=\int_{t_e}^{t}\frac{dt'}{a(t')}=rac{2}{a_eH_I}\left(u^{1/3}-1\right).
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

## Reasoning

The differential equation is piecewise because of the step functions. For $t<t_e$, $d\ln a/dt=H_I$, so integration relative to $t_e$ gives $a=a_e e^{H_I(t-t_e)}$. For $t>t_e$, integrating $d\ln a/dt=H_I/[1+\frac32H_I(t-t_e)]$ gives $\ln(a/a_e)=\frac23\ln[1+\frac32H_I(t-t_e)]$, hence the matter-like power law $a=a_e[1+\frac32H_I(t-t_e)]^{2/3}$. Conformal time follows from $d\eta=dt/a(t)$. In the post-transition era the substitution $u=1+\frac32H_I(t-t_e)$ makes the integral elementary and produces $\eta-\eta_e=2(a_eH_I)^{-1}(u^{1/3}-1)$. Choosing the branch $u^{1/3}=1$ at $t=t_e$ removes the fractional-power ambiguity in conformal time and makes $a(\eta)$ a simple quadratic polynomial. This is precisely the form needed to continue $\omega_k(\eta)=\sqrt{k^2+m^2a^2(\eta)}$ into complex $\eta$ and locate its square-root singularities.
