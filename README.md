# Quant Projects

These are personal articles, not homework. While I was working through the M.S. in Computational Finance and Risk Management at the University of Washington, understanding the theory took a lot of effort, and I always wanted to see how it would fare in the real world. So after each course, I picked the one or two topics I was most curious about and built a project around them to find out.

That meant hunting for cointegrated pairs across the entire S&P 500, building optimal portfolios from three different risk measures and backtesting how each one held up, testing whether a more tailored distribution like the Laplace forecasts prices better than the usual Normal, and forecasting how bank stocks would move on earnings day, the night before they reported.

My favorite came right after I took Machine Learning for Finance (CFRM 521). That summer I was leading the UW team in the Open Quant League hosted by QuantConnect, and we were working with several machine learning models at once. I noticed that when we blended them together, the forecasts got better and the mean squared error dropped by a large amount. That really stuck with me, because it felt like the wisdom of the crowd, where a group’s combined guess beats almost any single person’s. At the time I was also deep into interest rates and housing, since I had been working with Redfin’s real estate data. So I put the two together and pointed the idea at Washington County, Oregon, where I grew up, to see if I could forecast its median home sale price for the next month. I built four regression models and let each one have more or less say depending on how well it had done in similar economic times (grouping those times into clusters with k-means on macroeconomic data). That blended forecast beat every individual model by a wide margin.

Not everything went my way. I was sure a fat tailed Laplace distribution, which fit daily returns far better than a Normal, would make better price forecasts. It didn’t. Add up enough Laplace days and you get something that looks a lot like a Normal again. That’s the Central Limit Theorem, and I learned it the hard way. Surprises like that taught me more than the wins did.

You can read them on [the project website](https://roo-ctrl.github.io/quant-projects/).

Written before I found Claude, so every typo is handmade.

| Article | Course | What it is about |
|---|---|---|
| [Housing Research, Wisdom of the Crowd](https://roo-ctrl.github.io/quant-projects/housing-median-price-regime-ensemble.html) | CFRM 521, 2024 · my favorite | Four models forecast my home county’s median sale price, and whichever has done best in similar economic times gets the loudest voice. The blended forecast came out about five times more accurate than the best single model. |
| [Crypto Cointegration with Walk Forward Analysis*](https://roo-ctrl.github.io/quant-projects/crypto-cointegration-walk-forward-cfrm523.html) | CFRM 523 (2024) | Cointegrated BTC, ETH, LTC, and SOL spreads from Tim Leung’s paper, tuned with walk forward analysis, with a neural network forecast as a second opinion. Where I fell in love with backtesting and Backtrader |
| [Cointegration and the Two Step Method](https://roo-ctrl.github.io/quant-projects/cointegration-pairs-cfrm502.html) | CFRM 502, 2023 | I searched every pair of S&P 500 stocks for two that drift apart and snap back together, then watched how the best three behaved once my data ended. |
| [Mean Variance vs. MAD vs. CVaR](https://roo-ctrl.github.io/quant-projects/risk-measures-mv-mad-cvar-cfrm503.html) | CFRM 503, 2023 | Three different ways to build a portfolio around risk, each rebuilt every month and run through three years of real markets to see which held up best. |
| [Laplace vs. Normal Monte Carlo](https://roo-ctrl.github.io/quant-projects/laplace-vs-normal-monte-carlo-cfrm501.html) | CFRM 501, 2023 | Stock returns have fatter tails than a bell curve, so I tested whether simulating prices with a fatter tailed distribution gives better forecasts. Mostly, it didn’t. |
| [Composition Monte Carlo With Earnings](https://roo-ctrl.github.io/quant-projects/composition-monte-carlo-earnings-cfrm505.html) | CFRM 505, 2024 | How a stock moves on earnings day depends on whether the company beats or misses. I modeled both outcomes, mixed them by how often each happens, and forecast JPM, C, and BAC the night before they reported. |

*Actually was the final project, but I loved that this was my favorite class, and I wanted to share.

## Before the Master’s (please don’t laugh)

Long before I had the math to back it up, I was already hooked on markets. These are from my physics degree at Oregon State and the years right after, back when I had plenty of curiosity and not much mathematical rigor. Please don’t laugh. I’m proud of them, and of how far things have come since.

- [Senior Thesis, Lagrangian Mechanics Description of an Economic System](https://roo-ctrl.github.io/quant-projects/early-work/senior_thesis.html) (Oregon State University, 2018). I simulated an economy of 100 traders swapping five goods, each chasing their own happiness, and used the physics of Lagrange multipliers to see whether supply, demand, and inflation would show up on their own. They did.
- [Option Volatility and Pricing, Sheldon Natenberg](https://roo-ctrl.github.io/quant-projects/early-work/natenberg-option-volatility-and-pricing.html) (lunch breaks at Intel). During lunch breaks at Intel and on my days off, I tried to teach myself the daunting world of options with Natenberg’s classic. These are my chapter summaries and worked exercises for chapters 4 through 9, from parity graphs to dynamic hedging.
- [More Smirk Than Smile](https://roo-ctrl.github.io/quant-projects/early-work/more_smirk_than_smile.html) (2022). Textbooks promise options a volatility smile. I collected a week of minute by minute SPY options data, solved for implied volatility by brute force, and animated the curve. It looked a lot more like a smirk.
- [Hedge Finder](https://roo-ctrl.github.io/quant-projects/early-work/hedge_finder_page.html) (2022). A small script that takes any stock and ranks the rest of the S&P 500 by how closely their daily moves line up, to find possible hedges. Intel was my test subject.
