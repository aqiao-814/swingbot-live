# Swingbot Live

**Dashboard: https://aqiao-814.github.io/swingbot-live/**

A fully simulated $100,000 paper portfolio traded autonomously by an
online-learning RRL (recurrent reinforcement learning) policy over the
NASDAQ-100 universe:

- Each trading day after the close, the bot scores every stock, ranks by
  conviction, and queues orders that fill at the **next market open** with
  modeled spread, slippage, impact, and SEC/TAF fees.
- During market hours the dashboard marks the book to market with live
  quotes and shows the morning's fills as they execute.
- State in `state/` is the bot's persistent portfolio (JSON + parquet),
  updated nightly by GitHub Actions. `data.json` / `live.json` feed the page.

**No real money. Nothing here is investment advice.** Quotes via Yahoo
Finance, may be delayed ~15 minutes.
