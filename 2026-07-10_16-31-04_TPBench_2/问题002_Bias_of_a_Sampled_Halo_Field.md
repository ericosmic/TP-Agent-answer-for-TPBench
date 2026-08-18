---
row_number: 2
csv_index: 1
problem_id: Bias of a Sampled Halo Field
domain: Cosmology
difficulty_level: 5
---

# Bias of a Sampled Halo Field

## Domain

Cosmology

## Difficulty Level

5

## Problem

In cosmology, large-scale cosmological dark-matter halo fields are biased tracers of the underlying Gaussian matter density $\delta_m$. Assume we have a sample $\delta_m$. We simulate a halo number density field by taking $n(\mathbf{x}) = \bar{n}\max(0,1+b\delta_m(\mathbf{x}))$, where bare number density $\bar{n}$ and bare bias $b$ are specified constants. What is the bias of the sampled halo field? Derive an equation to evaluate the bias which depends on the bare bias and the variance in each pixel.

## Solution

\textbf{Detailed Steps:}
The solution to this question involves some domain knowledge, parts of which were given in the problem's statement, some approximations sourced by the domain knowledge, and some mathematical calculations. The domain knowledge is very basic and should be known to anyone in the field. Approximations are intuitive and also, mostly, inspired by the domain knowledge. Following Polya, we can organize it as follows: \\

\textbf{Understand the problem.} The number density of halos $n_h(\mathbf{x})$ is defined as
\begin{equation}    N_h = \int_{V} n_h(\mathbf{x})d\mathbf{x}.\end{equation}
The overdensity is defined as \begin{equation}    \delta_h(\mathbf{x}) = \frac{n_h(\mathbf{x})-\langle n_h(\mathbf{x})\rangle}{\langle n_h(\mathbf{x})\rangle}.\end{equation}
Linear bias is defined in terms of Fourier-transformed quantities:\begin{equation}    \delta_h(\mathbf{k}) = b\delta_m(\mathbf{k}).\end{equation} 
This is an approximation that holds on sufficiently large scales (small $k$). $\delta_m(\mathbf{k})$ and $\delta_h(\mathbf{k})$ are Gaussian random fields with zero mean and their variance depends only on the magnitude of the wave-vector $k=|\mathbf{k}|$: 
\begin{equation}    \delta_m \sim \mathcal{N}(0,P_{mm}(k)),\ \delta_h \sim \mathcal{N}(0,P_{hh}(k)).\end{equation}The quantity $P(k)$ is called the power spectrum and is defined as \begin{equation}    \langle\delta(\mathbf{k})\delta(\mathbf{k'})\rangle = (2\pi)^3\delta^D(\mathbf{k+k'})P(k).\end{equation}
It immediately follows that\begin{equation}    P_{hh}(k) = b^2P_{mm}(k).\end{equation}
We are given the expression in real space. In real space, the quantity $\delta_m(\mathbf{x})$ is also a Gaussian random field:\begin{equation}    \delta_m(\mathbf{x}) \sim \mathcal{N}(0, \xi_m),\ \delta_h(\mathbf{x}) \sim \mathcal{N}(0, \xi_h).\end{equation}
Quantity $\xi$ is called a two-point (real-space) correlation function and is defined as\begin{equation}    \langle\delta(\mathbf{x})\delta(\mathbf{x'})\rangle = \xi(|\mathbf{x}-\mathbf{x'}|).\end{equation}This quantity is sufficiently small when $|\mathbf{x}-\mathbf{x'}|\gg1$. We are asked to find what is the expression for $b$ in the equation $\delta_h(k) = b\delta_m(\mathbf{k})$, given the real-space expression for the number density $n_h(\mathbf{x})$ in terms of real-space sample of $\delta_m(\mathbf{x})$.\\

\textbf{Devise a plan.} The key point to solve this problem should be that real-space correlation function for halos $\xi_h$ should also be equal to $b^2\xi_m$. We want to calculate that correlation function. It should be expressed in terms of $\langle n(\mathbf{x})\rangle$ and $\langle n_h(\mathbf{x})n_h(\mathbf{x'})\rangle$. We expect to be able to calculate these expectations since they are the expectations of functions of the Gaussian random variables. We are given the pixel variance $\sigma$. How does it connect to the other quantities we know? In principle, that's also the part of domain knowledge but it also can be deducted from the definitions already given. A discretized version of the correlation function is \begin{equation}    \xi_{ij} = \langle\delta_{\mathbf{x_i}}\delta_{\mathbf{x_j}}\rangle.\end{equation}
When $i=j$, it becomes the pixel variance $\sigma$. \textit{Aside, we could have given instead of $\sigma$, the quantity $P_{mm}(k)$, that is a common description of a cosmological dark-matter field. In that case, from the definitions of $\xi(r)$ and $P_{mm}(k)$, we could have deduced that $\sigma = \frac{1}{V}\sum_{k}P_{mm}(k)$}. Then we pick the ensemble of all the pixels at given fixed large distance $r=|\mathbf{x_i}-\mathbf{x_j}|$. The key is to recognize that it is fully described by a correlated bivariate Gaussian distribution. \begin{equation}    (\delta^m_{i},\delta^m_{j}) \sim \mathcal{N}(0,\Sigma) \end{equation}with a covariance\begin{equation}    \Sigma = \begin{pmatrix}        \sigma^2 & \xi^m_r  \\      \xi^m_r & \sigma^2    \end{pmatrix}.\end{equation}In general, the integrals from the expectation values are cumbersome, but we should expect some simplifications from the fact that $\xi$ is small and we can Taylor-expand the pdf. \\


\textbf{Carry out the plan.} It's more convenient to define $\hat{\delta}_{i} = \delta^m_i/\sigma$ and $\hat{\xi} = \xi^m_r/\sigma^2$, and $\phi_2$ - a correlated bivariate Gaussian pdf - then \begin{equation}    (\hat{\delta}_{i},\hat{\delta}_{j}) \sim \frac{e^{-\frac{1}{2(1-\hat{\xi}^2)}[\hat{\delta}^2_{i}+\hat{\delta}^2_{j}-2\hat{\xi}\hat{\delta}_{i}\hat{\delta}_{j}]}}{2\pi\sqrt{1-\hat{\xi}^2}} \equiv \phi_2(\hat{\delta}_{i},\hat{\delta}_{j}|\hat{\xi}).\end{equation}We note that \begin{equation}    \xi^{n}_r = \frac{\langle n_in_j\rangle}{\langle n \rangle^2}-1.\end{equation}The quantity $\langle n\rangle$ is the actual mean number density:\begin{equation*}    \bar{n}^{'} = \langle n \rangle = \langle n_i \rangle = \int n^{loc}(\delta_i,b,\bar{n}) \phi_2(\hat{\delta}_{i},\hat{\delta}_{j}|\hat{\xi}) d\hat{\delta}_{i}d\hat{\delta}_{j} = \int n^{loc}_i \phi_1(\hat{\delta_i})d\hat{\delta_i}.\end{equation*}Here, $\phi_1$ - is a standard normal pdf. It is expected that it's not dependent on the correlation $\hat{\xi}$, but only on $b$ and $\sigma$, just as the marginal of 2D correlated Gaussian distribution is 1D Gaussian that's not dependent on the cross-correlation. To the linear order in $\hat{\xi}$, \begin{equation}    \phi_2(x,y|\hat{\xi}) \approx \phi_1(x)\phi_1(y)(1+\hat{\xi}xy).\end{equation} So that the two-point function neatly factorizes:\begin{align*}    &\langle n_in_j\rangle = \int n^{loc}(\delta_i,b,\bar{n})n^{loc}(\delta_j,b,\bar{n}) \phi_2(\hat{\delta}_{i},\hat{\delta}_{j}|\hat{\xi}) d\hat{\delta}_{i}d\hat{\delta}_{j} \\ &\approx \int n^{loc}_i \phi_1(\hat{\delta_i})d\hat{\delta_i}\int n^{loc}_j \phi_1(\hat{\delta_j})d\hat{\delta_j} + \hat{\xi}\int n^{loc}_i \phi_1(\hat{\delta_i})\hat{\delta_i}d\hat{\delta_i}\int n^{loc}_j \phi_1(\hat{\delta_j})\hat{\delta_j}d\hat{\delta_j} \\ &\equiv \langle n\rangle^2 + \hat{\xi} \langle n\hat{\delta }\rangle^2.\numberthis\end{align*}
Substituting the results for $\langle n\rangle$ and $\langle n_in_j\rangle$ in  the equation for $\xi^n_r$, we can read off the bias:\begin{equation}b^{'2} = \frac{\xi^n_r}{\sigma^2\hat{\xi}} = \frac{\langle n\hat{\delta}\rangle^2}{\sigma^2\langle n\rangle^2}.\end{equation}
All that is left is to calculate the expectations. One can evaluate for $b\geq0$ 
\begin{align*}    
\langle n\rangle &= \int n^{loc}_i \phi_1(\hat{\delta_i})d\hat{\delta_i} = \int \bar{n}\max(0, 1+b\sigma x)\phi_1(x)dx \\  &= \bar{n}\int_{-\frac{1}{b\sigma}}^{+\infty}(1+b\sigma x)\phi_1(x)dx = \bar{n}\left[\Phi_1\left(\frac{1}{b\sigma}\right)+b\sigma\phi_1\left(\frac{1}{b\sigma}\right)\right].\numberthis \end{align*}
For $b<0$ it's, however, 
\begin{align*}    
\langle n\rangle &= \bar{n}\int_{-\infty}^{+\frac{1}{|b|\sigma}}(1-|b|\sigma x)\phi_1(x)dx\\ &= \bar{n}\left[\Phi_1\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi_1\left(\frac{1}{|b|\sigma}\right)\right].\numberthis\end{align*}So we conclude that the latter expression is valid for all $b$. Similarly, one can show that\begin{equation}\langle n\hat{\delta }\rangle = \bar{n}\int\max(0,1+b\sigma x)x\phi_1(x)dx = \bar{n}b\sigma \Phi_1\left(\frac{1}{|b|\sigma}\right)\end{equation}
where $\Phi_1(x) = \int_{-\infty}^x\phi_1(x)dx$ - normal cdf. Finally, one can get
\begin{equation}\boxed{b^{'} = \frac{b \Phi_1\left(\frac{1}{|b|\sigma}\right)}{\Phi_1\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi_1\left(\frac{1}{|b|\sigma}\right)}}.\end{equation}

Note: We also accept solutions as correct if they omit the $|~|$ around the bias, since halo bias is usually positive.

## Answer

The bias of the sampled halo field is given by:
$$
\begin{equation}
\boxed{
b^{'} = \frac{b \Phi_1\left(\frac{1}{|b|\sigma}\right)}{\Phi_1\left(\frac{1}{|b|\sigma}\right)+|b|\sigma\phi_1\left(\frac{1}{|b|\sigma}\right)}}
\end{equation}
$$
where $\Phi_1$ is the normal cumulative distribution function, $\phi_1$ is the standard normal probability density function, $b$ is the bare bias, and $\sigma$ is the pixel variance.

## Code Answer Requirements

Provide the answer in the form of the \texttt{python} code. Implement the following function.
\begin{python}
#let b_in stand for bare bias
def b_eff(sigma: float, b_in:float) -> float:
    pass
\end{python}

## Reference Implementation

\begin{python}
from scipy.stats import norm
#let b_in stand for bare bias
def b_eff(sigma: float, b_in:float) -> float:
    alpha = sigma*abs(b_in)
    return b_in*norm.cdf(1/alpha)/(norm.cdf(1/alpha)+alpha*norm.pdf(1/alpha))
\end{python}

\newpage

\newpage
