# Triple EMA (3-in-1) — Pine Script v5 Indicator

A compact but powerful **Tradingview indiator** that plots three customizable **Exponential Moving Averages (EMAs)** in one scripts.
Designed to save indicator slots while adding built-in alerts and visual trend cues.

## Features

- **Three EMAs in one indicator** - no more stacking multiple EMA scripts
- **Configurable lengths and colors** for each EMA
- **Build0in alers** for EMA crossovers
- **Optional on-chart labels** showing crossover points
- **Background highlights** for bullish/bearish alignment
- **Dynamic trend label** that updates with current trend direction

## How it Works

The indicator plots **three EMAs** directly on the price chart. \
It detects when faster EMAs cross slower ones, signaling potential trend shifts. \
When all three EMAs align (e.g.,9>21>50), the chart background turns faint green or red to visualize trend strength.

## User Input

| Setting             | Description                           | Default |
| :------------------ | :------------------------------------ | :------ |
| `EMA 1 Length`      | Fast EMA period                       | 9       |
| `EMA 2 Length`      | Medium EMA period                     | 21      |
| `EMA 3 Length`      | Slow EMA period                       | 50      |
| `Source`            | Price source (close, open, hl2, etc.) | close   |
| `Show Trend Labels` | Toggle on-chart crossover labels      | true    |

## Alerts Included

| Condition               | Description                       |
| :---------------------- | :-------------------------------- |
| EMA1 crosses above EMA2 | Possible short-term bullish shift |
| EMA1 crosses below EMA2 | Possible short-term bearish shift |
| EMA2 crosses above EMA3 | Possible trend continuation       |
| EMA2 crosses below EMA3 | Possible trend weakening          |

To enable:
1. Add the indicator to your TradingView chart.
2. Open Alerts → Condition → Triple EMA (3-in-1) with Alerts.
3. Select a condition and your desired alert method (popup, email, webhook, etc.).

## Installation
1. Copy the code from triple-ema.pine.
2. Open TradingView → Pine Editor
3. Paste the script and click Add to Chart.
4. Customize your settings under the indicator’s gear icon ⚙️.

## Example Configuration

Common EMA combinations you can try:

- Scalping: 5/13/21
- Swing trading: 9/21/50
- Long-term trend: 20/50/200

### License

This project is released under the **MIT License** — you’re free to use, modify, and distribute with attribution.

### Disclaimer

This indicator is for **educational and research purposes only**. \
It is  **not financial advice**, and past performance does not guarentee future results. \
Always perform your own due diligence before making any trading decisions.

