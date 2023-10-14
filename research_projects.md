# Research Projects

## Foundations of Machine Learning

I am generally interested in how to build better machine learning (ML) models for applied scientific applications. A general feature of machine learning development is that it is often undertaken by individuals who have actually had very little background in applied sciences. As a consequence, ML methods can often be somewhat divorced from the real world realities of applications by stylising the problem into a form which is mathematically or computationally convenient and elegant but, in doing so, making it impractical in the real world.

### Stability of machine learning models

Let $X$ denote an input and $Y$ denote an output and assume a function $f_\theta$ parameterised by $\theta$ links input and output via the relationship $Y = f_\theta(X) + \epsilon$ where $\epsilon$ is iid noise. Given data $D = \{\{x_1, y_1\}, \dots, \{x_n,y_n\}\}$, learning corresponds to finding $\hat{theta}$ (or a distribution over $p(\theta|D)$ in a Bayesian setting) that minimises an empirical loss function $L_\theta(D)$:

$$
  \hat{\theta} = \arg \min_{\theta} L_\theta(D)
$$

The performance of the model depends on three key things:

1. The detailed specification of $f_\theta$, e.g. is it linear? is it a neural network?, and its capacity to flexibly model different relationships including the *unknown* but true function (**model specification**).
2. Our ability to learn $\hat{\theta}$ to identify that true function given data (**optimisation**).
3. The representative of the data $D$ of the test time data distribution (**predictive capability**).

The stability of a model refers to whether (potentially small) deviations in model parameters or data distribution could cause the model to give wildly different predictions. 

That is, if $y_1 = f_\theta(x)$ and $y_2 = f_{\theta'}(x)$, where $\theta' = \theta (1 + \delta)$, if the distance between the outputs $d(y_1, y_2) \gg 0$ when $\delta \ll 1$ then the model is considered to be *unstable* with respect to its parameters (which could be due to either model misspecification or poor optimisation). 

Similarly, if $y_1 = f_\theta(x_1)$ and $y_2 = f_{\theta}(x_2)$, where $x_1 \sim Q_1$ and $Q_2 \sim H_2$ and $H_1$ and $H_2$ are two input distributions, if the distance between the outputs $d(y_1, y_2) \gg 0$ when the distance between input distributions $h(Q_1,Q_2)$ then the model is considered to be *unstable* with respect to its input distribution.

**Research Problem** Unstable machine models are problematic in critical applications, such as in medical devices, can we build machine learning models with *built-in* mechanisms to minimise instability from the outset?

**Motivation** Medical devices based on provably stable machine learning models are better candidates for regulatory approval than those where there are no stability guarantees.

## Applications

###
