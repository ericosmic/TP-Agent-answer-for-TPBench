Topic:
One-Pole Problem

Problem:
Consider the conformally coupled scalar field $\phi$ 
$$

$$
\begin{equation}
\mathcal{L}=\frac{1}{2}\left[g^{\mu\nu}\partial_{\mu}\phi\partial_{\nu}\phi-\left(m^{2}-\frac{1}{6}R\right)\phi^{2}\right]
\end{equation}
$$

$$
in curved spacetime
$$
ds^{2}=a^{2}(\eta)\left(d\eta^{2}-|d\vec{x}|^{2}\right)
$$
where the Ricci scalar is
$$

$$
\begin{equation}
R=-6\frac{a''(\eta)}{a(\eta)}
\end{equation}
$$

$$
and $a$ satisfies the differential equation
$$

$$
\begin{equation}
\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}\label{eq:scalefactor-onepole}
\end{equation}
$$

$$
with $t_{e}$ a finite positive number, the $\Theta$ function having
the steplike behavior
$$

$$
\begin{equation}
\Theta(t-t_{e})\equiv\begin{cases}
1 & t\geq t_{e}\\
0 & \mbox{otherwise}
\end{cases},
\end{equation}
$$

$$
and $t$ being the comoving proper time related to $\eta$ through
$$

$$
\begin{equation}
t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy.
\end{equation}
$$

$$
The boundary condition for the differential equation (in comoving
proper time) is $a|_{t=t_{e}}=a_{e}$.

In the limit that $k/(a_{e}H_{I})\rightarrow\infty$, using the steepest
descent approximation starting from the dominant pole $\tilde{\eta}$
(with $\Re\tilde{\eta}>0$) of the integrand factor $\omega_{k}'(\eta)/\left(2\omega_{k}(\eta)\right)$,
compute the Bogoliubov coefficient magnitude $|\beta(k)|$ approximated
as
$$

$$
\begin{equation}
|\beta(k)|\approx\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{e}}^{\eta}d\eta'\omega_{k}(\eta')}\right|\label{eq:originalbeta}
\end{equation}
$$

$$
for particle production where the dispersion relationship given by
$$

$$
\begin{equation}
\omega_{k}^{2}(\eta)=k^{2}+m^{2}a^{2}(\eta)
\end{equation}
$$

$$
with $0<m\lesssim H_{I}$. Use a one pole approximation which dominates
in this limit.

Domain:
Cosmology