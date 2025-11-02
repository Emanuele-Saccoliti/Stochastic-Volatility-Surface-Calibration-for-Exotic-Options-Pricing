# Volatility-Surface-Calibration-for-Exotic-Options-Pricing

- This repository provides a stochastic volatility pricing engine based on Heston model calibration to vanilla option market quotes across a wide range of strikes and maturities, ensuring market-consistent volatility smiles and term structures.

- The tool provides 3D volatility surface visualization with color gradients to visualize how implied volatility changes across strikes and
expirations, allowing a clear comparison between market-implied volatilities and the model outputs for detecting potential inconsistencies or arbitrage opportunities.

- Building on the calibrated framework, model is extended to path-dependent payoffs, implementing Monte Carlo simulations to accurately value barrier options and other exotic derivatives.

- The tool integrates interactive dashboards for scenario analysis, equipped with sliders to vary strikes, barrier levels, and simulated paths in real time, enabling dynamic exploration of exotic option risk/return profiles under different market conditions.


# 🔍 Key Objectives
* Explore what are the challenges in exotic options pricing & stochastic volality calibration
* Generate volatility smiles & surfaces consistent with market conditions
* Price barrier options via Monte Carlo simulation under the calibrated model
* Build interactive dashboards for scenario analysis, dynmamic option pricing & risk management


# 📌 Key Takeaways
* Accurate calibration to vanillas is essential to ensure realistic exotic pricing
* The calibrated Heston model reproduces market smiles & term structures
* Monte Carlo simulation enables pricing of path-dependent payoffs (e.g., barriers)


# ⚠️ Challenges
* Market microstructure noise: Bid–ask spreads, sparse strikes/maturities, and stale quotes distort the implied volatility surface, demanding filtering and smoothing techniques.
* Discontinuities in payoff: Barriers create discontinuous payoff structures, and MC estimators suffer high variance, requiring variance-reduction.
* Balancing Accuracy vs. Speed: Undeniable computational cost that makes the calibration–pricing loops heavy.
* Ensuring Arbitrage-Free Surfaces: Model-generated volatility surfaces must avoid arbitrage (calendar, butterfly).
* Greeks estimation: Path-dependent Greeks under stochastic volatility do not have closed formula and require advanced techniques.
