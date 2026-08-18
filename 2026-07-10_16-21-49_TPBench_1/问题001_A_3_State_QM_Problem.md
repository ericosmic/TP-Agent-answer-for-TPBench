---
row_number: 1
csv_index: 0
problem_id: A 3-State QM Problem
domain: QM
difficulty_level: 2
---

# A 3-State QM Problem

## Domain

QM

## Difficulty Level

2

## Problem

The Hamiltonian of a three-level system is given as $H = \begin{pmatrix}
    E_a & 0 & A \\
    0 & E_b & 0 \\
    A & 0 & E_a \\
\end{pmatrix}$ where $A$ is real. The state of the system at time $t=0$ is (in this basis) $\psi(t=0) = \frac{1}{\sqrt{2}}\begin{pmatrix}1 \\
1\\
0\end{pmatrix}$ What is the expectation value of the energy at time $t$?

## Solution

The eigenstates are easily found to be $\frac{1}{\sqrt{2}}(1,0,\pm 1)^T$ and $(0,1,0)^T$ with corresponding energies $E_a\pm A$, $E_b$. Let us denote them as $|1\rangle$, $|2\rangle$ and $|3\rangle$. Given state $\psi$ is decomposed as $\frac{1}{2}(|1\rangle +|2\rangle) + \frac{1}{\sqrt{2}}|3\rangle$, the expectation of energy stays constant: 
\begin{equation}
    \langle E\rangle = \frac{1}{4}((E_a+A)+(E_a-A)) + \frac{1}{2}E_b =\boxed{ \frac{1}{2}(E_a+E_b)}.
\end{equation}

## Answer

\begin{equation*}
    \boxed{\langle E\rangle = \frac{1}{2}(E_a+E_b)}
\end{equation*}

## Code Answer Requirements

Provide the answer in the form of \texttt{python} code. Implement the following function
\begin{python}
def expectation_value(A: float, E_a:float, E_b:float, t:float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
def expectation_value(A: float, E_a:float, E_b:float, t:float) -> float:
    return 0.5*(E_a+E_b)
\end{python}
