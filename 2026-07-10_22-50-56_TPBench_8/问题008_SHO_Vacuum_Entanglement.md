---
row_number: 8
csv_index: 7
problem_id: SHO Vacuum Entanglement
domain: QM
difficulty_level: 4
---

# SHO Vacuum Entanglement

## Domain

QM

## Difficulty Level

4

## Problem

Consider a coupled simple harmonic oscillator governed by the Hamiltonian
\begin{align}
H & =\sum_{i=1}^{2}\frac{1}{2}\left(\frac{p_{i}^{2}}{m}+kx_{i}^{2}\right)+g\frac{(x_{1}-x_{2})^{2}}{2}.
\end{align}
If the ground state is $|\Omega\rangle$ and the operator $\hat{\rho}$
is the vacuum density matrix partially traced over the $|w\rangle_{x_{2}}$
components (satisfying $\hat{x}_{2}|w\rangle_{x_{2}}=w|w\rangle_{x_{2}}$),
i.e.
\begin{equation}
\hat{\rho}\equiv\int dx_{1}''\int dx_{1}'\int dw\left(|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}''|\otimes\,_{x_{2}}\langle w|\right)\left(|\Omega\rangle\langle\Omega|\right)\left(|x_{1}'\rangle_{x_{1}}\otimes|w\rangle_{x_{2}}\,_{x_{1}}\langle x_{1}'|\right)
\end{equation}
which is an operator acting on a reduced Hilbert space, compute 
\begin{equation}
S\equiv-\mathrm{Tr}_{x_{1}}\left[\hat{\rho}\ln\hat{\rho}\right]
\end{equation}
which involves the trace over $x_{1}$ states.

## Solution

Diagonalize the original Hamiltonian 
\begin{align}
H & =(x_{1}\quad x_{2}\quad p_{1}\quad p_{2})\left(\begin{array}{cccc}
\frac{k+g}{2} & -\frac{g}{2}\\
-\frac{g}{2} & \frac{k+g}{2}\\
 &  & \frac{1}{2m}\\
 &  &  & \frac{1}{2m}
\end{array}\right)\left(\begin{array}{c}
x_{1}\\
x_{2}\\
p_{1}\\
p_{2}
\end{array}\right).
\end{align}
One easily finds
\begin{equation}
x_{1}=\frac{y_{1}+y_{2}}{\sqrt{2}}\label{eq:x1}
\end{equation}
\begin{equation}
x_{2}=\frac{y_{1}-y_{2}}{\sqrt{2}}\label{eq:x2}
\end{equation}
diagonalizes the Hamiltonian such that in the $(y_{1},y_{2},q_{1}\equiv m\dot{y}_{1},q_{2}\equiv m\dot{y}_{2})$
basis, it is
\begin{align}
H & =(y_{1}\quad y_{2}\quad q_{1}\quad q_{2})\left(\begin{array}{cccc}
\frac{k}{2} & 0\\
0 & \frac{k}{2}+g\\
 &  & \frac{1}{2m}\\
 &  &  & \frac{1}{2m}
\end{array}\right)\left(\begin{array}{c}
y_{1}\\
y_{2}\\
q_{1}\\
q_{2}
\end{array}\right).
\end{align}
The ladder operators are
\begin{equation}
a_{j}=\frac{1}{\sqrt{2}}\left(\sqrt{m\omega_{j}}y_{j}+\frac{i}{\sqrt{m\omega_{j}}}q_{j}\right)
\end{equation}
\begin{equation}
\omega_{1}^{2}=\frac{k}{m}\,\,\,\,\,\,\,\,\omega_{2}^{2}=\frac{k+2g}{m}
\end{equation}
which allows one to rewrite the Hamiltonian as
\begin{equation}
H=\sum_{j=1}^{2}a_{j}^{\dagger}a_{j}\omega_{j}+\frac{\omega_{1}+\omega_{2}}{2}.
\end{equation}
In this basis, we denote the ground state as
\begin{equation}
a_{1}|00\rangle_{\vec{n}_{y}}=0=a_{2}|00\rangle_{\vec{n}_{y}}.
\end{equation}
Hence we have found $|\Omega\rangle=|00\rangle_{\vec{n}_{y}}$ .
We know that the wave function in the $\vec{y}$ coordinates is the
product of well known simple harmonic oscillator solutions:
\begin{equation}
\langle y'_{1},y'_{2}|00\rangle_{\vec{n}_{y}}=\frac{1}{\left(\pi b_{1}^{2}\right)^{1/4}}\exp\left[\frac{-\left(y_{1}'\right)^{2}}{2b_{1}^{2}}\right]\frac{1}{\left(\pi b_{2}^{2}\right)^{1/4}}\exp\left[\frac{-\left(y_{2}'\right)^{2}}{2b_{2}^{2}}\right]
\end{equation}
where
\begin{equation}
b_{n}\equiv\frac{1}{\sqrt{m\omega_{n}}}
\end{equation}
making this a convenient basis to work with. Note
\begin{align*}
\hat{y}_{1}\left(\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}\right) & =\int dy_{1}'dy_{2}'\hat{y}_{1}|y_{1}'y_{2}'\rangle\langle y_{1}'y_{2}'|\left(\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}\right)\\
 & =\int dy_{1}'dy_{2}'y_{1}'|y_{1}'y_{2}'\rangle\langle y_{1}'y_{2}'|\left(\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}\right)\\
 & =\int dx_{1}'dx_{2}'y_{1}'\left(\left|x_{1}'\right\rangle _{x_{1}}\otimes\left|x_{2}'\right\rangle _{x_{2}}\right)\left(\,_{x_{1}}\langle x_{1}'|\otimes\,_{x_{2}}\langle x_{2}'|\right)\left(\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}\right)\\
 & =\frac{a+b}{\sqrt{2}}\left(\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}\right)\numberthis
\end{align*}
where we used the completeness of the basis, Eqs.~(\ref{eq:x1})
and (\ref{eq:x2}), and the usual delta function normalization of
the position basis. This and a similar relation for $\hat{y}_{2}$
imply
\begin{equation}
\left|a\right\rangle _{x_{1}}\otimes\left|b\right\rangle _{x_{2}}=\left|\frac{a+b}{\sqrt{2}},\frac{a-b}{\sqrt{2}}\right\rangle .
\end{equation}
This means
\begin{equation}
\,_{\vec{n}_{y}}\langle00|\left(|x_{1}'\rangle_{x_{1}}\otimes|w\rangle_{x_{2}}\right)=\,_{\vec{n}_{y}}\langle00|\frac{x_{1}'+w}{\sqrt{2}},\frac{x_{1}'-w}{\sqrt{2}}\rangle=\frac{1}{\left(\pi b_{1}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}'+w}{\sqrt{2}}\right)^{2}}{2b_{1}^{2}}\right]\frac{1}{\left(\pi b_{2}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}'-w}{\sqrt{2}}\right)^{2}}{2b_{2}^{2}}\right].
\end{equation}
The partial trace is defined through the following contraction of
$(2,2)$ tensor to a $(1,1)$ tensor: 
\begin{align*}
\hat{\rho} & =\int dx_{1}''\int dx_{1}'\int dw\left(|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}''|\otimes\,_{x_{2}}\langle w|\right)\left(|00\rangle_{\vec{n}_{y}}\,_{\vec{n}_{y}}\langle00|\right)\left(|x_{1}'\rangle_{x_{1}}\otimes|w\rangle_{x_{2}}\,_{x_{1}}\langle x_{1}'|\right)\\
 & =\int dx_{1}''\int dx_{1}'\int dw|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}'|\frac{1}{\left(\pi b_{1}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}''+w}{\sqrt{2}}\right)^{2}}{2b_{1}^{2}}\right]\frac{1}{\left(\pi b_{2}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}''-w}{\sqrt{2}}\right)^{2}}{2b_{2}^{2}}\right]\times\nonumber \\
 & \frac{1}{\left(\pi b_{1}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}'+w}{\sqrt{2}}\right)^{2}}{2b_{1}^{2}}\right]\frac{1}{\left(\pi b_{2}^{2}\right)^{1/4}}\exp\left[\frac{-\left(\frac{x_{1}'-w}{\sqrt{2}}\right)^{2}}{2b_{2}^{2}}\right].\numberthis
\end{align*}
Integrate over $w$, we find
\begin{align*}
\hat{\rho} & =\int dx_{1}''\int dx_{1}'|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}'|\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}}\exp\left[-\frac{m}{4}\left(\omega_{1}+\omega_{2}\right)\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)\right]\times\nonumber \\
 & \frac{\sqrt{2\pi}}{\sqrt{m\left[\omega_{1}+\omega_{2}\right]}}\exp\left[\frac{(\frac{\sqrt{\omega_{2}}}{\sqrt{\omega_{1}}}-\frac{\sqrt{\omega_{1}}}{\sqrt{\omega_{2}}})^{2}(x_{1}'+x_{1}'')^{2}}{8\frac{1}{m}(\frac{1}{\omega_{1}}+\frac{1}{\omega_{2}})}\right]\\
 & =\int dx_{1}''\int dx_{1}'|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}'|\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}}\times\nonumber \\
 & \frac{\sqrt{2\pi}}{\sqrt{m\left[\omega_{1}+\omega_{2}\right]}}\exp\left[\frac{m(\omega_{2}-\omega_{1})^{2}2x_{1}'x_{1}''-m\left[8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}\right]\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)}{8(\omega_{1}+\omega_{2})}\right].\numberthis
\end{align*}
Next, to identify the matrix, use
\begin{equation}
\frac{m(\omega_{2}-\omega_{1})^{2}2x_{1}'x_{1}''-m\left[8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}\right]\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)}{8(\omega_{1}+\omega_{2})}=-\frac{1}{2b^{2}}\left[\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)-2\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma}x_{1}'x_{1}''\right]
\end{equation}
\begin{equation}
\gamma\equiv8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}
\end{equation}
\begin{equation}
\frac{1}{2b^{2}}\equiv\frac{m\gamma}{8(\omega_{1}+\omega_{2})}
\end{equation}
\begin{equation}
b=2\sqrt{\frac{\omega_{1}+\omega_{2}}{m[8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}]}}
\end{equation}
to write
\begin{align}
\hat{\rho} & =\int dx_{1}''\int dx_{1}'|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}'|\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}} \times \nonumber\\
 & \frac{\sqrt{2\pi}}{\sqrt{m\left[\omega_{1}+\omega_{2}\right]}}\exp\left[-\frac{1}{2b^{2}}\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)\right]\exp\left(\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}x_{1}'x_{1}''\right).
\end{align}
Change basis to energy with a new effective frequency
\begin{equation}
b_{3}=\frac{1}{\sqrt{m\omega_{3}}}
\end{equation}
\begin{equation}
\hat{\rho}=\sum_{nv}|v\rangle\langle v|\hat{\rho}|n\rangle\langle n|
\end{equation}
\begin{align}
\langle v|\hat{\rho}|n\rangle & =\int dx_{1}''\int dx_{1}'\langle v|x_{1}''\rangle_{x_{1}}\,_{x_{1}}\langle x_{1}'|n\rangle\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}}\times\nonumber \\
 & \frac{\sqrt{2\pi}}{\sqrt{m\left[\omega_{1}+\omega_{2}\right]}}\exp\left[-\frac{1}{2b^{2}}\left(\left[x_{1}'\right]^{2}+\left[x_{1}''\right]^{2}\right)\right]\exp\left(\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}x_{1}'x_{1}''\right)
\end{align}
where
\begin{equation}
\langle x_{1}'|n\rangle=\frac{1}{\sqrt{n!b_{3}\sqrt{\pi}2^{n}}}e^{\frac{-\left(x_{1}'\right)^{2}}{2b_{3}^{2}}}H_{n}\left(\frac{x_{1}'}{b_{3}}\right)
\end{equation}
are the well known oscillator wave functions and $b_{3}$ still has
to be chosen. One can show by carrying out the integrals that the
matrix is diagonalized if 
\begin{align*}
b_{3} & =\frac{b}{\left(1-b^{4}\left[\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}\right]^{2}\right)^{1/4}}\\
 & =\frac{1}{\sqrt{m}\omega_{1}^{1/4}\omega_{2}^{1/4}}.\numberthis
\end{align*}
This gives
\[
\langle v|\hat{\rho}|n\rangle=\lambda_{n}\delta_{vn}
\]
 where
\begin{align*}
\lambda_{n} & =\frac{\sqrt{2\pi}}{\sqrt{m\left[\omega_{1}+\omega_{2}\right]}}\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}}m_{11}\left(\frac{b^{2}\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}}{1+\sqrt{1-b^{4}\left[\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}\right]^{2}}}\right)^{n-1}\\
 & =\frac{\pi\sqrt{m}}{2\left[\omega_{1}+\omega_{2}\right]^{3/2}}\frac{1}{\left(\pi b_{1}^{2}\right)^{1/2}}\frac{1}{\left(\pi b_{2}^{2}\right)^{1/2}}\frac{(\omega_{2}-\omega_{1})^{2}}{\left(\sqrt{m}\omega_{1}^{1/4}\omega_{2}^{1/4}\right)^{3}\left(\frac{b_{3}^{2}}{b^{2}}+1\right)^{3/2}}\left(\frac{\frac{(\omega_{2}-\omega_{1})^{2}}{8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}}}{1+\frac{b^{2}}{b_{3}^{2}}}\right)^{n-1}\numberthis
\end{align*}
where we used
\begin{align*}
m_{11} & =\frac{b^{3}\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}\sqrt{2\pi}}{\left(1+\sqrt{1-b^{4}\left(\frac{(\omega_{2}-\omega_{1})^{2}}{\gamma b^{2}}\right)^{2}}\right)^{3/2}}\\
 & =\frac{m(\omega_{2}-\omega_{1})^{2}\sqrt{2\pi}}{4(\omega_{1}+\omega_{2})\left(\frac{1}{b^{2}}+\frac{1}{b_{3}^{2}}\right)^{3/2}}\numberthis
\end{align*}
\begin{align*}
\left(\frac{b_{3}}{b}\right)^{2} & =\frac{1}{m\omega_{1}^{1/2}\omega_{2}^{1/2}}\frac{1}{4\frac{\omega_{1}+\omega_{2}}{m[8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}]}}\\
 & =\frac{1}{\omega_{1}^{1/2}\omega_{2}^{1/2}}\frac{8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}}{4\left(\omega_{1}+\omega_{2}\right)}.\numberthis
\end{align*}
Simplify:
\begin{align*}
\lambda_{n} & =\frac{4\sqrt{\omega_{1}\omega_{2}}}{\sqrt{8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}+4\omega_{1}^{1/2}\omega_{2}^{1/2}\left(\omega_{1}+\omega_{2}\right)}}\left(\frac{(\omega_{2}-\omega_{1})^{2}}{8\omega_{1}\omega_{2}+(\omega_{1}-\omega_{2})^{2}+\omega_{1}^{1/2}\omega_{2}^{1/2}4\left(\omega_{1}+\omega_{2}\right)}\right)^{n}\\
 & =\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]^{n}.\numberthis
\end{align*}
Since we want to evaluate
\begin{equation}
-\mathrm{Tr}\left[\hat{\rho}\ln\hat{\rho}\right]=-\partial_{n}\ln\mathrm{tr}\hat{\rho}^{n}|_{n=1}
\end{equation}
we compute
\begin{align*}
\ln\mathrm{tr}\rho^{n} & =\ln\left(\sum_{j=0}^{\infty}\lambda_{j}^{n}\right)\\
 & =\ln\left(\sum_{j}\left[\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]^{j}\right]^{n}\right)\\
 & =n\ln\left[\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right]+\ln\left(\sum_{j}\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]^{nj}\right)\\
 & =n\ln\left[\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right]-\ln\left(1-\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]^{n}\right).\numberthis
\end{align*}
Hence, we arrive at
\begin{align*}
S & =-\left\{ \ln\left[\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right]-\frac{\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]\ln\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]}{\left(1-\left[\frac{(\omega_{1}-\omega_{2})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right]\right)}\right\} \\
 & =\boxed{-\ln\left(\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right)-\left(\frac{(\omega_{2}-\omega_{1})^{2}}{4\sqrt{\omega_{1}\omega_{2}}\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right)\ln\left(\frac{(\omega_{2}-\omega_{1})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right)}\numberthis
\end{align*}
where
\begin{equation}
\boxed{\omega_{1}=\sqrt{\frac{k}{m}}\,\,\,\,\,\,\,\,\omega_{2}=\sqrt{\frac{k+2g}{m}}}.
\end{equation}

## Answer
$$
\begin{equation}
S = \boxed{-\ln\left(\frac{4\sqrt{\omega_{1}\omega_{2}}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right)-\left(\frac{(\omega_{2}-\omega_{1})^{2}}{4\sqrt{\omega_{1}\omega_{2}}\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{2}}\right)\ln\left(\frac{(\omega_{2}-\omega_{1})^{2}}{\left(\sqrt{\omega_{1}}+\sqrt{\omega_{2}}\right)^{4}}\right)}
\end{equation}
$$
where
$$
\begin{equation}
\boxed{\omega_{1}=\sqrt{\frac{k}{m}}\,\,\,\,\,\,\,\,\omega_{2}=\sqrt{\frac{k+2g}{m}}}.
\end{equation}
$$
## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function 
\begin{python}
def entropy(k:float,g:float,m:float)->float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from math import sqrt, log
def entropy(k:float,g:float,m:float)->float:
    w_1 = sqrt(k/m)
    w_2 = sqrt((k+2*g)/m)
    expr_1 = 4*sqrt(w_1*w_2)
    expr_2 = (sqrt(w_1)+sqrt(w_2))**2
    expr_3 = (w_2-w_1)**2
    return - log(expr_1/expr_2)-(expr_3/expr_1/expr_2)*log(expr_3/expr_2**2) 
\end{python}
