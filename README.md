# pinescript-mmi_signal
Trend trading strategies filtered by the Market Meanness Index.

This is a port of the experiment described at

    http://www.financial-hacker.com/boosting-systems-by-trade-filtering/
    http://www.financial-hacker.com/trend-delusion-or-reality/
    http://www.financial-hacker.com/trend-and-exploiting-it/
    http://www.financial-hacker.com/whites-reality-check/

The Market Meanness Index tells whether the market is currently moving in or out of a "trending" regime. 
It can this way prevent losses by false signals of trend indicators. It is a purely statistical algorithm
and not based on volatility, trends, or cycles of the price curve.

The indicator measures the meanness of the market - its tendency to revert to the mean after pretending
to start a trend. If that happens too often, all trend following systems will bite the dust.

## Inputs

- `Price Source`: Either open, high, low, close, hl2, hlc3, or ohlc4. The default value is hlc3.
- `Trend MA Type`: Either SMA, EMA, LowPass, Hull MA, Zero-Lag MA, ALMA, Laguerre, Smooth, Decycle. The default value is LowPass.
- `Trend MA Period`: Sets the lookback period of trend MA. The default value is 200.
- `MMI Period`: Sets the lookback period of the Market Meanness Index. The default value is 300.
