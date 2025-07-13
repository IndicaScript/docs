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
