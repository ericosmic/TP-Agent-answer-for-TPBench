# Step 3 — Insert the relevant analytic branch of $a(\eta)$ into $\omega_{k}(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$ and find the dominant singularity $\tilde{\eta}$ of $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ from $\omega_{k}^{2}(\tilde{\eta})=0$, selecting the pole or turning point with $\Re\tilde{\eta}>0$ that gives the smallest positive suppression in the limit $k/(a_{e}H_{I})\rightarrow\infty$.

## Solution Reasoning

The post-transition branch is the correct analytic branch because the requested singularity has $\Re\tilde\eta>0$, while the transition has been placed at $\eta_e=0$. Substituting $a(\eta)=a_e(1+A\eta/2)^2$ into $\omega_k^2$ gives a quartic equation in $z=1+A\eta/2$. The zeros of $\omega_k^2$ are branch points of $\omega_k$ and therefore singularities of $\omega_k'/(2\omega_k)$. Solving $z^4=-q^2$ gives four roots separated by $\pi/2$. At large $q=k/(ma_e)$, the roots with phases $\pm\pi/4$ have positive real part, while those with phases $3\pi/4$ and $5\pi/4$ have negative real part. The integral contains $e^{-2i\int\omega d\eta}$, so the damped steepest-descent contour is reached through the lower-half plane; thus the root with phase $-\pi/4$ is selected as the dominant singularity for the one-pole approximation. Since $m\lesssim H_I$ and $k/(a_eH_I)\to\infty$, one has $q\to\infty$, ensuring $\Re\tilde\eta>0$.

## Result

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

## Physical Interpretation

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

**Consistency check:** passed
