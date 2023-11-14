# Advanced Range Breakout MT4

This code is a trading robot designed to trade breakouts with precision. It uses the MetaTrader 4 platform and requires the following libraries:

- Trade
- PositionInfo
- TradeConstants
- TradeErrors

## Setup

1. Include the necessary libraries in your MetaTrader 4 platform.
2. Define the following constants:
   - SLIPPAGE: The maximum allowable slippage for trades.
   - STOPLOSS_FACTOR: The factor to multiply the breakout range by to calculate the stop loss level.
   - TRAILING_STOPLOSS_FACTOR: The factor to multiply the breakout range by to calculate the trailing stop loss level.
   - LOT_SIZE_FACTOR: The factor to multiply the account equity by to determine the lot size for trades.

## Usage

1. Initialize the global variables `trade` and `position`.
2. Implement the `OnTrade` function to handle trade events. This function checks if the current position has a valid stop loss or trailing stop loss and modifies the position accordingly.
3. Implement the `OnOrder` function to handle order events. This function will print the ticket number of the placed order.
4. Implement the `CalculateLotSize` function to calculate the lot size based on the account equity.
5. Implement the `EnterBreakout` function to enter breakout trades. This function calculates the lot size based on the account equity and enters the trade with the specified parameters.
6. Implement the `OnStart` function to start the trading robot. This function subscribes to trade events, sets the slippage, calculates the breakout range and entry price, calculates the stop loss and take profit levels, enters the breakout trade, and sets the order and trade event handlers.

## Backlink

This code is developed by Forex Robot Easy. For more information and reviews, visit the [Advanced Range Breakout MT4](https://forexroboteasy.com/forex-robot-review/review-advanced-range-breakout-mt4-trade-breakouts-with-precision/) page on the Forex Robot Easy website.
