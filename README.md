# Order Blocks ICT MT5

This code is a custom indicator for MetaTrader 5 (MT5) that identifies order blocks on a specified time frame. Order blocks are areas of support and resistance on a price chart that are formed by institutional traders. The indicator calculates the highest high and lowest low for a given period and then determines if the current period is an order block based on a sensitivity level.

## Input Parameters

- TimeFrame: The time frame to use for identifying order blocks. The default is H1 (1 hour).
- OrderBlockPeriods: The number of periods to consider for order blocks. This determines the size of the order block. The default is 7.
- Sensitivity: The sensitivity level for identifying order blocks. This determines how close the current period's high or low must be to the previous period's high or low to be considered an order block. The default is 0.1.

## Global Variables

- orderBlockTime: The time of the order block.
- orderBlockPrice: The price of the order block.
- isOrderBlockUp: A flag indicating whether the order block is bullish or bearish.

## Custom Indicator Initialization Function

The OnInit function is called when the indicator is initialized. In this function, the indicator buffers are set for storing the order block time, price, and bullish/bearish flag. The indicator label is also set.

## Custom Indicator Iteration Function

The OnCalculate function is called for each new bar of data. In this function, the order blocks are calculated by iterating through the previous periods. The highest high and lowest low for the previous periods are found, and then the current period is checked to see if it qualifies as an order block based on the sensitivity level. If it does, the order block time, price, and bullish/bearish flag are updated. If not, they are set to 0.

## Product Description

**Order Blocks ICT MT5** is a powerful custom indicator for MetaTrader 5 that helps traders identify key areas of support and resistance on a price chart. Developed by ForexRobotEasy Team, this indicator utilizes the concept of order blocks, which are areas where institutional traders place their orders.

By using a specific time frame and sensitivity level, Order Blocks ICT MT5 accurately identifies these order blocks, giving traders an edge in their trading decisions. The indicator displays the time and price of each order block, as well as whether it is bullish or bearish.

With Order Blocks ICT MT5, traders can:

- Identify potential reversal points in the market
- Set more accurate entry and exit points for their trades
- Improve risk management by placing stop-loss orders near order blocks
- Enhance overall trading performance and profitability

Please note that ForexRobotEasy is not the official developer of this product. We provide this sample code to showcase how the indicator works. To find the official developer of Order Blocks ICT MT5 or to access detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/order-blocks-ict-mt5-review-unleashing-market-edge-with-advanced-forex-tool/).

For more information on how to use this indicator and optimize it for your trading strategy, please refer to the MQL5 documentation and resources.
