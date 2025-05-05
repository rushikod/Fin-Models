# Financial Risk and Pricing Models
## 1. Market Risk Measurement using Value at Risk (VaR) 

Value at Risk (VaR) estimates the potential loss in the value of a portfolio over a defined period for a given confidence level. It answers: "How much could I lose with X% confidence over Y days?"

**Common VaR Methods:**
1.Historical Simulation: Uses actual past returns to simulate potential losses.

VaR = Percentile loss at (1 - confidence level)

2.Variance-Covariance (Parametric): Assumes returns are normally distributed; uses mean and standard deviation.

VaR = Z × σ

3.Monte Carlo Simulation: Generates random scenarios based on statistical properties of asset returns.

VaR = Percentile of simulated loss distribution


## 2. Portfolio Optimization
Portfolio Optimization aims to allocate assets to maximize return and minimize risk, often using Mean-Variance Optimization (MVO).
Steps Involved
Collect Data: Historical prices → returns

Compute Statistics: Mean returns, covariance matrix

Define Objective: Maximize return or minimize risk

Apply Constraints:

Sum of weights = 1 (fully invested)

Weights ≥ 0 (long-only portfolio)

Optimize: Use solvers (e.g., scipy.optimize or cvxpy)

Plot Efficient Frontier: Shows best possible return for each level of risk.

Important Parameters
Expected Return (μ): CAPM Model = Rf + Beta * (Rm - Rf).

Covariance Matrix (Σ)

Portfolio Weights (w)

Risk-Free Rate (rf) (for Sharpe ratio-based optimization)

## 3. Option Pricing

 Black-Scholes Model (Analytical)

 Used for pricing European call/put options on non-dividend paying stocks.
 ![640144bce6aad280ca7202e7_FWHezgjutKI5WaPNR7v_BI20Je-u6NbUgBVKMySCEbOj-iVHp8tZ-VLPkItcHHBO2tcopGIC-4EmS1vdRrHe4A994C1EcCs8OFHm3dZykEqy7YQnMaSV1-WwY-vUVGM9q3K3Liueq6Ua](https://github.com/user-attachments/assets/6a176f5d-8f9d-4d09-957d-fec964e32161)
