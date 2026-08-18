---
row_number: 4
csv_index: 3
problem_id: Boosted Parabolic Trajectory
domain: Classical Mechanics
difficulty_level: 1
---

# Boosted Parabolic Trajectory

## Domain

Classical Mechanics

## Difficulty Level

1

## Problem

Consider a situation where a space-probe very briefly fires its rockets while passing a planet of mass \(M\) at periapsis, its nearest point to the planet. Suppose that the probe is on a parabolic trajectory and at periapsis, when travelling at velocity $v_e$, it results in a boost of $\delta v$. What will be its speed once it escapes the planet's gravitational field only in terms of $v_e$ and $\delta v$?

## Solution

Conservation of energy gives $\frac{1}{2}m(v_e+\delta v)^2-\frac{mMG}{r_p} = \frac{1}{2}mv^2_\infty$. We also know that $\frac{1}{2}m(v_e)^2-\frac{mMG}{r_p} = E = 0$ for the parabolic trajectory. We can solve for $v_e$: $v_e = \sqrt{\frac{2MG}{r_p}}$. Then we can substitute it in the first equation and get:
\begin{equation}
\boxed{v_\infty = \delta v\sqrt{1+\frac{2v_e}{\delta v}}}.
\end{equation}

## Answer
$$
\begin{equation*}
    \boxed{v_\infty = \delta v\sqrt{1+\frac{2v_e}{\delta v}}}
\end{equation*}
$$
## Code Answer Requirements

Provide the answer in the form of \texttt{python} code. Implement the following function
\begin{python}
def speed(v_e: float, delta_v:float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from math import sqrt
def speed(v_e: float, delta_v:float) -> float:
    return delta_v*sqrt(1+2*v_e/delta_v)
\end{python}
