# Step 2 — Write the scaling form of the photon/gauge-boson thermal energy density in $d$ spatial dimensions: $$u \sim \int \frac{d^d k}{(2\pi)^d}\, \frac{\hbar \omega}{e^{\beta \hbar \omega}-1}, \qquad \omega = c|\mathbf{k}|.$$

## Solution Reasoning

The energy density is obtained by summing the average energy per mode over all momentum modes. For a massless photon or gauge boson, the energy of a mode is $\hbar \omega = \hbar c k$, and the Bose-Einstein occupation number is $(e^{\beta \hbar \omega}-1)^{-1}$. In d spatial dimensions, the momentum-space measure is $d^d k/(2\pi)^d$. By rotational symmetry, the angular integration contributes only a dimensionless factor $S_{d-1}$, leaving the radial integral proportional to $\int_0^\infty dk\, k^{d-1}$. Multiplying by the mode energy $\hbar c k$ gives the integrand proportional to $k^d/(e^{\beta \hbar c k}-1)$. This step sets up the scaling integral; the temperature scaling follows in the next step by changing variables to $x = \beta \hbar c k$.

## Result

For massless photons or gauge bosons in d spatial dimensions, the thermal energy density has the scaling form

$$u \sim \int \frac{d^d k}{(2\pi)^d}\, \frac{\hbar \omega}{e^{\beta \hbar \omega}-1}, \qquad \omega = c |\mathbf{k}|.$$

Using rotational symmetry in momentum space,

$$d^d k = S_{d-1} k^{d-1} dk,$$

where $S_{d-1}$ is the area of the unit $(d-1)$-sphere. Therefore,

$$u \sim \int_0^\infty dk\, k^{d-1}\, \frac{\hbar c k}{e^{\beta \hbar c k}-1}.$$

Equivalently,

$$u \sim \hbar c \int_0^\infty dk\, \frac{k^d}{e^{\beta \hbar c k}-1}.$$

Up to dimensionless constants and polarization degeneracy factors, this is the desired d-dimensional scaling form.

## Physical Interpretation

For massless photons or gauge bosons in d spatial dimensions, the thermal energy density has the scaling form

$$u \sim \int \frac{d^d k}{(2\pi)^d}\, \frac{\hbar \omega}{e^{\beta \hbar \omega}-1}, \qquad \omega = c |\mathbf{k}|.$$

Using rotational symmetry in momentum space,

$$d^d k = S_{d-1} k^{d-1} dk,$$

where $S_{d-1}$ is the area of the unit $(d-1)$-sphere. Therefore,

$$u \sim \int_0^\infty dk\, k^{d-1}\, \frac{\hbar c k}{e^{\beta \hbar c k}-1}.$$

Equivalently,

$$u \sim \hbar c \int_0^\infty dk\, \frac{k^d}{e^{\beta \hbar c k}-1}.$$

Up to dimensionless constants and polarization degeneracy factors, this is the desired d-dimensional scaling form.

**Consistency check:** passed
