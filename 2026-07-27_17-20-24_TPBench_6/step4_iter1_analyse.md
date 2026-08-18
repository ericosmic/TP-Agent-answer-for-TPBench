# Analyse Step 4 Iteration 1

**Description:** Evaluate the WKB phase integral $S(k)=\int_{\eta_e}^{\tilde{\eta}}d\eta\,\omega_k(\eta)$ using the large-$k/(a_eH_I)$ expansion with $0<m\lesssim H_I$, keeping the leading non-analytic/exponential contribution that controls $|\beta(k)|$ and retaining only prefactors that survive the requested approximation accuracy.

## Decision

- Conditions complete: True
- Plan needs computation: False
- LLM needs computation: False
- Compute tool: none
- Disputes reflect: False

## Information Needed

The step is complete using prior results: the post-transition analytic scale factor $a(\eta)=a_e[1+(a_eH_I/2)(\eta-\eta_e)]^2$, the dominant turning point $\tilde\eta=\eta_e+\frac{2}{a_eH_I}[(k/(ma_e))^{1/2}e^{i\pi/4}-1]$, and $\omega_k^2=k^2+m^2a_e^2 z^4$ with $z=1+(a_eH_I/2)(\eta-\eta_e)$.

## Critical Rubrics

A correct answer must: (i) use the post-transition variable $z=1+(a_eH_I/2)(\eta-\eta_e)$; (ii) map the dominant pole to $z=\rho e^{i\pi/4}$ with $\rho=(k/(ma_e))^{1/2}$; (iii) rescale $z=\rho s$ and isolate the large-$\rho$ nonanalytic contribution; (iv) evaluate $\int_0^{e^{i\pi/4}}\sqrt{1+s^4}\,ds=e^{i\pi/4}\sqrt\pi\Gamma(1/4)/(6\Gamma(3/4))$; (v) recognize that the lower-limit correction $-2k/(a_eH_I)$ is real and irrelevant for $|\beta|$; and (vi) report the exponential control as $2|\operatorname{Im}S|=\frac{\sqrt{2\pi}\Gamma(1/4)}{3\Gamma(3/4)}\frac{k}{a_eH_I}(k/(ma_e))^{1/2}$ up to subleading corrections.

## Candidate Result

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

## Reasoning

The relevant phase integral lies entirely on the post-transition analytic continuation because the dominant turning point has positive real part. The natural variable $z=1+(a_eH_I/2)(\eta-\eta_e)$ maps the lower endpoint to $z=1$ and the turning point to $z=\rho e^{i\pi/4}$, where $\rho=(k/(ma_e))^{1/2}$. After the rescaling $z=\rho s$, the large-$k/(a_eH_I)$, $0<m\lesssim H_I$ limit corresponds to $\rho\gg1$ for the nonanalytic turning-point contribution. The integral from $0$ to $e^{i\pi/4}$ gives the complex nonanalytic contribution proportional to $k\rho/(a_eH_I)\sim k^{3/2}m^{-1/2}$, while the correction from replacing the lower limit $1/\rho$ by $0$ is real at leading order and hence does not contribute to the magnitude of $\beta(k)$. Evaluating the universal constant by the beta function gives $C=(1/4)B(1/4,3/2)=\sqrt\pi\Gamma(1/4)/(6\Gamma(3/4))$. Therefore only the imaginary part of the $e^{i\pi/4}C$ term controls the exponential suppression in the Bogoliubov coefficient.
