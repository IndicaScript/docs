# Variables

Variables are ways to store values to be used elsewhere. Users can store their own variables, but there are some builtin variables.

## Creating Variables

You can create variables like so:

```
length = 14
smaValue = SMA(close, length)
wmaValue = WMA(close, length)
```

Variables can then be referenced anywhere after that in your code.

## Builtin Variables

> Scripts typically run once per candlestick, so these variables refer to values specific to that candle (time period).

### open

`open` represents the opening price of the current candlestick.

### close

`close` represents the closing price of the current candlestick.

### upticks

`upticks` represents the number of price changes (ticks) during the current candlestick where the price moved **upward**.
It can be used as a proxy for **buying pressure** or **bullish activity** within the candle's timeframe.

### downticks

`downticks` represents the number of price changes (ticks) during the current candlestick where the price moved **downward**.
It serves as a proxy for **selling pressure** or **bearish activity** within the current candlestick.
