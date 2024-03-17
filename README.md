# Heikin Ashi Volume Weighted for MT5 ReadMe File

This code is a custom indicator for MetaTrader 5 (MT5) called Heikin Ashi Volume Weighted. It is designed to reduce false reversals in trading by calculating Heikin Ashi candles and volume-weighted highs and lows.

## Features

- Heikin Ashi Candles: The indicator calculates Heikin Ashi values for each candle. Heikin Ashi candles are calculated based on the open, high, low, and close prices of each candle.
- Average Volume Calculation: The indicator calculates the average volume over a specified period. This is used to adjust the trailing of highs and lows.
- Volume-weighted Highs and Lows: The indicator calculates volume-weighted highs and lows by adding or subtracting a multiplier based on the current volume compared to the average volume. This helps to reduce false reversals in trading.

## Input Parameters

- Period: The period for calculating the average volume.
- Multiplier: The multiplier for adjusting the trailing of highs and lows.

## Indicator Buffers

- UpBuffer: Stores the Heikin Ashi open values when the close is higher than the open. Otherwise, it is set to EMPTY_VALUE.
- DownBuffer: Stores the Heikin Ashi close values when the close is lower than the open. Otherwise, it is set to EMPTY_VALUE.
- MaxExcursionUpBuffer: Stores the volume-weighted highs.
- MaxExcursionDownBuffer: Stores the volume-weighted lows.

## Initialization

The indicator initializes by mapping the indicator buffers and setting the indicator labels.

## Calculation

The indicator calculates the average volume using the iMAOnArray function. Then, for each candle, it calculates the Heikin Ashi values, volume-weighted highs and lows, and stores them in the respective buffers.

## Usage

This code serves as a sample of how the Heikin Ashi Volume Weighted indicator can be implemented. It is not the official developer's code. To find the official developer of this product, please refer to the MQL5 website.

For detailed reviews and trading results of this product, you can visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/heikin-ashi-volume-weighted-for-mt5-reducing-false-reversals/).

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work similarly to the product's description.
