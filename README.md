# Quant Projects

These are personal articles, not homework. While I was working through the M.S. in Computational Finance and Risk Management at the University of Washington, I kept running into the same itch: the theory looked clean on the whiteboard, but would it actually hold up on real market data? So after each course I picked one idea and went to find out.

That meant hunting for cointegrated pairs across the entire S&P 500, pitting three risk measures against each other in a backtest, and forecasting how bank stocks would move on earnings day, the night before they reported.

My favorite isn't from a course at all. I grew up in Washington County, Oregon, so I tried forecasting its median home sale price with a "wisdom of the crowd" twist: four regression models, each trusted more or less depending on the macro regime it had historically done well in. That regime-weighted forecast beat every individual model by a wide margin.

Not everything went my way. I was sure a fat-tailed Laplace distribution, which fit daily returns far better than a Normal, would make better price forecasts. It didn't. Add up enough Laplace days and you get something that looks a lot like a Normal again. That's the Central Limit Theorem, and I learned it the hard way. Surprises like that taught me more than the wins did.

Read them rendered at **https://roo-ctrl.github.io/quant-projects/**

| Write-up | Course | Topic |
|---|---|---|
| [Housing Research: Wisdom of the Crowd](https://roo-ctrl.github.io/quant-projects/housing-median-price-regime-ensemble.html) | Personal (2024) | Regime-weighted ensemble of Linear, Lasso, Ridge, ElasticNet (PCA + k-means on FRED data) |
| [Cointegration and the Two-Step Method](https://roo-ctrl.github.io/quant-projects/cointegration-pairs-cfrm502.html) | CFRM 502 | S&P 500 pairs screen: Engle-Granger, Phillips-Ouliaris, KPSS |
| [Risk Measures: Mean-Variance vs. MAD vs. CVaR](https://roo-ctrl.github.io/quant-projects/risk-measures-mv-mad-cvar-cfrm503.html) | CFRM 503 | Convex portfolio optimization (CVXPY) and backtests |
| [Monte Carlo: Laplace vs. Normal Returns](https://roo-ctrl.github.io/quant-projects/laplace-vs-normal-monte-carlo-cfrm501.html) | CFRM 501 | Fat-tailed return modeling, method of moments |
| [Composition Monte Carlo With Earnings](https://roo-ctrl.github.io/quant-projects/composition-monte-carlo-earnings-cfrm505.html) | CFRM 505 | Earnings-day price ranges from beat/miss distributions |
