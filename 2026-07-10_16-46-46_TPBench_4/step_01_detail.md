# Step 1 — Identify the parabolic periapsis condition: before the burn the probe has zero specific orbital energy, so at periapsis $\frac{1}{2}v_e^2-\frac{GM}{r_p}=0$, implying $\frac{GM}{r_p}=\frac{1}{2}v_e^2$.

## Solution Reasoning

For a Keplerian orbit in a Newtonian gravitational potential, the specific orbital energy is $\epsilon = \frac{1}{2}v^2 - GM/r$. A parabolic trajectory is the marginally bound case, so $\epsilon=0$. Evaluating this at periapsis, where the pre-burn speed is $v_e$ and the distance from the planet is $r_p$, gives $\frac{1}{2}v_e^2 - GM/r_p=0$. Rearranging yields $GM/r_p=\frac{1}{2}v_e^2$. This establishes the key relation needed to eliminate $GM/r_p$ later when computing the post-burn hyperbolic excess speed.

## Result

Before the burn, the probe is on a parabolic orbit, so its specific orbital energy is zero:

$$
\epsilon = \frac{1}{2}v_e^2 - \frac{GM}{r_p}=0.
$$

Therefore, at periapsis,

$$
\frac{GM}{r_p}=\frac{1}{2}v_e^2.
$$

Equivalently, the periapsis speed $v_e$ is the local escape speed at radius $r_p$:

$$
v_e = \sqrt{\frac{2GM}{r_p}}.
$$

## Physical Interpretation

Before the burn, the probe is on a parabolic orbit, so its specific orbital energy is zero:

$$
\epsilon = \frac{1}{2}v_e^2 - \frac{GM}{r_p}=0.
$$

Therefore, at periapsis,

$$
\frac{GM}{r_p}=\frac{1}{2}v_e^2.
$$

Equivalently, the periapsis speed $v_e$ is the local escape speed at radius $r_p$:

$$
v_e = \sqrt{\frac{2GM}{r_p}}.
$$

**Consistency check:** passed
