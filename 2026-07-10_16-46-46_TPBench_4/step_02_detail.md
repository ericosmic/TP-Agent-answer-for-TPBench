# Step 2 — Model the impulsive rocket burn at periapsis as an instantaneous tangential velocity change from $v_e$ to $v_e+\delta v$, while the radius remains $r_p$.

## Solution Reasoning

An impulsive burn is assumed to occur over a time interval short enough that the spacecraft's position is effectively unchanged, so the gravitational potential term remains evaluated at $r_p$. Since the burn is tangential and aligned with the instantaneous velocity, the velocity vectors add collinearly: the original velocity magnitude $v_e$ becomes $v_e+\delta v$. This step does not yet require solving the full escape speed at infinity; it only establishes the post-burn initial condition and post-burn specific energy expression.

## Result

Because the burn is very brief, it may be modeled as an impulse applied at fixed radius $r_p$. Since the boost is tangential and in the direction of motion, the post-burn periapsis speed is simply

$$
v_p^+ = v_e + \delta v.
$$

The radius during the burn remains

$$
r^+ = r_p.
$$

Thus, immediately after the burn, the probe is at periapsis radius $r_p$ with velocity magnitude $v_e+\delta v$. Its post-burn specific mechanical energy is therefore set up as

$$
\epsilon^+ = \frac{1}{2}(v_e+\delta v)^2 - \frac{GM}{r_p}.
$$

Using the parabolic condition from Step 1, $GM/r_p = \frac{1}{2}v_e^2$, this can later be written entirely in terms of $v_e$ and $\delta v$ as

$$
\epsilon^+ = \frac{1}{2}(v_e+\delta v)^2 - \frac{1}{2}v_e^2.
$$

## Physical Interpretation

Because the burn is very brief, it may be modeled as an impulse applied at fixed radius $r_p$. Since the boost is tangential and in the direction of motion, the post-burn periapsis speed is simply

$$
v_p^+ = v_e + \delta v.
$$

The radius during the burn remains

$$
r^+ = r_p.
$$

Thus, immediately after the burn, the probe is at periapsis radius $r_p$ with velocity magnitude $v_e+\delta v$. Its post-burn specific mechanical energy is therefore set up as

$$
\epsilon^+ = \frac{1}{2}(v_e+\delta v)^2 - \frac{GM}{r_p}.
$$

Using the parabolic condition from Step 1, $GM/r_p = \frac{1}{2}v_e^2$, this can later be written entirely in terms of $v_e$ and $\delta v$ as

$$
\epsilon^+ = \frac{1}{2}(v_e+\delta v)^2 - \frac{1}{2}v_e^2.
$$

**Consistency check:** passed
