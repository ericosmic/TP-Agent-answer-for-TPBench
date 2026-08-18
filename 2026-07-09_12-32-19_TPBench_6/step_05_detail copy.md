# Step 5 — Combine the one-pole prefactor and steepest-descent exponential to state the final leading asymptotic expression for $|\beta(k)|$ in terms of $k$, $a_{e}$, $H_{I}$, and $m$, with validity for $0<m\lesssim H_{I}$ and $k/(a_{e}H_{I})\rightarrow\infty$.

## Solution Reasoning

Step 3 gives
$$
|\beta(k)|_{\text{1-pole}}\simeq \frac{\pi}{3}\left|\exp\left[-2i\int_{\eta_e}^{\tilde\eta}\omega_k(\eta)d\eta\right]\right|.
$$
Step 4 finds
$$
-2i\int_{\eta_e}^{\tilde\eta}\omega_k d\eta
=-\frac{\pi m}{H_I}-\frac{2ik}{a_eH_I}
+i\,O\!\left(\frac{m^2a_e}{kH_I}\right).
$$
The real part is $-\pi m/H_I$, producing the suppression $e^{-\pi m/H_I}$. The terms involving $k$ and $a_e$ are imaginary and hence contribute only to the phase. Multiplication by the pole prefactor therefore yields $(\pi/3)e^{-\pi m/H_I}$. No specific relative correction of order $m^2a_e/(kH_I)$ can be assigned to the magnitude from the displayed action because that omitted action term is purely a phase; subleading magnitude corrections would require additional analysis of the prefactor or real part of the action.

## Result

Combining the one-pole prefactor with the steepest-descent suppression gives
$$
\boxed{\left|\beta(k)\right|\sim \frac{\pi}{3}\exp\!\left(-\frac{\pi m}{H_I}\right)},
\qquad 0<m\lesssim H_I,\qquad \frac{k}{a_eH_I}\to\infty.
$$
More precisely, at the level of the established leading asymptotics,
$$
\left|\beta(k)\right|=\frac{\pi}{3}e^{-\pi m/H_I}[1+o(1)].
$$
Thus the leading magnitude is independent of $k$ and $a_e$; these parameters enter the leading complex coefficient only through an oscillatory phase. Up to uncomputed subleading prefactor corrections, one may write schematically
$$
\beta(k)\sim \frac{\pi}{3}e^{-\pi m/H_I}
\exp\!\left[-\frac{2ik}{a_eH_I}+i\,O\!\left(\frac{m^2a_e}{kH_I}\right)\right].
$$

## Physical Interpretation

Combining the one-pole prefactor with the steepest-descent suppression gives
$$
\boxed{\left|\beta(k)\right|\sim \frac{\pi}{3}\exp\!\left(-\frac{\pi m}{H_I}\right)},
\qquad 0<m\lesssim H_I,\qquad \frac{k}{a_eH_I}\to\infty.
$$
More precisely, at the level of the established leading asymptotics,
$$
\left|\beta(k)\right|=\frac{\pi}{3}e^{-\pi m/H_I}[1+o(1)].
$$
Thus the leading magnitude is independent of $k$ and $a_e$; these parameters enter the leading complex coefficient only through an oscillatory phase. Up to uncomputed subleading prefactor corrections, one may write schematically
$$
\beta(k)\sim \frac{\pi}{3}e^{-\pi m/H_I}
\exp\!\left[-\frac{2ik}{a_eH_I}+i\,O\!\left(\frac{m^2a_e}{kH_I}\right)\right].
$$

**Consistency check:** passed
