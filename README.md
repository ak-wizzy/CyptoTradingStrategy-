# CyptoTradingStrategy-
Long &amp; Short Signal Strategy with trend reversal confirmation
This is a Pine script that can be deployed as a TradingView Crypto strategy

1.	Candlestick Reversal as Confirmation:
o	Reversal patterns (isBullishReversal, isBearishReversal) are combined with EMA crossover and other conditions.
o	Reversal patterns alone no longer trigger signals.

3.	Conditions for Entry:
o	A long entry requires:
	EMA 55 crossing above EMA 200.
	Price above EMA 200.
	A bullish reversal candlestick.
	RSI > 40 and MACD Line > Signal Line.
o	A short entry requires:
	EMA 55 crossing below EMA 200.
	Price below EMA 200.
	A bearish reversal candlestick.
	RSI < 60 and MACD Line < Signal Line.

5.	Exit Signals:
o	Exits occur only on EMA crossovers back in the opposite direction, combined with price conditions.

•	The buy signal should occur only when the following conditions are met:
1.	EMA 55 crossover EMA 200 (or price crosses EMA 200).
2.	The reversal candlestick (Hammer or Engulfing) confirms the direction.
3.	RSI and MACD provide additional validation.
This prevents a buy signal from being triggered on every reversal candlestick.

