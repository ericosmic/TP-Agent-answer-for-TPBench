---
row_number: 3
csv_index: 2
problem_id: Blackbody in d Dimensions
domain: Stat Mech
difficulty_level: 1
---

# Blackbody in d Dimensions

## Domain

Stat Mech

## Difficulty Level

1

## Problem

Assume we live in a 4+1 dimensional spacetime. How does the total energy density of a black body scale with temperature T. Find the exponent $n$ in the expression $u \propto T^{n}$.

## Solution

The density of states scales as $k^{D-1}dk$ in D spatial dimensions giving 
$T^{D+1}$ scaling for the total energy density. Hence, $\boxed{n=5}.$

## Answer

$\boxed{n=5}.$

## Code Answer Requirements

Provide the answer in a form of \texttt{python} code. Implement the following function
\begin{python}
def answer() -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
def answer() -> float:
    return 5
\end{python}
