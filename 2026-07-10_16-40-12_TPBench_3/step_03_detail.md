# Step 3 — Use spherical momentum coordinates in $d$ dimensions and rescale $x=\beta \hbar c k$ to extract the temperature dependence: $$u \sim \int_0^\infty dk\, k^{d-1}\frac{\hbar c k}{e^{\beta \hbar c k}-1} \propto T^{d+1}.$$

## Solution Reasoning

The density of states in $d$ spatial dimensions contributes a factor $k^{d-1}$ from the spherical momentum-space volume element. Each photon mode has energy $\hbar \omega = \hbar c k$, giving an additional factor of $k$. Hence the integrand contains $k^d/(e^{\beta \hbar c k}-1)$. Rescaling the integration variable to the dimensionless combination $x=\beta \hbar c k$ pulls out a factor $(\beta \hbar c)^{-(d+1)}$. Since $\beta = 1/(k_B T)$, this gives $u \propto T^{d+1}$. The omitted constants only affect the prefactor, not the exponent.

## Result

Using spherical coordinates in $d$-dimensional momentum space, constants such as $S_{d-1}$, $(2\pi)^{-d}$, and polarization degeneracies do not affect the temperature scaling. Thus

$$u \sim \int_0^\infty dk\, k^{d-1}\frac{\hbar c k}{e^{\beta \hbar c k}-1} = \hbar c \int_0^\infty dk\, \frac{k^d}{e^{\beta \hbar c k}-1}.$$

Now rescale

$$x = \beta \hbar c k, \qquad k = \frac{x}{\beta \hbar c}, \qquad dk = \frac{dx}{\beta \hbar c}.$$

Then

$$u \sim \hbar c \int_0^\infty \frac{dx}{\beta \hbar c}\, \frac{\left(\frac{x}{\beta \hbar c}\right)^d}{e^x-1}.$$

Therefore

$$u \sim \frac{1}{(\beta \hbar c)^{d+1}}\,\hbar c \int_0^\infty dx\,\frac{x^d}{e^x-1}.$$

The remaining integral is dimensionless and independent of $T$, so the temperature dependence is

$$u \propto \beta^{-(d+1)} \propto T^{d+1}.$$

Thus, in $d$ spatial dimensions, the blackbody energy density scales as

$$u \propto T^{d+1}.$$

## Physical Interpretation

Using spherical coordinates in $d$-dimensional momentum space, constants such as $S_{d-1}$, $(2\pi)^{-d}$, and polarization degeneracies do not affect the temperature scaling. Thus

$$u \sim \int_0^\infty dk\, k^{d-1}\frac{\hbar c k}{e^{\beta \hbar c k}-1} = \hbar c \int_0^\infty dk\, \frac{k^d}{e^{\beta \hbar c k}-1}.$$

Now rescale

$$x = \beta \hbar c k, \qquad k = \frac{x}{\beta \hbar c}, \qquad dk = \frac{dx}{\beta \hbar c}.$$

Then

$$u \sim \hbar c \int_0^\infty \frac{dx}{\beta \hbar c}\, \frac{\left(\frac{x}{\beta \hbar c}\right)^d}{e^x-1}.$$

Therefore

$$u \sim \frac{1}{(\beta \hbar c)^{d+1}}\,\hbar c \int_0^\infty dx\,\frac{x^d}{e^x-1}.$$

The remaining integral is dimensionless and independent of $T$, so the temperature dependence is

$$u \propto \beta^{-(d+1)} \propto T^{d+1}.$$

Thus, in $d$ spatial dimensions, the blackbody energy density scales as

$$u \propto T^{d+1}.$$

**Consistency check:** passed
