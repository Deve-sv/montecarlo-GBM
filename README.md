# Monte Carlo Simulation of Stock Prices using Geometric Brownian Motion (GBM)

##  Project Overview
This project simulates stock price trajectories using the Geometric Brownian Motion (GBM) model.  
GBM is one of the most widely used stochastic processes in quantitative finance, forming the basis for:
- Stock price modeling
- Option pricing (e.g., Black–Scholes model)
- Risk and portfolio simulations

The notebook generates multiple price paths, visualizes the results, and explores the impact of drift (mu) and volatility (sigma).

---

##  Objectives
- Implement a GBM simulation in Python.
- Understand the role of drift (expected annual return) and volatility (annualized standard deviation).
- Visualize multiple simulated paths of stock prices over time.
- Show the distribution of final prices at maturity.

---

##  Mathematical Model
The GBM model can be described as:

Change in price over time:
dS = mu * S * dt + sigma * S * dW

Where:
- S = Stock price at time t  
- mu = Drift (expected return)  
- sigma = Volatility of returns  
- W = Standard Brownian motion  

The analytical solution can be written as:
S_t = S_0 * exp( (mu - 0.5 * sigma^2) * t + sigma * W_t )

---

## Method
1. Define parameters: initial price (S0), drift (mu), volatility (sigma), time horizon (T), number of time steps, number of paths.
2. Simulate Brownian motion increments as random values from a normal distribution with mean 0 and variance proportional to the time step.
3. Apply the GBM formula to simulate paths.
4. Plot multiple stock price paths.
5. Plot histogram of terminal prices.

---

##  How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Deve-sv/montecarlo-sps.git
