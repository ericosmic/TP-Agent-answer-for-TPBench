---
row_number: 5
csv_index: 4
problem_id: Dark Matter Capture as a Function of Time
domain: Cosmology
difficulty_level: 2
---

# Dark Matter Capture as a Function of Time

## Domain

Cosmology

## Difficulty Level

2

## Problem

Suppose $C$ is the capture rate of dark matter in an astrophysical
body. Let $C_{A}$ be the dark matter annihilation rate per effective
volume. Then an approximate Boltzmann equation governing the number
$N$ of dark matter particles in the astrophysical body is
\[
\frac{d N}{dt}=C-C_{A}N^{2}.
\]
If initially, $N(0)=0$, what is $N(t)$ as a function of time?

## Solution

We can integrate by quadrature.
\begin{equation}
\int\frac{dN}{C-C_{A}N^{2}}=t.
\end{equation}
We can express the integrand as a sum of two fractions:
\begin{align*}
\frac{1}{C-C_{A}N^{2}} & = \frac{1}{\sqrt{C}-\sqrt{C_{A}}N}\frac{1}{\sqrt{C}+\sqrt{C_{A}}N}\\
 & = \frac{1}{2\sqrt{C}}\left[\frac{1}{\sqrt{C}-\sqrt{C_{A}}N}+\frac{1}{\sqrt{C}+\sqrt{C_{A}}N}\right]\numberthis.
\end{align*}
Integrating, we find
\begin{align*}
t+K & = \frac{1}{2\sqrt{C}}\left[\frac{-1}{\sqrt{C_{A}}}\ln\left(\sqrt{C}-\sqrt{C_{A}}N\right)+\frac{1}{\sqrt{C_{A}}}\ln\left(\sqrt{C}+\sqrt{C_{A}}N\right)\right]\\
 & = \frac{1}{2\sqrt{C_{A}C}}\ln\left(\frac{\sqrt{C}+\sqrt{C_{A}}N}{\sqrt{C}-\sqrt{C_{A}}N}\right)\numberthis
\end{align*}
where $K$ is an integration constant. Setting the boundary condition
$N=0$ at $t=0$, we find
\[
K=0.
\]
We find the solution 
\begin{equation}
\boxed{N=\frac{\sqrt{C}}{\sqrt{C_{A}}}\frac{\left(e^{2\sqrt{C C_A}t}-1\right)}{\left(e^{2\sqrt{C C_A}t}+1\right)}}.
\end{equation}
Note that it is easy to check that it reaches the obvious steady state
in the limit $t\rightarrow\infty$.

## Answer

$$
\boxed{N=\frac{\sqrt{C}}{\sqrt{C_{A}}}\frac{\left(e^{2\sqrt{C C_A}t}-1\right)}{\left(e^{2\sqrt{C C_A}t}+1\right)}}.
$$

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function.
\begin{python}
def answer(C: float, C_A: float, t: float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from math import sqrt, exp

def answer(C: float, C_A: float, t: float) -> float:
    return sqrt(C/C_A) * (
        (exp(2*sqrt(C*C_A)*t) - 1)
        / (exp(2*sqrt(C*C_A)*t) + 1)
    )
\end{python}

\newpage

\newpage
