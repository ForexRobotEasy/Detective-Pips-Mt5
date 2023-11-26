# Detective Pips MT5 ReadMe

## Description
This ReadMe file provides an overview of the code for the Detective Pips MT5 Expert Advisor. The code is written by Forex Robot Easy Team and is intended for use in the MetaTrader 5 (MT5) platform. This Expert Advisor is designed to identify breakouts in the forex market and place pending orders with defined take profit and stop loss levels. The code includes input parameters for spread, commission, and risk tolerance, which can be adjusted by the user. The Expert Advisor also includes custom functions to adjust the trailing stop and close trades if the market changes direction. 

Please note that Forex Robot Easy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 platform.

## Developer Information
- Developer: Forex Robot Easy Team
- Developer's Site: forexroboteasy.com

## Input Parameters
- spread: The required minimum spread for the Expert Advisor to place pending orders. Default value is 0.5.
- commission: The required minimum commission for the Expert Advisor to place pending orders. Default value is 0.1.
- riskTolerance: User-defined risk tolerance for setting take profit and stop loss levels. Default value is 2.0.

## Global Variables
- previousHigh: Holds the previous high value.
- previousLow: Holds the previous low value.
- trailingStop: Holds the trailing stop value.

## Initialization Function (OnInit)
- Retrieves the previous high and low values from the previous candle.
- Sets the initial trailing stop based on the previous high and low values.

## Expert Advisor Start Function (OnTick)
- Calculates the current high and low values from the previous candle.
- Checks if the current high is greater than the previous high or if the current low is lower than the previous low (indicating a breakout).
- If a breakout occurs, places pending orders with defined take profit and stop loss levels.
- Prints a message indicating the success or failure of placing pending orders.
- Updates the previous high and low values.

## Custom Function to Adjust Trailing Stop (AdjustTrailingStop)
- Calculates the current high and low values from the previous candle.
- Updates the trailing stop value based on the market direction (if the current high is greater than the previous high or if the current low is lower than the previous low).

## Custom Function to Close Trades if Market Changes Direction (CloseTrades)
- Checks if there are any open trades.
- Loops through open trades and closes them if the market changes direction (if the current low is lower than the opening price of a buy trade or if the current high is greater than the opening price of a sell trade).

## Expert Advisor Deinitialization Function (OnDeinit)
- Closes all open trades when the Expert Advisor is deinitialized.

## Product Description
Detective Pips MT5 is a profitable non-martingale Expert Advisor developed by the Forex Robot Easy Team. It is designed to identify breakouts in the forex market and place pending orders with defined take profit and stop loss levels. The Expert Advisor is optimized for the MetaTrader 5 (MT5) platform and can be used with any currency pair. It includes input parameters for spread, commission, and risk tolerance, allowing users to customize their trading preferences. The Expert Advisor also includes custom functions to adjust the trailing stop and close trades if the market changes direction. For detailed reviews and trading results of this product, please visit [forexroboteasy.com/forex-robot-review/detective-pips-mt5-review-profitable-non-martingale-ea/](https://forexroboteasy.com/forex-robot-review/detective-pips-mt5-review-profitable-non-martingale-ea/). Please note that Forex Robot Easy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 platform.
