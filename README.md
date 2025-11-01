# SV EMA

A simple EMA (Exponential Moving Average) Tradingview indicator.

### Features
Based on the EMA values used by PandaTheTrader.
- EMA(8) with linewidth 1
- EMA(13) with linewidth 2
- EMA(48) with linewidth 3
- EMA(200) with linewidth 4

### Installation and Usage
1. **Copy the Pine Script**
- The full script is available in sv-ema.pine (or paste it directly from below).

2. **Add to Tradingview**
- Log in to [TradingView](tradingview.com).
- Open the Pine Editor (bottom panel of any chart).
- Paste the script into the editor.
- Click "Add to Chart" to apply it.
- Customize colors, lengths, or other parameters as needed via the indicator's settings menu.

### Pine Script Code
``` pinescript
//@version=6

// Created by Sebastian Vencill

indicator(title="SV EMA", shorttitle="EMA", overlay = true)

ema8 = ta.ema(close, 8)
ema13 = ta.ema(close, 13)
ema48 = ta.ema(close, 48)
ema200 = ta.ema(close, 200)

plot(ema8, title = "EMA 8", color = color.rgb(0, 0, 0), linewidth = 1)
plot(ema13, title = "EMA 13", color = color.rgb(0, 0, 0), linewidth = 2)
plot(ema48, title = "EMA 48", color = color.rgb(0, 0, 0), linewidth = 3)
plot(ema200, title = "EMA 200", color = color.rgb(0, 0, 0), linewidth = 4)
```

#### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 

If you have any questions or suggestions, open an issue in the repository!
