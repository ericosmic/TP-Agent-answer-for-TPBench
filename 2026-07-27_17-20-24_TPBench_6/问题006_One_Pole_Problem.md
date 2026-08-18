---
row_number: 6
csv_index: 5
problem_id: One-Pole Problem
domain: Cosmology
difficulty_level: 5
---

## Solution

\begin{figure}
\begin{centering}
\begin{tikzpicture} 
\draw[->] (-5,0) -- (5,0); 
\draw[blue,ultra thick, ->] (-4,-0.1) -- (4,-0.1); 
\draw plot[only marks, mark=x, mark size=4pt](0,-1);
\draw[ultra thick, orange, ->] (-4,-.1) arc (180:225:4);
\draw[ultra thick, orange, ->] (-2.82843, -2.92843) -- (-.2,-1);
\draw[ultra thick, orange] (-.2,-1) arc (180:0:.2);
\draw[ultra thick, orange,->] (+.2,-1) -- (3.87052, -1.98351);
\draw[ultra thick, orange, ->] (3.87052, -1.98351) arc (345:371:4);
\draw[gray, dashed] (-5,-1) -- (5, -1);
\draw[purple] (0,-1) -- (2.82843, 1.82843);
\draw[green] (0,-1) -- (-4.82963, 0.294095);
\draw[draw=red, snake it] (0,-1) -- (1.03528, -4.8637);
\usetikzlibrary {angles,quotes} 
\draw [transparent] (5,-1) coordinate (A) -- (0,-1) coordinate (B)
         -- (2.82843, 1.82843) coordinate (C);
\draw pic ["$\pi/4$",ultra thick, draw,->,purple,angle radius=1cm] {angle = A--B--C}; 
\draw [transparent] (5,-1) coordinate (D) -- (0,-1) coordinate (E)
         -- (-4.82963, 0.294095) coordinate (F);
\draw pic ["$11\pi/12$", draw,->,green,angle radius=1cm] {angle = D--E--F}; 

\end{tikzpicture}
\par\end{centering}
\caption{\label{fig:The-original-contour}\footnotesize The original contour in blue is deformed
into the orange contour in the lower half complex plane of $\eta$.
The large radius arcs have vanishing contributions, and one-pole approximation
has been taken. The upper green and purple boundaries correspond to
where integrations over any arcs extended beyond this boundary would not converge. The
dashed horizontal curve is parallel to the real axis.  The red squiggly line is the branch cut at $-5 \pi/12$.}
\end{figure}

To find the pole of $\omega_{k}'(\eta)/\omega_{k}(\eta)$, we need
$a(\eta)$ from the given differential equation
\begin{equation}
\frac{d\ln a}{dt}=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}.\label{eq:Hubble}
\end{equation}
Integrating from time $t=t_{e}$, we find
\begin{align}
\ln\frac{a}{a_{e}} & =\int_{t_{e}}^{t}dT\frac{H_{I}}{1+\frac{3}{2}H_{I}(T-t_{e})}\\
 & =\frac{2}{3}\ln\left[1+\frac{3}{2}H_{I}(T-t_{e})\right]_{t_{e}}^{t}\\
 & =\frac{2}{3}\ln\left[1+\frac{3}{2}H_{I}(t-t_{e})\right]
\end{align}
for $t\geq t_{e}$. In other words, this scale factor
\begin{equation}
\frac{a}{a_{e}}=\left[1+\frac{3}{2}H_{I}(t-t_{e})\right]^{2/3}\label{eq:aHeq}
\end{equation}
behaves as a typical coherent oscillations spacetime minus the oscillatory
effects. Hence, note that for $t\gg t_{e}$, the scale factor can
be approximated as 
\begin{equation}
a(\eta)\approx c_{1}\eta^{2}
\end{equation}
for $\eta\gg\eta_{e}$ (where $\eta_{e}$ is the corresponding conformal
time for $t_{e}$) where we see by matching 
\begin{equation}
\int_{\eta_{i}}^{\eta}a(\eta)d\eta=t-t_{i}
\end{equation}
with $\eta_{i}\gg\eta_{e}$ and $t_{i}\gg t_{e}$, we can write
\begin{equation}
\frac{1}{3}c_{1}\eta^{3}\approx t
\end{equation}
for times much larger than $\eta_{i}$. This means that at time $\eta_{i}\gg\eta_{e}$,
we have
\begin{equation}
c_{1}\approx\frac{2}{H(\eta_{i})\eta_{i}^{3}}
\end{equation}
(where the Hubble expansion rate is $H(\eta)=a'(\eta)/a^{2}(\eta)$)
which gives
\begin{equation}
a(\eta)\approx\frac{2\eta^{2}}{H(\eta_{i})\eta_{i}^{3}}
\end{equation}
for $\eta>\eta_{i}$ where the choice of $\eta_{i}$ controls the
approximation error proportional to positive power of $\eta_{e}/\eta_{i}$.
Since $\eta_{i}\gg\eta_{e}>0$, we can approximate $\eta=0$ to be
equivalent to $\eta-\eta_{i}\rightarrow-\infty$. In other words,
when we analytically continue and consider the poles of the integrand,
we will consider only the region with $\Re\eta>0$.

Next, note the pole of

\begin{equation}
\frac{\omega'}{2\omega}=\frac{m^{2}\partial_{\eta}a^{2}}{4\left(k^{2}+m^{2}a^{2}\right)}
\end{equation}
is at $\tilde{\eta}$ defined by 
\begin{equation}
k^{2}=-m^{2}a^{2}(\tilde{\eta})\label{eq:poleexpl}
\end{equation}
which means
\begin{align*}
\tilde{\eta} & =\sqrt{\frac{H(\eta_{i})\eta_{i}^{3}}{2}}\left(\frac{-k^{2}}{m^{2}}\right)^{1/4}\\
 & =\eta_{i}\sqrt{\frac{1}{a(\eta_{i})}}\left(\frac{-k^{2}}{m^{2}}\right)^{1/4}\\
 & =\eta_{i}e^{i(2l+1)\pi/4}\frac{\sqrt{k/a(\eta_{i})}}{\sqrt{m}}\numberthis \label{eq:branchpoints}
\end{align*}
where $l$ is an integer. We see that $\Re\tilde{\eta}\gg\eta_{i}$
for $k/a(\eta_{e})\gg k/a(\eta_{i})\gg m$. We also see that $l\in\{1,2\}$
have negative $\Re\tilde{\eta}$ which are in the region that we excised
with the $\eta-\eta_{i}\rightarrow-\infty$ discussed above. That
means we can consider either $l\in\{3,4\}$. We will see below that
one of these poles is irrelevant.

Eq.~(\ref{eq:originalbeta}) tells us that

\begin{align*}
\left|\beta(\eta)\right| & =\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{e}}^{\eta}d\eta'\omega_{k}(\eta')}\right|\\
 & =\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{i}}^{\eta}d\eta'\omega_{k}(\eta')}e^{-2i\int_{\eta_{e}}^{\eta_{i}}d\eta'\omega_{k}(\eta')}\right|\\
 & =\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\int_{\eta_{i}}^{\eta}d\eta'\omega_{k}(\eta')}\right|.\numberthis
\end{align*}
With the steepest descent technique starting from the pole of $\omega_{k}'/\omega_{k}$,
we write after analytically continuing $\eta$
\begin{align*}
\left|\beta\right| & =\left|\int_{-\infty}^{\infty}d\eta\frac{\omega_{k}'(\eta)}{2\omega_{k}(\eta)}e^{-2i\left[\int_{\eta_{i}}^{\tilde{\eta}}d\eta'\omega_{k}(\eta')+\int_{\tilde{\eta}}^{\eta}d\eta'\omega_{k}(\eta')\right]}\right|\\
 & =\left|e^{-2i\int_{\eta_{i}}^{\tilde{\eta}}d\eta'\omega_{k}(\eta')}v\right|\numberthis\label{eq:betaeq}
\end{align*}
where $\tilde{\eta}$ is the pole of $\omega_{k}'(\eta)/\omega_{k}(\eta)$
and  $v$ is the part obtained from the steepest descent. The factor
in the integrand of Eq.~(\ref{eq:originalbeta}) is therefore
\begin{equation}
\frac{\omega'}{2\omega}\approx\frac{1}{4(\eta-\tilde{\eta})}
\end{equation}
which implies $v$ in eq.~(\ref{eq:betaeq}) is
\begin{equation}
v=\int_{-\infty}^{\infty}\frac{d\eta}{4(\eta-\tilde{\eta})}e^{-\frac{4}{3}im\sqrt{C'(\tilde{\eta})}(\eta-\tilde{\eta})^{3/2}}\label{eq:vexplic}
\end{equation}
where 
\begin{equation}
C(\eta)\equiv a^{2}(\eta).
\end{equation}
Deforming the integration contour as shown in Fig.~\ref{fig:The-original-contour}
allows us to rewrite this as
\begin{equation}
v=\int_{\mathcal{C}}\frac{d\eta}{4(\eta-\tilde{\eta})}e^{-\frac{4}{3}im\sqrt{C'(\tilde{\eta})}(\eta-\tilde{\eta})^{3/2}}
\end{equation}
where the $\mathcal{C}$ is the orange part of the contour in the
lower half plane. 

To define the contour, one must understand the complex values of $C'(\tilde{\eta})$.
To this end, let
\begin{equation}
-i\sqrt{C'(\tilde{\eta})}=U+iW
\end{equation}
where the imaginary part generically is nonvanishing. The branch points
are given by eqs.~(\ref{eq:branchpoints}) which gives
\begin{align}
C'(\tilde{\eta}) & =\frac{4a^{2}(\eta_{i})}{\eta_{i}}e^{\frac{3}{4}i(2l+1)\pi}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/2}
\end{align}
which says 
\begin{align*}
U+iW & =\frac{2a(\eta_{i})}{\sqrt{\eta_{i}}}e^{\frac{1}{8}i(6l-1)\pi}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/4}\\
 & =a^{3/2}(\eta_{i})\sqrt{2H(\eta_{i})}e^{\frac{1}{8}i(6l-1)\pi}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/4}.\numberthis
\end{align*}

To deform the contour, we need regions where the arcs with large radius
does not contribute to the integral. Note that if we define $\delta\equiv\eta-\tilde{\eta}=Re^{i\theta}$,
we have
\begin{equation}
\delta^{3/2}=R^{3/2}e^{i3\theta/2}=R^{3/2}\left(\cos\frac{3\theta}{2}+i\sin\frac{3\theta}{2}\right)
\end{equation}
making the exponent in $v$ 
\begin{equation}
-\frac{4}{3}im\sqrt{C'(\tilde{\eta})}(\eta-\tilde{\eta})^{3/2}=\frac{4}{3}mR^{3/2}(U+iW)\left(\cos\frac{3\theta}{2}+i\sin\frac{3\theta}{2}\right)
\end{equation}
which is damped only if 
\begin{equation}
U\cos(3\theta/2)-W\sin(3\theta/2)<0.
\end{equation}
For the case of Eq.~(\ref{eq:poleexpl}), we need 
\begin{equation}
\cos\left[\frac{\pi}{8}(6l-1)\right]\cos(3\theta/2)-\sin\left[\frac{\pi}{8}(6l-1)\right]\sin(3\theta/2)<0
\end{equation}
for one choice of $l$. For the choice of $l=3$, we can choose the
arc regions to be $\theta\in[\frac{-5\pi}{12},\frac{\pi}{4}]$ and
another arc region to be $\theta\in[\frac{11\pi}{12},\frac{19\pi}{12}]$
with a branch cut at $-5\pi/12$. 

Choosing $l=3$, we find the steepest descent contour shown in orange
in Fig.~\ref{fig:The-original-contour}. The left contour is $5\pi/4$
and the right contour is at $-\pi/12$, along which 
\begin{align*}
-\frac{4}{3}im\sqrt{C'(\tilde{\eta})}(\eta-\tilde{\eta})^{3/2} & =-\frac{4}{3}mR^{3/2}a^{3/2}(\eta_{i})\sqrt{2H(\eta_{i})}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/4}
\end{align*}
gives a damped exponential in eq.~(\ref{eq:vexplic}). Hence, the
integral is
\begin{align*}
v & =\frac{1}{4}\int_{\infty}^{\epsilon}\frac{dR}{R}e^{-\frac{4}{3}mR^{3/2}a^{3/2}(\eta_{i})\sqrt{2H_{e}}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/4}}+\frac{1}{4}\int_{\epsilon}^{\infty}\frac{dR}{R}e^{-\frac{4}{3}mR^{3/2}a^{3/2}(\eta_{i})\sqrt{2H_{e}}\left(\frac{k/a(\eta_{i})}{m}\right)^{3/4}}\nonumber\\
 & + \frac{1}{4}\int_{5\pi/4}^{-\pi/12}id\theta\exp\left[-\frac{4}{3}im\sqrt{C'(\tilde{\eta})}(\epsilon\, e^{i\theta})^{3/2}\right]\\
 & =\frac{i}{4}\left[\frac{-\pi}{12}-\frac{15\pi}{12}\right]=\frac{-i\pi}{3}\numberthis
\end{align*}
where in the first line we have introduced a regulator $\epsilon\rightarrow0$.

The final piece in eq.~(\ref{eq:betaeq}) is
\begin{align}
I & =e^{-2i\int_{\eta_{i}}^{\tilde{\eta}}d\eta'\omega_{k}(\eta')}.
\end{align}
Use the expansion 
\begin{align*}
I & =e^{-2i\int_{\eta_{i}}^{\tilde{\eta}}d\eta'\omega_{k}(\eta')}\\
 & =\exp\left(-2i\left[\Phi+J\right]\right)\numberthis
\end{align*}
where $\Phi$ is real and $J$ is purely imaginary. We take the path
to be along the real axis until $\eta=\Re\tilde{\eta}$ and then integrate
in the imaginary $\eta$ direction:
\begin{equation}
J=i\Im\int_{\Re\tilde{\eta}}^{\Re\tilde{\eta}+i\Im\tilde{\eta}}d\eta'\omega_{k}(\eta').
\end{equation}
 This gives
\begin{align}
J & \approx-i\frac{2}{3}\sqrt{2\pi}\frac{\Gamma(5/4)}{\Gamma(3/4)}\frac{(k/a(\eta_{i}))^{3/2}}{H(\eta_{i})\sqrt{m}}.
\end{align}
Now, note from Eq.~(\ref{eq:aHeq}), we can compute
\begin{align*}
\frac{1}{a_{e}^{3/2}} & =\frac{1}{a^{3/2}(\eta_{i})}\left[1+\frac{3}{2}H_{I}(t_{i}-t_{e})\right]\\
 & \approx\frac{1}{a^{3/2}(\eta_{i})}\frac{3}{2}H_{I}t_{i}\\
 & \approx\frac{1}{a^{3/2}(\eta_{i})}\frac{H_{I}}{H(\eta_{i})}\numberthis
\end{align*}
where we used Eq.~(\ref{eq:Hubble}). Eq.~(\ref{eq:betaeq}) then
becomes
\begin{equation}
\boxed{|\beta|\approx\frac{\pi}{3}\exp\left(-\frac{4}{3}\sqrt{2\pi}\frac{\Gamma(5/4)}{\Gamma(3/4)}\frac{(k/a_{e})^{3/2}}{H_{I}\sqrt{m}}\right)}.\label{eq:exampleresult}
\end{equation}

\newpage

\newpage

## Answer

$$
\boxed{|\beta|\approx\frac{\pi}{3}\exp\left(-\frac{4}{3}\sqrt{2\pi}\frac{\Gamma(5/4)}{\Gamma(3/4)}\frac{(k/a_{e})^{3/2}}{H_{I}\sqrt{m}}\right)}.
$$

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function.
\begin{python}
def abs_beta(k:float, a_e:float, m:float, H_I:float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from numpy import sqrt, exp, pi
from scipy.special import gamma
def abs_beta(k:float, a_e:float, m:float, H_I:float) -> float:    
    return pi/3*exp(-4/3*sqrt(2*pi)*gamma(5/4)*(k/a_e)**(3/2)/gamma(3/4)/H_I/sqrt(m))
\end{python}

\newpage

\newpage
