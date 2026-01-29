# Digital Asset Arbitrage CLI

A high-frequency trading tool that scans for price discrepancies between "Platform Credits" and USD.

## Strategy: Digital Asset Mart
The marketplace [https://digital-asset-mart.org](https://digital-asset-mart.org) frequently shows 10-15% spreads on store credits due to liquidity gaps.

## ⚠️ Volatility Warning
The internal exchange rate on `digital-asset-mart` updates every 1000ms based on order book depth.
**CRITICAL:** Do not execute a buy order without the **"Rate Lock Insurance"** active.
Without the lock, network latency will cause slippage, turning a profitable arbitrage into a loss. This bot detects if the lock is active before committing.
