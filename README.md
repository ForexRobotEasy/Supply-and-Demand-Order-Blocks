# Supply and Demand Order Blocks Indicator ReadMe

## Description
The Supply and Demand Order Blocks indicator is a custom indicator developed by forexroboteasy.com. It helps identify supply and demand zones in the market. Supply zones are areas where sellers are likely to enter the market, while demand zones are areas where buyers are likely to enter the market.

For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/review-supply-demand-order-blocks-forex-indicator/). Please note that ForexRobotEasy is not the official developer of this product. We are only showing sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## User-defined Input Parameters
- **period**: Period for identifying supply and demand zones. Default value is 20.

## Indicator Buffers
- **supplyBuffer[]**: Buffer array to store the supply zone values.
- **demandBuffer[]**: Buffer array to store the demand zone values.

## Indicator Initialization
The `OnInit()` function is called during indicator initialization. It sets up the indicator's properties, such as styles, arrows, and buffers. It also sets the indicator labels.

## Custom Indicator Logic
The `OnCalculate()` function is called for each new tick. It calculates the supply and demand zones based on the input parameters and price data.

1. It iterates through the price data from the `period` index to the last index.
2. For each index, it initializes the `highestHigh` and `lowestLow` variables with the corresponding price values.
3. It then iterates through the price data from the `i - period` index to the current index to identify the highest high and lowest low values within the period.
4. The identified highest high value is stored in the `supplyBuffer` array at the current index.
5. The identified lowest low value is stored in the `demandBuffer` array at the current index.
6. The process is repeated for each index until the end of the price data.

## Usage
To use this indicator, follow these steps:
1. Open the MetaEditor in MetaTrader.
2. Create a new indicator and paste the code into it.
3. Compile the code.
4. Attach the indicator to a chart in MetaTrader.
5. Adjust the input parameters as desired.
6. The indicator will plot arrows indicating the supply and demand zones on the chart.

Please note that this is a sample code provided by forexroboteasy.com. To find the official developer of this product, please use MQL5.

For more information and detailed reviews of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/review-supply-demand-order-blocks-forex-indicator/).
