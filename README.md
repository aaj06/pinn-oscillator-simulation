# Physics-Informed Neural Network Simulation

The objective of this repository is to model/analyze 1D dampled harmonic oscillation using neural networks under the following 3 cases:

Case 1: Purely data-driven DNN's (deep neural networks)
Case 2: Limited data-driven 
Case 3: Purely physics-informed

## Mathematical setup

1. Equation of interest

$$
m \frac{d^2 u}{dt^2} + \mu \frac{du}{dt} + k u = 0
$$ 

2. Normalized form
$$
u'' + 2\delta u' + \omega_0^2 u = 0
$$
, where 
$$
\delta = \frac{\mu}{2m}, \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

## Initial Conditions

\begin{equation}
u(0) = 1, \qquad \frac{du}{dt}(0) = 0
\end{equation}

## Exact (Analytical) Solution

\begin{equation}
u(t) = e^{-\delta t}\left( 2A \cos(\phi + \omega t) \right)

## Intial Conditions

$$
\begin{equation}
u(0) = 1, \qquad \frac{du}{dt}(0) = 0
\end{equation}
$$

## Case 1
- Neural networks purely fed data
- Fully supervised learning

## Case 2
- Trained on t in [0,0.75]
- Expected extrapolation error for t > 0.75

## Case 3
- No training data
Loss: 
$$
\mathcal{L} = \frac{1}{N} \sum (m u'' + \mu u' + k u)^2
$$

## Key Observations
- Physics-informed models are only fed governing equations, no data
- Data-driven are only given data points, no physics
- Physics-informed predictive models are more accurate than data-driven models

## Author
Ameera Junaid
