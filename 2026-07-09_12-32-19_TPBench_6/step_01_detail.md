# Step 1 — Derive the physical scale factor from $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$, choosing $\eta_{e}=0$ if convenient. Track continuity of $a$ and $a'$ at $t=t_{e}$ and identify the nonanalyticity in higher derivatives caused by the sudden transition.

## Solution Reasoning

Integrating the proper-time equation separately on the two sides of $t_e$ gives an exponential scale factor before the transition and a power-law scale factor after it. The integration constants are fixed by $a(t_e)=a_e$. Conformal time is obtained from $d\eta=dt/a(t)$, again integrated separately on each branch and normalized by setting $\eta_e=0$. Inverting the resulting relations gives the conformal-time scale factor. Differentiating both conformal-time branches shows that $a$ and $a'$ match at $\eta=0$, while $a''$ does not. Hence the sudden change in the Hubble law creates a nonanalyticity in higher derivatives, specifically a discontinuity starting at second derivative order.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
