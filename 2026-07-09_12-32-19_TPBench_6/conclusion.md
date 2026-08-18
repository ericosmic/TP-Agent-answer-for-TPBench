## Solution Plan
  1. Derive the physical scale factor from $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$, choosing $\eta_{e}=0$ if convenient. Track continuity of $a$ and $a'$ at $t=t_{e}$ and identify the nonanalyticity in higher derivatives caused by the sudden transition.
  2. Before applying the one-pole contour estimate, impose a UV-consistent prescription: verify whether the sharp $\Theta$ transition produces a power-law high-$k$ tail in $|\beta(k)|$ from discontinuities of derivatives of $a(\eta)$, and either include the corresponding boundary contribution or state that a smoothed/adiabatic transition is assumed so that the one-pole exponential result is meaningful and avoids a UV catastrophe in $\int d^{3}k\,|\beta(k)|^{2}$ or $\int d^{3}k\,\omega_{k}|\beta(k)|^{2}$.
  3. Insert the relevant analytic branch of $a(\eta)$ into $\omega_{k}(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$ and find the dominant singularity $\tilde{\eta}$ of $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ from $\omega_{k}^{2}(\tilde{\eta})=0$, selecting the pole or turning point with $\Re\tilde{\eta}>0$ that gives the smallest positive suppression in the limit $k/(a_{e}H_{I})\rightarrow\infty$.
  4. Evaluate the local one-pole contribution by expanding $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ near $\tilde{\eta}$ and combine it with the steepest-descent phase $\exp\left[-2i\int_{\eta_{e}}^{\tilde{\eta}}d\eta'\,\omega_{k}(\eta')\right]$, retaining the leading magnitude and discarding irrelevant phases.
  5. Compare the one-pole exponential contribution with any UV boundary or sudden-transition contribution found earlier; report the dominant UV-safe expression for $|\beta(k)|$ and explicitly state the condition under which it avoids UV catastrophe, for example exponential suppression from an analytic or sufficiently smooth transition versus unacceptable power-law behavior from the sharp $\Theta$ idealization.

---

## Execution Step Results

### Step 1: Derive the physical scale factor from $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$, choosing $\eta_{e}=0$ if convenient. Track continuity of $a$ and $a'$ at $t=t_{e}$ and identify the nonanalyticity in higher derivatives caused by the sudden transition.

**Reasoning:**
Integrating the proper-time equation separately on the two sides of $t_e$ gives an exponential scale factor before the transition and a power-law scale factor after it. The integration constants are fixed by $a(t_e)=a_e$. Conformal time is obtained from $d\eta=dt/a(t)$, again integrated separately on each branch and normalized by setting $\eta_e=0$. Inverting the resulting relations gives the conformal-time scale factor. Differentiating both conformal-time branches shows that $a$ and $a'$ match at $\eta=0$, while $a''$ does not. Hence the sudden change in the Hubble law creates a nonanalyticity in higher derivatives, specifically a discontinuity starting at second derivative order.

**Result:**
Let $\Delta t\equiv t-t_e$. Away from the transition point, the equation is piecewise
$$
\frac{d\ln a}{dt}=\begin{cases}
H_I, & t<t_e,\\[4pt]
\dfrac{H_I}{1+\frac32 H_I(t-t_e)}, & t>t_e.
\end{cases}
$$
With $a(t_e)=a_e$, integration gives
$$
a(t)=\begin{cases}
a_e e^{H_I(t-t_e)}, & t<t_e,\\[6pt]
a_e\left[1+\dfrac32 H_I(t-t_e)\right]^{2/3}, & t\ge t_e.
\end{cases}
$$
Thus the pre-transition phase is de Sitter-like, while the post-transition phase has the matter-dominated form $a\propto t^{2/3}$ at late times.

Now choose $\eta_e=0$, so that $t=t_e$ corresponds to $\eta=0$. Since $dt=a\,d\eta$, we have
$$
\eta=\int_{t_e}^{t}\frac{dt'}{a(t')}.
$$
For $t<t_e$,
$$
\eta=\frac{1}{a_eH_I}\left[1-e^{-H_I(t-t_e)}\right],
$$
so
$$
e^{H_I(t-t_e)}=\frac{1}{1-a_eH_I\eta},
$$
and therefore
$$
a(\eta)=\frac{a_e}{1-a_eH_I\eta},\qquad \eta<0.
$$
For $t\ge t_e$,
$$
\eta=\frac{2}{a_eH_I}\left[\left(1+\frac32 H_I(t-t_e)\right)^{1/3}-1\right],
$$
so
$$
\left(1+\frac32 H_I(t-t_e)\right)^{1/3}=1+\frac12 a_eH_I\eta,
$$
and hence
$$
a(\eta)=a_e\left(1+\frac12 a_eH_I\eta\right)^2,\qquad \eta\ge 0.
$$
Thus, with $\eta_e=0$,
$$
\boxed{
a(\eta)=\begin{cases}
\dfrac{a_e}{1-a_eH_I\eta}, & \eta<0,\\[10pt]
a_e\left(1+\dfrac12 a_eH_I\eta\right)^2, & \eta\ge 0.
\end{cases}}
$$
At $\eta=0$, both pieces give
$$
a(0^-)=a(0^+)=a_e.
$$
The conformal-time derivative is also continuous. For $\eta<0$,
$$
a'(\eta)=\frac{a_e^2H_I}{(1-a_eH_I\eta)^2},
$$
so $a'(0^-)=a_e^2H_I$. For $\eta>0$,
$$
a'(\eta)=a_e^2H_I\left(1+\frac12 a_eH_I\eta\right),
$$
so $a'(0^+)=a_e^2H_I$. Therefore
$$
\boxed{a'(0^-)=a'(0^+)=a_e^2H_I.}
$$
However, the second derivative jumps. For $\eta<0$,
$$
a''(\eta)=\frac{2a_e^3H_I^2}{(1-a_eH_I\eta)^3},
$$
so
$$
a''(0^-)=2a_e^3H_I^2.
$$
For $\eta>0$,
$$
a''(\eta)=\frac12 a_e^3H_I^2,
$$
so
$$
a''(0^+)=\frac12 a_e^3H_I^2.
$$
Thus
$$
\boxed{a''(0^-)\neq a''(0^+).}
$$
The sudden transition therefore produces a scale factor that is $C^1$ but not $C^2$ in conformal time. Equivalently, in proper time, $a$ and $\dot a$ are continuous at $t=t_e$, but $\ddot a$ jumps. The scale factor is piecewise analytic but nonanalytic at the transition surface.

**Analysis:**
Integrating the proper-time equation separately on the two sides of $t_e$ gives an exponential scale factor before the transition and a power-law scale factor after it. The integration constants are fixed by $a(t_e)=a_e$. Conformal time is obtained from $d\eta=dt/a(t)$, again integrated separately on each branch and normalized by setting $\eta_e=0$. Inverting the resulting relations gives the conformal-time scale factor. Differentiating both conformal-time branches shows that $a$ and $a'$ match at $\eta=0$, while $a''$ does not. Hence the sudden change in the Hubble law creates a nonanalyticity in higher derivatives, specifically a discontinuity starting at second derivative order.

### Step 2: Before applying the one-pole contour estimate, impose a UV-consistent prescription: verify whether the sharp $\Theta$ transition produces a power-law high-$k$ tail in $|\beta(k)|$ from discontinuities of derivatives of $a(\eta)$, and either include the corresponding boundary contribution or state that a smoothed/adiabatic transition is assumed so that the one-pole exponential result is meaningful and avoids a UV catastrophe in $\int d^{3}k\,|\beta(k)|^{2}$ or $\int d^{3}k\,\omega_{k}|\beta(k)|^{2}$.

**Reasoning:**
The sudden transition found in Step 1 makes $a$ and $a'$ continuous but $a''$ discontinuous. Since $\omega^2=k^2+m^2a^2$, $\omega$ and $\omega'$ are continuous, so the integrand prefactor $f=\omega'/(2\omega)$ is continuous. However $f'$ contains the term $m^2aa''/(2\omega^2)$ and therefore inherits a finite jump proportional to $[a'']$. For an oscillatory integral with a continuous amplitude but a jump in its first derivative, the first nonzero boundary contribution appears after two integrations by parts and scales as $[f']/(2\omega)^2$. Evaluating this at the transition gives $|\beta_{\rm bdry}|\sim k^{-4}$. This is a real-axis nonanalyticity contribution, independent of the complex pole contribution, and must be included unless one assumes the physical transition is smoothed. Although this particular $k^{-4}$ tail is UV-convergent in both number and energy density, it still dominates over any exponentially suppressed one-pole estimate at asymptotically high $k$.

**Result:**
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

**Analysis:**
Let $\Delta t\equiv t-t_e$. Away from the transition point, the equation is piecewise
$$
\frac{d\ln a}{dt}=\begin{cases}
H_I, & t<t_e,\\[4pt]
\dfrac{H_I}{1+\frac32 H_I(t-t_e)}, & t>t_e.
\end{cases}
$$
With $a(t_e)=a_e$, integration gives
$$
a(t)=\begin{cases}
a_e e^{H_I(t-t_e)}, & t<t_e,\\[6pt]
a_e\left[1+\dfrac32 H_I(t-t_e)\right]^{2/3}, & t\ge t_e.
\end{cases}
$$
Thus the pre-transition phase is de Sitter-like, while the post-transition phase has the matter-dominated form $a\propto t^{2/3}$ at late times.

Now choose $\eta_e=0$, so that $t=t_e$ corresponds to $\eta=0$. Since $dt=a\,d\eta$, we have
$$
\eta=\int_{t_e}^{t}\frac{dt'}{a(t')}.
$$
For $t<t_e$,
$$
\eta=\frac{1}{a_eH_I}\left[1-e^{-H_I(t-t_e)}\right],
$$
so
$$
e^{H_I(t-t_e)}=\frac{1}{1-a_eH_I\eta},
$$
and therefore
$$
a(\eta)=\frac{a_e}{1-a_eH_I\eta},\qquad \eta<0.
$$
For $t\ge t_e$,
$$
\eta=\frac{2}{a_eH_I}\left[\left(1+\frac32 H_I(t-t_e)\right)^{1/3}-1\right],
$$
so
$$
\left(1+\frac32 H_I(t-t_e)\right)^{1/3}=1+\frac12 a_eH_I\eta,
$$
and hence
$$
a(\eta)=a_e\left(1+\frac12 a_eH_I\eta\right)^2,\qquad \eta\ge 0.
$$
Thus, with $\eta_e=0$,
$$
\boxed{
a(\eta)=\begin{cases}
\dfrac{a_e}{1-a_eH_I\eta}, & \eta<0,\\[10pt]
a_e\left(1+\dfrac12 a_eH_I\eta\right)^2, & \eta\ge 0.
\end{cases}}
$$
At $\eta=0$, both pieces give
$$
a(0^-)=a(0^+)=a_e.
$$
The conformal-time derivative is also continuous. For $\eta<0$,
$$
a'(\eta)=\frac{a_e^2H_I}{(1-a_eH_I\eta)^2},
$$
so $a'(0^-)=a_e^2H_I$. For $\eta>0$,
$$
a'(\eta)=a_e^2H_I\left(1+\frac12 a_eH_I\eta\right),
$$
so $a'(0^+)=a_e^2H_I$. Therefore
$$
\boxed{a'(0^-)=a'(0^+)=a_e^2H_I.}
$$
However, the second derivative jumps. For $\eta<0$,
$$
a''(\eta)=\frac{2a_e^3H_I^2}{(1-a_eH_I\eta)^3},
$$
so
$$
a''(0^-)=2a_e^3H_I^2.
$$
For $\eta>0$,
$$
a''(\eta)=\frac12 a_e^3H_I^2,
$$
so
$$
a''(0^+)=\frac12 a_e^3H_I^2.
$$
Thus
$$
\boxed{a''(0^-)\neq a''(0^+).}
$$
The sudden transition therefore produces a scale factor that is $C^1$ but not $C^2$ in conformal time. Equivalently, in proper time, $a$ and $\dot a$ are continuous at $t=t_e$, but $\ddot a$ jumps. The scale factor is piecewise analytic but nonanalytic at the transition surface.

### Step 3: Insert the relevant analytic branch of $a(\eta)$ into $\omega_{k}(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$ and find the dominant singularity $\tilde{\eta}$ of $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ from $\omega_{k}^{2}(\tilde{\eta})=0$, selecting the pole or turning point with $\Re\tilde{\eta}>0$ that gives the smallest positive suppression in the limit $k/(a_{e}H_{I})\rightarrow\infty$.

**Reasoning:**
The post-transition branch is the correct analytic branch because the requested singularity has $\Re\tilde\eta>0$, while the transition has been placed at $\eta_e=0$. Substituting $a(\eta)=a_e(1+A\eta/2)^2$ into $\omega_k^2$ gives a quartic equation in $z=1+A\eta/2$. The zeros of $\omega_k^2$ are branch points of $\omega_k$ and therefore singularities of $\omega_k'/(2\omega_k)$. Solving $z^4=-q^2$ gives four roots separated by $\pi/2$. At large $q=k/(ma_e)$, the roots with phases $\pm\pi/4$ have positive real part, while those with phases $3\pi/4$ and $5\pi/4$ have negative real part. The integral contains $e^{-2i\int\omega d\eta}$, so the damped steepest-descent contour is reached through the lower-half plane; thus the root with phase $-\pi/4$ is selected as the dominant singularity for the one-pole approximation. Since $m\lesssim H_I$ and $k/(a_eH_I)\to\infty$, one has $q\to\infty$, ensuring $\Re\tilde\eta>0$.

**Result:**
Choose $\eta_e=0$ and define $A\equiv a_eH_I$. The relevant analytic branch with $\Re\eta>0$ is the post-transition branch
$$
a(\eta)=a_e\left(1+\frac{A\eta}{2}\right)^2 .
$$
Hence
$$
\omega_k^2(\eta)=k^2+m^2a_e^2\left(1+\frac{A\eta}{2}\right)^4 .
$$
The singularities of $\omega_k'/(2\omega_k)$ occur at the turning points where
$$
\omega_k^2(\tilde\eta)=0,
$$
so
$$
\left(1+\frac{A\tilde\eta}{2}\right)^4=-\frac{k^2}{m^2a_e^2}.
$$
Let
$$
q\equiv \frac{k}{ma_e}>0.
$$
Then the four turning points are
$$
1+\frac{A\tilde\eta_n}{2}=q^{1/2}\exp\left[i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right],\qquad n=0,1,2,3,
$$
or
$$
\tilde\eta_n=\frac{2}{a_eH_I}\left[q^{1/2}\exp\left(i\frac{\pi}{4}+i\frac{n\pi}{2}\right)-1\right].
$$
For $q\to\infty$, the two roots with $\Re\tilde\eta>0$ are
$$
\tilde\eta_{+}=\frac{2}{a_eH_I}\left(q^{1/2}e^{i\pi/4}-1\right),
\qquad
\tilde\eta_{-}=\frac{2}{a_eH_I}\left(q^{1/2}e^{-i\pi/4}-1\right).
$$
For the phase convention in
$$
\exp\left[-2i\int_0^\eta \omega_k(\eta')d\eta'\right],
$$
the steepest-descent deformation giving exponential damping lies in the lower half $\eta$-plane. Therefore the dominant one-pole/turning-point singularity is
$$
\boxed{
\tilde\eta=\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{-i\pi/4}-1\right]
}
$$
with
$$
\Re\tilde\eta=\frac{2}{a_eH_I}\left[\frac{1}{\sqrt2}\left(\frac{k}{ma_e}\right)^{1/2}-1\right]>0
$$
for $k/(a_eH_I)\to\infty$ and $m\lesssim H_I$, and
$$
\Im\tilde\eta=-\frac{\sqrt2}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}<0.
$$
The conjugate upper-half root has the same real part but gives the opposite sign of the imaginary phase contribution for this contour choice. The other two roots have $\Re\tilde\eta<0$ at large $q$ and are not the dominant post-transition one-pole singularities required here.

**Analysis:**
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

### Step 4: Evaluate the local one-pole contribution by expanding $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ near $\tilde{\eta}$ and combine it with the steepest-descent phase $\exp\left[-2i\int_{\eta_{e}}^{\tilde{\eta}}d\eta'\,\omega_{k}(\eta')\right]$, retaining the leading magnitude and discarding irrelevant phases.

**Reasoning:**
The factor $\omega_k'/(2\omega_k)$ can be written as $(\omega_k^2)'/(4\omega_k^2)$. At a simple zero of $\omega_k^2$, it therefore has a simple pole with universal residue $1/4$, independent of the detailed slope of $\omega_k^2$. The dominant turning point selected in Step 3 lies in the lower half-plane, consistent with the phase convention $\exp[-2i\int\omega]$. Deforming the real contour through the one-pole/steepest-descent contribution gives a residue magnitude $2\pi\times(1/4)=\pi/2$. The phase integral is then evaluated on the post-transition branch. After changing variables to $z=1+A\eta/2$ and then to $z=q^{1/2}y$, the large-$q$ leading imaginary part comes from the path from $y=0$ to $y=e^{-i\pi/4}$. Parameterizing this path by $y=e^{-i\pi/4}x$ reduces the integral to the positive real constant $C=\int_0^1\sqrt{1-x^4}\,dx$. The imaginary part of the action is negative, so $\mathrm{Re}[-2iS]=2\,\mathrm{Im}S<0$, producing the stated exponential suppression. Subleading contributions from the lower endpoint $z=1$ are smaller by $q^{-1/2}$ relative to the leading complex action and contribute only irrelevant or subleading phase/magnitude corrections.

**Result:**
Let $A\equiv a_eH_I$ and introduce $$z\equiv 1+\frac{A\eta}{2},\qquad q\equiv \frac{k}{ma_e}.$$ On the relevant post-transition branch, $$\omega_k^2(\eta)=k^2+m^2a_e^2z^4.$$ Near the dominant turning point $$z_t=q^{1/2}e^{-i\pi/4},\qquad \tilde\eta=\frac{2}{A}(z_t-1),$$ we have $$\omega_k^2(\eta)\simeq (\omega_k^2)'_{\tilde\eta}(\eta-\tilde\eta),$$ and therefore $$\frac{\omega_k'}{2\omega_k}=\frac{1}{4}\frac{(\omega_k^2)'}{\omega_k^2}\simeq \frac{1}{4}\frac{1}{\eta-\tilde\eta}.$$ Thus the local singularity has residue $1/4$. The one-pole contour contribution is therefore, up to an irrelevant phase, $$\beta_{\rm pole}(k)\simeq \frac{\pi}{2}\exp\left[-2i\int_{0}^{\tilde\eta}d\eta\,\omega_k(\eta)\right],$$ where the factor $\pi/2$ is the magnitude of $2\pi i$ times the residue $1/4$. The leading large-$q$ part of the phase is $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)=\frac{2k}{A}\int_{1}^{z_t}dz\,\sqrt{1+\frac{z^4}{q^2}}.$$ For $q\to\infty$, set $z=q^{1/2}y$. The lower endpoint gives only a subleading, mostly real phase, so the leading complex contribution is $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\simeq \frac{2k}{A}q^{1/2}\int_0^{e^{-i\pi/4}}dy\,\sqrt{1+y^4}.$$ Along the steepest path $y=e^{-i\pi/4}x$, $0\le x\le1$, this becomes $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\simeq \frac{2k}{A}q^{1/2}e^{-i\pi/4}C,$$ with $$C\equiv \int_0^1dx\,\sqrt{1-x^4}=\frac14 B\left(\frac14,\frac32\right)=\frac{\sqrt\pi}{6}\frac{\Gamma(1/4)}{\Gamma(3/4)}.$$ Hence $$\left|\exp\left[-2i\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\right]\right|=\exp\left[-2\sqrt2\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right].$$ Therefore the leading one-pole magnitude is $$\boxed{|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-2\sqrt2\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]}$$ with $$2\sqrt2\,C=\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}.$$ Equivalently, $$\boxed{|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]}.$$ This result discards the irrelevant overall phase and keeps the leading exponential suppression and the residue prefactor.

**Analysis:**
Choose $\eta_e=0$ and define $A\equiv a_eH_I$. The relevant analytic branch with $\Re\eta>0$ is the post-transition branch
$$
a(\eta)=a_e\left(1+\frac{A\eta}{2}\right)^2 .
$$
Hence
$$
\omega_k^2(\eta)=k^2+m^2a_e^2\left(1+\frac{A\eta}{2}\right)^4 .
$$
The singularities of $\omega_k'/(2\omega_k)$ occur at the turning points where
$$
\omega_k^2(\tilde\eta)=0,
$$
so
$$
\left(1+\frac{A\tilde\eta}{2}\right)^4=-\frac{k^2}{m^2a_e^2}.
$$
Let
$$
q\equiv \frac{k}{ma_e}>0.
$$
Then the four turning points are
$$
1+\frac{A\tilde\eta_n}{2}=q^{1/2}\exp\left[i\left(\frac{\pi}{4}+\frac{n\pi}{2}\right)\right],\qquad n=0,1,2,3,
$$
or
$$
\tilde\eta_n=\frac{2}{a_eH_I}\left[q^{1/2}\exp\left(i\frac{\pi}{4}+i\frac{n\pi}{2}\right)-1\right].
$$
For $q\to\infty$, the two roots with $\Re\tilde\eta>0$ are
$$
\tilde\eta_{+}=\frac{2}{a_eH_I}\left(q^{1/2}e^{i\pi/4}-1\right),
\qquad
\tilde\eta_{-}=\frac{2}{a_eH_I}\left(q^{1/2}e^{-i\pi/4}-1\right).
$$
For the phase convention in
$$
\exp\left[-2i\int_0^\eta \omega_k(\eta')d\eta'\right],
$$
the steepest-descent deformation giving exponential damping lies in the lower half $\eta$-plane. Therefore the dominant one-pole/turning-point singularity is
$$
\boxed{
\tilde\eta=\frac{2}{a_eH_I}\left[\left(\frac{k}{ma_e}\right)^{1/2}e^{-i\pi/4}-1\right]
}
$$
with
$$
\Re\tilde\eta=\frac{2}{a_eH_I}\left[\frac{1}{\sqrt2}\left(\frac{k}{ma_e}\right)^{1/2}-1\right]>0
$$
for $k/(a_eH_I)\to\infty$ and $m\lesssim H_I$, and
$$
\Im\tilde\eta=-\frac{\sqrt2}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}<0.
$$
The conjugate upper-half root has the same real part but gives the opposite sign of the imaginary phase contribution for this contour choice. The other two roots have $\Re\tilde\eta<0$ at large $q$ and are not the dominant post-transition one-pole singularities required here.

### Step 5: Compare the one-pole exponential contribution with any UV boundary or sudden-transition contribution found earlier; report the dominant UV-safe expression for $|\beta(k)|$ and explicitly state the condition under which it avoids UV catastrophe, for example exponential suppression from an analytic or sufficiently smooth transition versus unacceptable power-law behavior from the sharp $\Theta$ idealization.

**Reasoning:**
The comparison is between the complex-plane singularity contribution and the real-axis nonanalyticity contribution. The one-pole term is exponentially small at large $k$, scaling as $\exp[-{\rm const}\, k^{3/2}]$ in the dimensionless combination $[k/(a_eH_I)] [k/(ma_e)]^{1/2}$. The sharp transition gives a boundary term because $f(\eta)=\omega_k'/(2\omega_k)$ is continuous but $f'$ jumps, producing a $k^{-4}$ contribution. Any power law dominates an exponential at sufficiently large $k$, so the literal sharp-$\Theta$ asymptotic is the boundary term, not the pole term. Nevertheless, $k^{-4}$ is soft enough to make both $\int d^3k |\beta|^2$ and $\int d^3k\,\omega_k |\beta|^2$ converge. If the transition is smoothed so that the derivative discontinuity is removed, the boundary contribution disappears and the one-pole exponential becomes the dominant UV-safe estimate.

**Result:**
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

**Analysis:**
Let $A\equiv a_eH_I$ and introduce $$z\equiv 1+\frac{A\eta}{2},\qquad q\equiv \frac{k}{ma_e}.$$ On the relevant post-transition branch, $$\omega_k^2(\eta)=k^2+m^2a_e^2z^4.$$ Near the dominant turning point $$z_t=q^{1/2}e^{-i\pi/4},\qquad \tilde\eta=\frac{2}{A}(z_t-1),$$ we have $$\omega_k^2(\eta)\simeq (\omega_k^2)'_{\tilde\eta}(\eta-\tilde\eta),$$ and therefore $$\frac{\omega_k'}{2\omega_k}=\frac{1}{4}\frac{(\omega_k^2)'}{\omega_k^2}\simeq \frac{1}{4}\frac{1}{\eta-\tilde\eta}.$$ Thus the local singularity has residue $1/4$. The one-pole contour contribution is therefore, up to an irrelevant phase, $$\beta_{\rm pole}(k)\simeq \frac{\pi}{2}\exp\left[-2i\int_{0}^{\tilde\eta}d\eta\,\omega_k(\eta)\right],$$ where the factor $\pi/2$ is the magnitude of $2\pi i$ times the residue $1/4$. The leading large-$q$ part of the phase is $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)=\frac{2k}{A}\int_{1}^{z_t}dz\,\sqrt{1+\frac{z^4}{q^2}}.$$ For $q\to\infty$, set $z=q^{1/2}y$. The lower endpoint gives only a subleading, mostly real phase, so the leading complex contribution is $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\simeq \frac{2k}{A}q^{1/2}\int_0^{e^{-i\pi/4}}dy\,\sqrt{1+y^4}.$$ Along the steepest path $y=e^{-i\pi/4}x$, $0\le x\le1$, this becomes $$\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\simeq \frac{2k}{A}q^{1/2}e^{-i\pi/4}C,$$ with $$C\equiv \int_0^1dx\,\sqrt{1-x^4}=\frac14 B\left(\frac14,\frac32\right)=\frac{\sqrt\pi}{6}\frac{\Gamma(1/4)}{\Gamma(3/4)}.$$ Hence $$\left|\exp\left[-2i\int_0^{\tilde\eta}d\eta\,\omega_k(\eta)\right]\right|=\exp\left[-2\sqrt2\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right].$$ Therefore the leading one-pole magnitude is $$\boxed{|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-2\sqrt2\,C\,\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]}$$ with $$2\sqrt2\,C=\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}.$$ Equivalently, $$\boxed{|\beta_{\rm pole}(k)|\simeq \frac{\pi}{2}\exp\left[-\frac{\sqrt{2\pi}}{3}\frac{\Gamma(1/4)}{\Gamma(3/4)}\frac{k}{a_eH_I}\left(\frac{k}{ma_e}\right)^{1/2}\right]}.$$ This result discards the irrelevant overall phase and keeps the leading exponential suppression and the residue prefactor.

---

## Final Result
{"result": "The one-pole contribution obtained from the dominant complex turning point is
$$
|\\beta_{\\rm pole}(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-\\alpha\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right],
\\qquad
\\alpha\\equiv \\frac{\\sqrt{2\\pi}}{3}\\frac{\\Gamma(1/4)}{\\Gamma(3/4)}.
$$
Equivalently,
$$
|\\beta_{\\rm pole}(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-2\\sqrt{2}\\,C\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right],
\\qquad
C=\\int_0^1 dx\\,\\sqrt{1-x^4}.
$$
However, for the exact sharp $\\Theta$ scale factor, the transition is only $C^1$ in conformal time: $a$ and $a'$ are continuous, but $a''$ jumps at $\\eta=0$. This produces a real-axis boundary contribution
$$
|\\beta_{\\rm bdry}(k)|\\simeq \\frac{3m^2a_e^4H_I^2}{16\\left(k^2+m^2a_e^2\\right)^2}
\\xrightarrow{k\\gg a_eH_I,\\,ma_e}
\\frac{3m^2a_e^4H_I^2}{16k^4}.
$$
Since a power law dominates over an exponential at asymptotically large $k$, the exact sharp-$\\Theta$ model has
$$
|\\beta(k)|\\simeq |\\beta_{\\rm bdry}(k)|
$$
in the strict UV, with the exponentially small pole term subleading.

Thus there are two physically distinct statements:

1. For the literal sharp $\\Theta$ transition,
$$
|\\beta(k)|\\simeq \\frac{3m^2a_e^4H_I^2}{16\\left(k^2+m^2a_e^2\\right)^2}
+O\\!\\left(\\exp\\left[-\\alpha\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right]\\right),
$$
up to phases and possible interference. This is not exponentially suppressed, because it is an artifact of the nonanalytic transition. In the present $C^1$ case the $k^{-4}$ tail is still UV convergent for both number and energy densities:
$$
\\int d^3k\\,|\\beta|^2\\sim \\int^\\infty dk\\,k^2k^{-8}<\\infty,
\\qquad
\\int d^3k\\,\\omega_k|\\beta|^2\\sim \\int^\\infty dk\\,k^3k^{-8}<\\infty.
$$
So this particular power law is UV safe, but it is not the one-pole exponential asymptotic.

2. If the $\\Theta$ transition is understood as an idealization of an analytic or sufficiently smooth adiabatic transition, so that the derivative discontinuity at $\\eta=0$ is removed, then the artificial boundary term is absent or parametrically suppressed. In that UV-consistent smoothed model, the dominant one-pole result is
$$
\\boxed{
|\\beta(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-\\frac{\\sqrt{2\\pi}}{3}\\frac{\\Gamma(1/4)}{\\Gamma(3/4)}\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right]
}
$$
for $k/(a_eH_I)\\to\\infty$ and $0<m\\lesssim H_I$.

The condition for avoiding a UV catastrophe is that the transition be analytic or sufficiently smooth/adiabatic so that no discontinuity produces a hard high-$k$ tail. Exponential suppression is manifestly UV safe. More generally, if a residual power-law tail $|\\beta|\\sim k^{-p}$ remains, finite particle number requires $p>3/2$, and finite energy density requires $p>2$ for relativistic UV modes. The present sharp model gives $p=4$, so it is convergent, but a less smooth sudden transition could yield an unacceptable UV-divergent power law. Therefore, the clean one-pole expression should be quoted as the dominant UV-safe result only after smoothing the sharp $\\Theta$ idealization.", "physical_interpretation": "The one-pole contribution obtained from the dominant complex turning point is
$$
|\\beta_{\\rm pole}(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-\\alpha\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right],
\\qquad
\\alpha\\equiv \\frac{\\sqrt{2\\pi}}{3}\\frac{\\Gamma(1/4)}{\\Gamma(3/4)}.
$$
Equivalently,
$$
|\\beta_{\\rm pole}(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-2\\sqrt{2}\\,C\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right],
\\qquad
C=\\int_0^1 dx\\,\\sqrt{1-x^4}.
$$
However, for the exact sharp $\\Theta$ scale factor, the transition is only $C^1$ in conformal time: $a$ and $a'$ are continuous, but $a''$ jumps at $\\eta=0$. This produces a real-axis boundary contribution
$$
|\\beta_{\\rm bdry}(k)|\\simeq \\frac{3m^2a_e^4H_I^2}{16\\left(k^2+m^2a_e^2\\right)^2}
\\xrightarrow{k\\gg a_eH_I,\\,ma_e}
\\frac{3m^2a_e^4H_I^2}{16k^4}.
$$
Since a power law dominates over an exponential at asymptotically large $k$, the exact sharp-$\\Theta$ model has
$$
|\\beta(k)|\\simeq |\\beta_{\\rm bdry}(k)|
$$
in the strict UV, with the exponentially small pole term subleading.

Thus there are two physically distinct statements:

1. For the literal sharp $\\Theta$ transition,
$$
|\\beta(k)|\\simeq \\frac{3m^2a_e^4H_I^2}{16\\left(k^2+m^2a_e^2\\right)^2}
+O\\!\\left(\\exp\\left[-\\alpha\\,\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right]\\right),
$$
up to phases and possible interference. This is not exponentially suppressed, because it is an artifact of the nonanalytic transition. In the present $C^1$ case the $k^{-4}$ tail is still UV convergent for both number and energy densities:
$$
\\int d^3k\\,|\\beta|^2\\sim \\int^\\infty dk\\,k^2k^{-8}<\\infty,
\\qquad
\\int d^3k\\,\\omega_k|\\beta|^2\\sim \\int^\\infty dk\\,k^3k^{-8}<\\infty.
$$
So this particular power law is UV safe, but it is not the one-pole exponential asymptotic.

2. If the $\\Theta$ transition is understood as an idealization of an analytic or sufficiently smooth adiabatic transition, so that the derivative discontinuity at $\\eta=0$ is removed, then the artificial boundary term is absent or parametrically suppressed. In that UV-consistent smoothed model, the dominant one-pole result is
$$
\\boxed{
|\\beta(k)|\\simeq \\frac{\\pi}{2}\\exp\\left[-\\frac{\\sqrt{2\\pi}}{3}\\frac{\\Gamma(1/4)}{\\Gamma(3/4)}\\frac{k}{a_eH_I}\\left(\\frac{k}{ma_e}\\right)^{1/2}\\right]
}
$$
for $k/(a_eH_I)\\to\\infty$ and $0<m\\lesssim H_I$.

The condition for avoiding a UV catastrophe is that the transition be analytic or sufficiently smooth/adiabatic so that no discontinuity produces a hard high-$k$ tail. Exponential suppression is manifestly UV safe. More generally, if a residual power-law tail $|\\beta|\\sim k^{-p}$ remains, finite particle number requires $p>3/2$, and finite energy density requires $p>2$ for relativistic UV modes. The present sharp model gives $p=4$, so it is convergent, but a less smooth sudden transition could yield an unacceptable UV-divergent power law. Therefore, the clean one-pole expression should be quoted as the dominant UV-safe result only after smoothing the sharp $\\Theta$ idealization.", "consistency_check": "passed", "potential_issues": "", "step_complete": true}