# Step 6 — Insert $\nu$ into the one-mode Gaussian entropy formula $S=\left(\nu+\frac{1}{2}\right)\ln\left(\nu+\frac{1}{2}\right)-\left(\nu-\frac{1}{2}\right)\ln\left(\nu-\frac{1}{2}\right)$ and express the result in terms of $k$, $g$, and $m$, noting that $m$ cancels through the ratio $\omega_{-}/\omega_{+}=\sqrt{1+2g/k}$.

## Solution Reasoning

The entropy of a single-mode Gaussian state depends only on the symplectic eigenvalue $\nu$. From the covariance calculation, $\nu=(\omega_++\omega_-)/(4\sqrt{\omega_+\omega_-})$. Dividing numerator and denominator by $\omega_+$ shows that only the ratio $r=\omega_-/\omega_+$ enters: $\nu=(1+r)/(4\sqrt r)$. Since $\omega_+=\sqrt{k/m}$ and $\omega_- = \sqrt{(k+2g)/m}$, their ratio is $r=\sqrt{(k+2g)/k}=\sqrt{1+2g/k}$, so $m$ cancels. Then $\nu\pm 1/2$ simplify to $((\sqrt r\pm 1)^2)/(4\sqrt r)$, and substitution into $S=(\nu+1/2)\ln(\nu+1/2)-(\nu-1/2)\ln(\nu-1/2)$ yields the final expression.

## Result

Let
$$r\equiv \frac{\omega_-}{\omega_+}=\sqrt{1+\frac{2g}{k}}.$$
Then
$$\nu=\frac{1}{4}\frac{\omega_++\omega_-}{\sqrt{\omega_+\omega_-}}=\frac{1}{4}\frac{1+r}{\sqrt r}=\frac{1}{4}\left(\sqrt r+\frac{1}{\sqrt r}\right).$$
Therefore
$$\nu+\frac{1}{2}=\frac{(\sqrt r+1)^2}{4\sqrt r},\qquad \nu-\frac{1}{2}=\frac{(\sqrt r-1)^2}{4\sqrt r}.$$
Inserting into the one-mode Gaussian entropy formula gives
$$\boxed{S=\frac{(\sqrt r+1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r+1)^2}{4\sqrt r}\right]-\frac{(\sqrt r-1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r-1)^2}{4\sqrt r}\right]}$$
with
$$r=\sqrt{1+\frac{2g}{k}}.$$
Equivalently, defining
$$a\equiv \sqrt r=\left(1+\frac{2g}{k}\right)^{1/4},$$
one may write
$$\boxed{S=\frac{(a+1)^2}{4a}\ln\left[\frac{(a+1)^2}{4a}\right]-\frac{(a-1)^2}{4a}\ln\left[\frac{(a-1)^2}{4a}\right],\qquad a=\left(1+\frac{2g}{k}\right)^{1/4}.}$$
The mass $m$ has cancelled, as expected. For $g=0$, $a=1$, so $\nu=1/2$ and $S=0$, corresponding to an unentangled product vacuum.

## Physical Interpretation

Let
$$r\equiv \frac{\omega_-}{\omega_+}=\sqrt{1+\frac{2g}{k}}.$$
Then
$$\nu=\frac{1}{4}\frac{\omega_++\omega_-}{\sqrt{\omega_+\omega_-}}=\frac{1}{4}\frac{1+r}{\sqrt r}=\frac{1}{4}\left(\sqrt r+\frac{1}{\sqrt r}\right).$$
Therefore
$$\nu+\frac{1}{2}=\frac{(\sqrt r+1)^2}{4\sqrt r},\qquad \nu-\frac{1}{2}=\frac{(\sqrt r-1)^2}{4\sqrt r}.$$
Inserting into the one-mode Gaussian entropy formula gives
$$\boxed{S=\frac{(\sqrt r+1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r+1)^2}{4\sqrt r}\right]-\frac{(\sqrt r-1)^2}{4\sqrt r}\ln\left[\frac{(\sqrt r-1)^2}{4\sqrt r}\right]}$$
with
$$r=\sqrt{1+\frac{2g}{k}}.$$
Equivalently, defining
$$a\equiv \sqrt r=\left(1+\frac{2g}{k}\right)^{1/4},$$
one may write
$$\boxed{S=\frac{(a+1)^2}{4a}\ln\left[\frac{(a+1)^2}{4a}\right]-\frac{(a-1)^2}{4a}\ln\left[\frac{(a-1)^2}{4a}\right],\qquad a=\left(1+\frac{2g}{k}\right)^{1/4}.}$$
The mass $m$ has cancelled, as expected. For $g=0$, $a=1$, so $\nu=1/2$ and $S=0$, corresponding to an unentangled product vacuum.

**Consistency check:** passed
