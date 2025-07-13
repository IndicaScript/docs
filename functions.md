# Functions

These are builtin functions that corresponds to functions within ThinkScript

## SMA (Simple Moving Average)

`SMA(price, length)`
`SimpleMovingAverage(price, length)`

Calculates the **Simple Moving Average** of the given `price` over the past `length` candlesticks.

[Investopedia Link](https://www.investopedia.com/terms/s/sma.asp)

### Example:

`smaValue = SMA(close, 14)`

This calculates the 14-period simple moving average of the **closing price**.

## WMA (Weighted Moving Average)

`WMA(price, length)`
`WeightedMovingAverage(price, length)`

Calculates the **Weighted Moving Average** of the given `price` over the past `length` candlesticks.

[Investopedia Link](https://www.investopedia.com/ask/answers/071414/whats-difference-between-moving-average-and-weighted-moving-average.asp)

### Example:

`wmaValue = WMA(close, 14)`

This calculates the 14-period weighted moving average of the **closing price**.

## WildersAverage (Wilder’s Smoothing)

`WildersAverage(price, length)`

Calculates the **Wilder’s Moving Average** of the given `price` over the past `length` candlesticks.  
It is similar to an exponential moving average but uses a smoothing factor of `1/length`.

This average is commonly used in indicators like **RSI**, **ADX**, and others in technical analysis.

[TrendSpider Link](https://trendspider.com/learning-center/definition-of-wilders-moving-average/)

## Momentum

`Momentum(price, length)`

Calculates the **momentum** of the given `price` over the past `length` candlesticks.  
It measures the difference between the current price and the price `length` periods ago:

```
Momentum = price - price[length]
```

A positive value indicates upward momentum, while a negative value indicates downward momentum.

[Investopedia Link](https://www.investopedia.com/terms/m/momentum.asp)

### Example:

    m = Momentum(close, 10)

This calculates the difference between the current close and the close from 10 candles ago.

## RSI (Relative Strength Index)

`RSI(price, length)`
`RelativeStrengthIndex(price, length)`

Calculates the **Relative Strength Index (RSI)** of the given `price` over the past `length` candlesticks.  
RSI is a momentum oscillator that ranges from 0 to 100 and is used to measure the speed and change of price movements.

- RSI values above 70 typically indicate **overbought** conditions.
- RSI values below 30 typically indicate **oversold** conditions.

Internally, RSI uses Wilder’s smoothing method.

[Investopedia Link](https://www.investopedia.com/terms/r/rsi.asp)

### Example:

```
r = RSI(close, 14)
```

This computes the 14-period RSI of the **closing price**.
