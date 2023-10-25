
# COMP4680 ASE: Total Variation Denoising
This project involves the investigation of problems in deep declarative networks [Gould et al., 2021]. 
We will specifically be focused on the problem of differentiating the solution of a total variation reconstruction problem [Boyd and Vandenberghe, 2004, §6.3.3]. 
Concretely the total variation problem can be stated as

```math
\mathrm{minimize}_u \quad  f(u,x) =  \frac{1}{2}\|Ax - b\|_2^2 + \lambda \sum_{i=1}^n |u_{i+1}-u_i|
```

where $x ∈ \mathbb{R}^n$ is a one-dimensional input signal of length $n$ and $u \in \mathbb{R}^n$ is the optimization variable. The solution $u^⋆$ is a smoothed, or de-noised, version of the input, we define $y(x)=u^*$. The goal is to implement a PyTorch autograd function for differentiable total variation denoising.