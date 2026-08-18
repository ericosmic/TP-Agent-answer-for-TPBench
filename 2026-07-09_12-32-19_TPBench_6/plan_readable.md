# Plan

**步骤数：5**

---

### Step 1

**Description**: Derive the physical scale factor from $\frac{d}{dt}\ln a=\Theta(t_{e}-t)H_{I}+\Theta(t-t_{e})\frac{H_{I}}{1+\frac{3}{2}H_{I}(t-t_{e})}$ with $a|_{t=t_{e}}=a_{e}$, then convert to conformal time using $t=t_{e}+\int_{\eta_{e}}^{\eta}a(y)dy$, choosing $\eta_{e}=0$ if convenient. Track continuity of $a$ and $a'$ at $t=t_{e}$ and identify the nonanalyticity in higher derivatives caused by the sudden transition.

- **Needs computation**: No
- **Reasoning**: The integrations are elementary, but the smoothness class of $a(\eta)$ must be identified because it controls the ultraviolet behavior.

---

### Step 2

**Description**: Before applying the one-pole contour estimate, impose a UV-consistent prescription: verify whether the sharp $\Theta$ transition produces a power-law high-$k$ tail in $|\beta(k)|$ from discontinuities of derivatives of $a(\eta)$, and either include the corresponding boundary contribution or state that a smoothed/adiabatic transition is assumed so that the one-pole exponential result is meaningful and avoids a UV catastrophe in $\int d^{3}k\,|\beta(k)|^{2}$ or $\int d^{3}k\,\omega_{k}|\beta(k)|^{2}$.

- **Needs computation**: No
- **Reasoning**: This is a conceptual and asymptotic consistency check; a discontinuous or insufficiently smooth background can dominate the high-$k$ limit and invalidate the pure one-pole estimate.

---

### Step 3

**Description**: Insert the relevant analytic branch of $a(\eta)$ into $\omega_{k}(\eta)=\sqrt{k^{2}+m^{2}a^{2}(\eta)}$ and find the dominant singularity $\tilde{\eta}$ of $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ from $\omega_{k}^{2}(\tilde{\eta})=0$, selecting the pole or turning point with $\Re\tilde{\eta}>0$ that gives the smallest positive suppression in the limit $k/(a_{e}H_{I})\rightarrow\infty$.

- **Needs computation**: No
- **Reasoning**: Once $a(\eta)$ is known, the turning-point condition is algebraic and the large-$k/(a_{e}H_{I})$ limit is analytically accessible.

---

### Step 4

**Description**: Evaluate the local one-pole contribution by expanding $\omega_{k}'(\eta)/(2\omega_{k}(\eta))$ near $\tilde{\eta}$ and combine it with the steepest-descent phase $\exp\left[-2i\int_{\eta_{e}}^{\tilde{\eta}}d\eta'\,\omega_{k}(\eta')\right]$, retaining the leading magnitude and discarding irrelevant phases.

- **Needs computation**: No
- **Reasoning**: The residue or local branch-point prefactor and the leading complex WKB action can be obtained by hand in the asymptotic regime.

---

### Step 5

**Description**: Compare the one-pole exponential contribution with any UV boundary or sudden-transition contribution found earlier; report the dominant UV-safe expression for $|\beta(k)|$ and explicitly state the condition under which it avoids UV catastrophe, for example exponential suppression from an analytic or sufficiently smooth transition versus unacceptable power-law behavior from the sharp $\Theta$ idealization.

- **Needs computation**: No
- **Reasoning**: The final answer must not only give the one-pole result but also verify convergence of the particle number and energy integrals in the ultraviolet.

## Symmetries
- Spatial homogeneity and isotropy conserve comoving momentum $\vec{k}$.
- Conformal coupling cancels the explicit curvature term in the rescaled mode equation, leaving $\omega_{k}^{2}(\eta)=k^{2}+m^{2}a^{2}(\eta)$.
- The result depends only on $k=|\vec{k}|$ because of rotational invariance.

## Approximations
- $k/(a_{e}H_{I})\rightarrow\infty$.
- $0<m\lesssim H_{I}$.
- Retain only the dominant singularity $\tilde{\eta}$ with $\Re\tilde{\eta}>0$ after checking UV boundary terms.
- The one-pole exponential estimate is valid only if the transition is analytic or sufficiently smooth so that nonadiabatic boundary terms do not dominate the UV tail.
- For finite particle number require sufficiently fast decay of $|\beta(k)|$ so that $\int d^{3}k\,|\beta(k)|^{2}$ converges; for finite energy require convergence of $\int d^{3}k\,\omega_{k}|\beta(k)|^{2}$.

## Other Constraints
- Use the boundary condition $a|_{t=t_{e}}=a_{e}$.
- Respect the step-function convention $\Theta(t-t_{e})=1$ for $t\geq t_{e}$ and $0$ otherwise.
- Choose the analytic continuation of $a(\eta)$ consistently with the real physical branch.
- Do not present a pure one-pole exponential answer without addressing the sharp-transition UV tail.
- Since $|\beta(k)|$ is requested, phases that do not affect the magnitude may be discarded only after the UV consistency check.