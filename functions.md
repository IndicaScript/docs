# Functions

These are builtin functions that corresponds to functions within ThinkScript

## SMA (Simple Moving Average)

`SMA(price, length)`

Calculates the **Simple Moving Average** of the given `price` over the past `length` candlesticks.

[Investopedia Link](https://www.investopedia.com/terms/s/sma.asp)

### Example:

`smaValue = SMA(close, 14)`

This calculates the 14-period simple moving average of the **closing price**.

## WMA (Weighted Moving Average)

`WMA(price, length)`

Calculates the **Weighted Moving Average** of the given `price` over the past `length` candlesticks.

[Investopedia Link](https://www.investopedia.com/ask/answers/071414/whats-difference-between-moving-average-and-weighted-moving-average.asp)

### Example:

`wmaValue = WMA(close, 14)`

This calculates the 14-period weighted moving average of the **closing price**.

