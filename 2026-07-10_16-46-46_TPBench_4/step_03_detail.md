# Step 3 — Compute the post-burn specific energy using $\epsilon=\frac{1}{2}(v_e+\delta v)^2-\frac{GM}{r_p}$ and substitute $\frac{GM}{r_p}=\frac{1}{2}v_e^2$ to obtain $\epsilon=v_e\delta v+\frac{1}{2}(\delta v)^2$.

## Solution Reasoning

Immediately after the impulsive burn, the probe is still at the same periapsis radius $r_p$, but its speed has increased from $v_e$ to $v_e+\delta v$. Therefore its specific mechanical energy is kinetic energy per unit mass minus gravitational potential energy per unit mass: $\epsilon = \frac{1}{2}(v_e+\delta v)^2 - GM/r_p$. Since the original orbit was parabolic, its pre-burn specific energy was zero, giving $\frac{1}{2}v_e^2 - GM/r_p=0$, or $GM/r_p=\frac{1}{2}v_e^2$. Substituting this into the post-burn energy and simplifying yields $\epsilon=v_e\delta v+\frac{1}{2}(\delta v)^2$.

## Result

The post-burn specific mechanical energy is

$$
\epsilon = \frac{1}{2}(v_e+\delta v)^2 - \frac{GM}{r_p}.
$$

Using the parabolic periapsis condition

$$
\frac{GM}{r_p}=\frac{1}{2}v_e^2,
$$

we obtain

$$
\epsilon = \frac{1}{2}(v_e+\delta v)^2 - \frac{1}{2}v_e^2.
$$

Expanding,

$$
\epsilon = \frac{1}{2}\left(v_e^2+2v_e\delta v+(\delta v)^2\right)-\frac{1}{2}v_e^2,
$$

so

$$
\boxed{\epsilon = v_e\delta v + \frac{1}{2}(\delta v)^2}.
$$

## Physical Interpretation

The post-burn specific mechanical energy is

$$
\epsilon = \frac{1}{2}(v_e+\delta v)^2 - \frac{GM}{r_p}.
$$

Using the parabolic periapsis condition

$$
\frac{GM}{r_p}=\frac{1}{2}v_e^2,
$$

we obtain

$$
\epsilon = \frac{1}{2}(v_e+\delta v)^2 - \frac{1}{2}v_e^2.
$$

Expanding,

$$
\epsilon = \frac{1}{2}\left(v_e^2+2v_e\delta v+(\delta v)^2\right)-\frac{1}{2}v_e^2,
$$

so

$$
\boxed{\epsilon = v_e\delta v + \frac{1}{2}(\delta v)^2}.
$$

**Consistency check:** passed
