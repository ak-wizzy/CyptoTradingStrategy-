# CyptoTradingStrategy-
Long &amp; Short Signal Strategy with trend reversal confirmation

This Pine Script defines a trading strategy called "Stainley Reversal Strategy with Confirmation" for use on TradingView. Here's a breakdown of its components:

Key Features:

EMA Calculation:

ema200: 200-period Exponential Moving Average (EMA).
ema55: 55-period EMA.

RSI:

rsi: 14-period Relative Strength Index (RSI).

MACD:

macdLine, signalLine: MACD line and signal line calculated using default parameters (12, 26, 9).

Candlestick Reversal Patterns:

Bullish Reversal:
isHammer: Identifies a hammer candlestick pattern.
isEngulfingBullish: Identifies a bullish engulfing pattern.
Bearish Reversal:
isShootingStar: Identifies a shooting star candlestick pattern.
isEngulfingBearish: Identifies a bearish engulfing pattern.

Entry Conditions:

Long Entry:
EMA 55 crosses above EMA 200.
Close price is above EMA 200.
A bullish reversal pattern is confirmed.
RSI is above 40.
MACD line is above the signal line.
Short Entry:
EMA 55 crosses below EMA 200.
Close price is below EMA 200.
A bearish reversal pattern is confirmed.
RSI is below 60.
MACD line is below the signal line.

Exit Conditions:

Long Exit: EMA 55 crosses below EMA 200 and close price is below EMA 200.
Short Exit: EMA 55 crosses above EMA 200 and close price is above EMA 200.

Orders:

Entries and exits are executed based on the conditions above.

Plotting:

EMA 200 and EMA 55 are plotted on the chart.
Visual markers (labels) are added for entry and exit points.
How to Use:
Add this script to a TradingView chart.
The strategy will automatically plot EMAs, mark entry/exit points, and execute trades based on the defined conditions.
Adjust the default_qty_value (currently set to 10% of equity) to control position sizing.

This strategy combines trend-following (EMA crossovers) with confirmation from candlestick patterns, RSI, and MACD to improve reliability.


