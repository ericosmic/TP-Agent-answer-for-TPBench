---
row_number: 10
csv_index: 9
problem_id: SUSY-Symmetry
domain: HET
difficulty_level: 4
---

## Solution

Denoting the variation $\left(\delta_{\eta}\phi\right)^{\dagger}$
as $\delta_{\eta}\bar{\phi}$, we write 
\begin{align*}
\delta_{\eta}\mathcal{L} & = i\delta_{\eta}\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}\xi+i\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}\delta_{\eta}\xi+\partial_{\mu}\delta_{\eta}\bar{\phi}\partial^{\mu}\phi+\partial_{\mu}\bar{\phi}\partial^{\mu}\delta_{\eta}\phi-\delta_{\eta}\bar{F}F-\bar{F}\delta_{\eta}F\\
 & = i[-i\sqrt{2}\eta\sigma^{\beta}\partial_{\beta}\bar{\phi}+\cancel{\sqrt{2}\bar{\eta}\bar{F}}]\bar{\sigma}^{\mu}\partial_{\mu}\xi+i\bar{\xi}\bar{\sigma}^{\mu}\partial_{\mu}[i\sqrt{2}\sigma^{\beta}\bar{\eta}\partial_{\beta}\phi+\sqrt{2}\eta F]\\
 & +\partial_{\mu}\delta_{\eta}\bar{\phi}\partial^{\mu}\phi+\partial_{\mu}\bar{\phi}\partial^{\mu}\delta_{\eta}\phi-[-i\sqrt{2}\partial_{\mu}\bar{\xi}\bar{\sigma}^{\mu}\eta]F-\cancel{\bar{F}[i\sqrt{2}\bar{\eta}\bar{\sigma}^{\mu}\partial_{\mu}\xi]}\,.\numberthis
\end{align*}
Integrating by parts, we find (denoting with equality an equivalence
up to total derivative terms)
\begin{align}
\delta_{\eta}\mathcal{L} & =\sqrt{2}\eta\sigma^{\beta}\partial_{\beta}\bar{\phi}\bar{\sigma}^{\mu}\partial_{\mu}\xi+\partial_{\mu}\bar{\xi}\bar{\sigma}^{\mu}[\sqrt{2}\sigma^{\beta}\bar{\eta}\partial_{\beta}\phi-\cancel{i\sqrt{2}\eta F}]\nonumber \\
 & +\partial_{\mu}\delta_{\eta}\bar{\phi}\partial^{\mu}\phi+\partial_{\mu}\bar{\phi}\partial^{\mu}\delta_{\eta}\phi+\cancel{i\sqrt{2}\partial_{\mu}\bar{\xi}\bar{\sigma}^{\mu}\eta F} \,.
\end{align}
Integrate by parts the first two terms to eliminate the the $\sigma$
matrices using the identity $\bar{\sigma}^{\mu}\sigma^{\nu}+\bar{\sigma}^{\nu}\sigma^{\mu}=2g^{\mu\nu}$:
\begin{align}
\delta_{\eta}\mathcal{L} & =\sqrt{2}\left(\eta\partial_{\mu}\bar{\phi}\partial^{\mu}\xi+\partial^{\mu}\bar{\xi}\bar{\eta}\partial_{\mu}\phi\right)\nonumber \\
 & +\partial_{\mu}\delta_{\eta}\bar{\phi}\partial^{\mu}\phi+\partial_{\mu}\bar{\phi}\partial^{\mu}\delta_{\eta}\phi
\end{align}
again denoting with equality an equivalence up to total derivative
terms, and we are using the standard notation $\eta\xi\equiv\eta^{\alpha}\xi_{\alpha}$
and $\bar{\xi}_{\dot{\alpha}}\bar{\eta}^{\dot{\alpha}}\equiv\bar{\xi}\bar{\eta}$.
To make the remainder cancel, we solve
\begin{equation}
\sqrt{2}\eta\partial_{\mu}\bar{\phi}\partial^{\mu}\xi+\partial_{\mu}\bar{\phi}\partial^{\mu}\delta_{\eta}\phi=0
\end{equation}
yielding
\begin{equation}
\boxed{\delta_{\eta}\phi=-\sqrt{2}\eta\xi,\quad\left(\delta_{\eta}\phi\right)^{\dagger}=-\sqrt{2}\bar{\xi}\bar{\eta}}.\label{eq:L4-susy}
\end{equation}

## Answer

\begin{equation}
\boxed{\delta_{\eta}\phi=-\sqrt{2}\eta\xi,\quad\left(\delta_{\eta}\phi\right)^{\dagger}=-\sqrt{2}\bar{\xi}\bar{\eta}}.\label{eq:L4-susy}
\end{equation}

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function 
\begin{python}
from math import sqrt
def find_delta_phi(eta:float, xi:float, bar_eta:float, bar_xi:float) -> Tuple[float, float]:
    """
    Returns the SUSY transformation rules for phi and its Hermitian conjugate: 
    a tuple (delta_phi, delta_phi_dagger)
    """
    pass
\end{python}

## Reference Implementation

\begin{python}
from math import sqrt
def find_delta_phi(eta:float, xi:float, bar_eta:float, bar_xi:float):
    """
    Returns the SUSY transformation rules for phi and its Hermitian conjugate
    
    Returns
    -------
    A tuple (delta_phi, delta_phi_dagger)
    """

    delta_phi = -sqrt(2)*eta*xi
    delta_phi_dagger = -sqrt(2)*bar_xi*bar_eta

    return (delta_phi, delta_phi_dagger)
\end{python}
\newpage
