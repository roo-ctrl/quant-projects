# Quant Projects

These are personal articles, not homework. While I was working through the M.S. in Computational Finance and Risk Management at the University of Washington, I kept running into the same itch. The theory looked clean on the whiteboard, but would it actually hold up on real market data? So after each course I picked one idea and went to find out.

That meant hunting for cointegrated pairs across the entire S&P 500, pitting three risk measures against each other in a backtest, and forecasting how bank stocks would move on earnings day, the night before they reported.

My favorite came out of Machine Learning for Finance (CFRM 521). I grew up in Washington County, Oregon, so I took what I learned there and tried forecasting the county’s median home sale price with a “wisdom of the crowd” twist. I trained four regression models and let each one have more or less say depending on how well it had done in similar economic times. That blended forecast beat every individual model by a wide margin.

Not everything went my way. I was sure a fat tailed Laplace distribution, which fit daily returns far better than a Normal, would make better price forecasts. It didn’t. Add up enough Laplace days and you get something that looks a lot like a Normal again. That’s the Central Limit Theorem, and I learned it the hard way. Surprises like that taught me more than the wins did.

You can read them on [the project website](https://roo-ctrl.github.io/quant-projects/).

| Article | Course | What it is about |
|---|---|---|
| [Housing Research, Wisdom of the Crowd](https://roo-ctrl.github.io/quant-projects/housing-median-price-regime-ensemble.html) | CFRM 521, 2024 · my favorite | Four models forecast my home county’s median sale price, and whichever has done best in similar economic times gets the loudest voice. The blended forecast came out about five times more accurate than the best single model. |
| [Cointegration and the Two Step Method](https://roo-ctrl.github.io/quant-projects/cointegration-pairs-cfrm502.html) | CFRM 502, 2023 | I searched every pair of S&P 500 stocks for two that drift apart and snap back together, then watched how the best three behaved once my data ended. |
| [Mean Variance vs. MAD vs. CVaR](https://roo-ctrl.github.io/quant-projects/risk-measures-mv-mad-cvar-cfrm503.html) | CFRM 503, 2023 | Three different ways to build a portfolio around risk, each rebuilt every month and run through three years of real markets to see which held up best. |
| [Laplace vs. Normal Monte Carlo](https://roo-ctrl.github.io/quant-projects/laplace-vs-normal-monte-carlo-cfrm501.html) | CFRM 501, 2023 | Stock returns have fatter tails than a bell curve, so I tested whether simulating prices with a fatter tailed distribution gives better forecasts. Mostly, it didn’t. |
| [Composition Monte Carlo With Earnings](https://roo-ctrl.github.io/quant-projects/composition-monte-carlo-earnings-cfrm505.html) | CFRM 505, 2024 | How a stock moves on earnings day depends on whether the company beats or misses. I modeled both outcomes, mixed them by how often each happens, and forecast JPM, C, and BAC the night before they reported. |
