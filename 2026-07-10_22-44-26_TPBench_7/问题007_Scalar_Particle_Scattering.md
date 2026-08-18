---
row_number: 7
csv_index: 6
problem_id: Scalar Particle Scattering
domain: HET
difficulty_level: 3
---

# Scalar Particle Scattering

## Domain

HET

## Difficulty Level

3

## Problem

Consider
$$
\begin{equation}
\mathcal{L} = \left\{ \sum_{i=1}^2 \left[ \frac{1}{2} (\partial_\mu \phi_i)(\partial^\mu \phi_i) - \frac{m_i^2}{2} \phi_i \phi_i \right] - \frac{\lambda}{4} \phi_1^2 \phi_2^2 \right\}
\end{equation}
$$
What is the differential cross section \( \frac{d\sigma}{d\Omega} \) for \( \phi_1 (\vec{k}_1) \phi_1 (-\vec{k}_1) \to \phi_2 (\vec{k}_1') \phi_2 (-\vec{k}_1') \) in the CM frame accurate to \( O(\lambda^2) \)? Express your final answer in terms of Mandelstam variables.

## Solution

\textbf{Detailed Steps:}
The amplitude for this process is
\begin{equation}
i \mathcal{M} = -4 i \frac{\lambda}{4} = -i \lambda
\end{equation}
In the CM frame, energy conservation gives
\begin{equation}
2 \sqrt{|\vec{k}_1|^2 + m_1^2} = 2 \sqrt{|\vec{k}_1'|^2 + m_2^2}
\end{equation}
A standard formula for differential cross section gives
\begin{align*}
\left( \frac{d\sigma}{d\Omega} \right)_{\text{CM}} &= \frac{1}{64 \pi^2 s} \frac{k_1'}{k_1} |\mathcal{M}|^2 \\
&= \frac{\lambda^2}{64 \pi^2 s} \frac{\sqrt{|\vec{k}_1|^2 + (m_1^2 - m_2^2)}}{k_1} \numberthis
\end{align*}
Since in the CM frame, we know
\begin{equation}
k_1 = \frac{1}{2 \sqrt{s}} \sqrt{s^2 - 4 m_1^2 s}
\end{equation}
\begin{align*}
\left( \frac{d\sigma}{d\Omega} \right)_{\text{CM}} &= \frac{2 \sqrt{s}}{64 \pi^2 s} \sqrt{\frac{1}{4s} \left[ s^2 - 4 m_1^2 s \right] + (m_1^2 - m_2^2)} \frac{\lambda^2}{\sqrt{s^2 - 4 m_1^2 s}} \\
&= \frac{\lambda^2}{64 \pi^2 s} \frac{\sqrt{s^2 - 4 m_1^2 s + 4s(m_1^2 - m_2^2)}}{\sqrt{s^2 - 4 m_1^2 s}}.\numberthis
\end{align*}

The final result is
\begin{equation}
\boxed{
\left( \frac{d\sigma}{d\Omega} \right)_{\text{CM}}
= \frac{\lambda^2}{64 \pi^2 s} \frac{\sqrt{s - 4 m_2^2}}{\sqrt{s - 4 m_1^2}}
}.
\end{equation}

## Answer

\[
\left( \frac{d\sigma}{d\Omega} \right)_{\text{CM}} = \frac{\lambda^2}{64 \pi^2 s} \frac{\sqrt{s - 4 m_2^2}}{\sqrt{s - 4 m_1^2}}
\]

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function.
\begin{python}
def dsigma_domega(lam: float, s_m: float, p_m: float, u_m: float, 
                  m1: float, m2: float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from math import sqrt, pi
def dsigma_domega(lam: float, s_m: float, p_m: float, u_m: float, m1: float, m2: float) -> float:
    return lam**2/(64*pi**2*s_m)*sqrt(s_m-4 * m2**2)/sqrt(s_m-4*m1**2)
\end{python}

\newpage
