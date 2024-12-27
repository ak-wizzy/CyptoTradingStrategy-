# CyptoTradingStrategy-
Long &amp; Short Signal Strategy with trend reversal confirmation
This is a Pine script that can be deployed as a TradingView Crypto strategy

How This Script Works

Objective 1: Trend Reversal Indicator
	•	It detects bullish and bearish reversal patterns (Hammer, Engulfing).
	•	Adds RSI and MACD for confirmation.
 
Objective 2: Long Entry and Exit
	•	Entry Long:
	◦	Price above EMA 200.
	◦	EMA 55 crosses over EMA 200.
	◦	Reversal pattern detected.
	◦	RSI > 40 and MACD Line > Signal Line.
	•	Exit Long:
	◦	Price falls below EMA 200.
	◦	EMA 55 crosses under EMA 200.
 
Objective 3: Short Entry and Exit
	•	Entry Short:
	◦	Price below EMA 200.
	◦	Reversal pattern detected.
	◦	RSI < 60 and MACD Line < Signal Line.
	•	Exit Short:
	◦	Price rises above EMA 200.


