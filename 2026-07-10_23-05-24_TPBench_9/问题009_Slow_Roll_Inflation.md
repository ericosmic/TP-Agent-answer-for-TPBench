---
row_number: 9
csv_index: 8
problem_id: Slow-Roll Inflation
domain: Cosmology
difficulty_level: 3
---

# Slow-Roll Inflation

## Domain

Cosmology

## Difficulty Level

3

## Problem

For the action
\begin{equation}
S = \int dt a^3(t) \left\{ \frac{1}{2} \dot{\phi}^2 - V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] \right\}
\end{equation}
where \( q \) and \(V_0\) are constants, derive and solve (integrate) the equation of motion for the field $\phi$ assuming slow-roll inflation and initial condition $\phi(t=0) = \phi_0$.

## Solution

The equation of motion is
\begin{equation}
\ddot{\phi} + 3 H \dot{\phi} - \sqrt{\frac{2}{q}} \left( \frac{1}{M_P} \right) V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right] = 0.
\end{equation}
For the slow-roll inflation, the following must hold: 
\begin{equation}
    \ddot{\phi}\ll 3H\dot{\phi} \,.
\end{equation}
Hence, we have
\begin{equation}
3 H \dot{\phi} = \sqrt{\frac{2}{q}} \left( \frac{1}{M_P} \right) V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right].
\end{equation}
Slow-roll approximation also implies 
\begin{equation}
H^2\approx\frac{V(\phi)}{3M^2_P}
\end{equation}
so we need to solve the following ODE:
\begin{equation}
3 \sqrt{\frac{V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right]}{3 M_P^2}} \frac{d\phi}{dt} = \sqrt{\frac{2}{q}} \left( \frac{1}{M_P} \right) V_0 \exp \left[ - \sqrt{\frac{2}{q}} \left( \frac{\phi}{M_P} \right) \right]
\end{equation}

\begin{equation}
\int \frac{d\phi}{\sqrt{V_0}} \exp \left[ \sqrt{\frac{1}{2q}} \left( \frac{\phi}{M_P} \right) \right] = \sqrt{\frac{2}{3q}} t \,.
\end{equation}
Performing the integration and solving for $\phi(t)$ we get
\begin{equation}
\frac{1}{\sqrt{V_0}} M_P \sqrt{2q} \left( \exp \left[ \sqrt{\frac{1}{2q}} \left( \frac{\phi}{M_P} \right) \right] - \exp \left[ \sqrt{\frac{1}{2q}} \left( \frac{\phi_0}{M_P} \right) \right] \right) = \sqrt{\frac{2}{3q}} t
\end{equation}

\begin{equation}
\boxed{
\phi = \sqrt{2q} M_P \ln \left\{ \exp \left[ \sqrt{\frac{1}{2q}} \left( \frac{\phi_0}{M_P} \right) \right] + \frac{1}{M_P q} \sqrt{\frac{V_0}{3}} t \right\}}.
\end{equation}

## Answer

\[
\phi = \sqrt{2q} M_P \ln \left\{ \exp \left[ \sqrt{\frac{1}{2q}} \left( \frac{\phi_0}{M_P} \right) \right] + \frac{1}{M_P q} \sqrt{\frac{V_0}{3}} t \right\}.
\]

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function 
\begin{python}
import numpy as np
def phi(q: float, M_p: float, phi_0: float, V_0: float, t: np.ndarray)->np.ndarray:
    pass
\end{python}

## Reference Implementation

\begin{python}
import numpy as np
from numpy import sqrt, log, exp
def phi(q: float, M_p: float, phi_0: float, V_0: float, t: np.ndarray):
    answer = sqrt(2*q)*M_p*log(exp(sqrt(1/(2*q))*(phi_0/M_p))+1/(M_p*q)*sqrt(V_0/3)*t)
    return answer
\end{python}
\newpage

\newpage
