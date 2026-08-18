# Plan

**步骤数：4**

---

### Step 1

**Description**: Identify the parabolic periapsis condition: before the burn the probe has zero specific orbital energy, so at periapsis $\frac{1}{2}v_e^2-\frac{GM}{r_p}=0$, implying $\frac{GM}{r_p}=\frac{1}{2}v_e^2$.

- **Needs computation**: No
- **Reasoning**: This follows directly from conservation of mechanical energy for a parabolic orbit; no symbolic computation is needed.

---

### Step 2

**Description**: Model the impulsive rocket burn at periapsis as an instantaneous tangential velocity change from $v_e$ to $v_e+\delta v$, while the radius remains $r_p$.

- **Needs computation**: No
- **Reasoning**: The problem states a very brief firing at periapsis; the standard impulse approximation is a conceptual step.

---

### Step 3

**Description**: Compute the post-burn specific energy using $\epsilon=\frac{1}{2}(v_e+\delta v)^2-\frac{GM}{r_p}$ and substitute $\frac{GM}{r_p}=\frac{1}{2}v_e^2$ to obtain $\epsilon=v_e\delta v+\frac{1}{2}(\delta v)^2$.

- **Needs computation**: No
- **Reasoning**: The algebra is simple enough to do by hand.

---

### Step 4

**Description**: Relate the positive post-burn energy to the asymptotic escape speed $v_\infty$ via $\epsilon=\frac{1}{2}v_\infty^2$, yielding $v_\infty=\sqrt{2v_e\delta v+(\delta v)^2}$.

- **Needs computation**: No
- **Reasoning**: This is a direct application of energy conservation at infinity where gravitational potential vanishes.

## Symmetries
- Central gravitational field of the planet
- Conservation of mechanical energy before and after the instantaneous burn, excluding the impulse itself
- Spherical symmetry of the potential $-GM/r$

## Approximations
- The rocket firing is instantaneous compared with orbital timescales
- The boost $\delta v$ is applied prograde along the periapsis velocity
- Planetary atmosphere, rotation, tidal effects, and other bodies are neglected
- Newtonian gravity is assumed

## Other Constraints
- Final answer must be expressed only in terms of $v_e$ and $\delta v$
- The periapsis radius $r_p$ and planet mass $M$ should cancel out using the parabolic condition