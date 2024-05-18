# Stock Market Calculator Application

## Overview

This Java application performs various stock market calculations using static data. The calculations include:
- Dividend Yield
- P/E Ratio
- Volume Weighted Stock Price (VWSP)
- All Share Index

The results are printed directly to the console.

## How to Run the Application on JDoodle

1. **Open the JDoodle Link**:
   - Click on the following link to open the JDoodle project:
     [JDoodle Project](https://www.jdoodle.com/a/7CD8)

2. **Review the Code**:
   - The code for the Stock Market Calculator is already provided in the JDoodle editor.

3. **Run the Code**:
   - Click the **"Execute"** button located at the top of the JDoodle editor to compile and run the program.

4. **Review the Output**:
   - The output will be displayed in the console section below the editor.

## Example Output

The output will display the results of the calculations for the static data provided in the code. Below is an example of what you should see:




## Understanding the Calculations

1. **Dividend Yield**:
   - For an ordinary share: `Dividend Yield = Last Dividend / Price`
   - For a preferred share: `Dividend Yield = (Fixed Dividend * Par Value) / Price`
   - Example: For `TEA` at price 100, the dividend yield is `0.0` because the last dividend is `0`.

2. **P/E Ratio**:
   - `P/E Ratio = Price / Dividend`
   - Example: For `MIL` at price 120, the P/E ratio is `15.0` because the last dividend is `8`.

3. **Volume Weighted Stock Price (VWSP)**:
   - `VWSP = (Sum of (Traded Price * Quantity)) / (Sum of Quantity)`
   - Example: For `MIL`, after recording trades, the VWSP is `113.0`.

4. **All Share Index**:
   - Calculated as the geometric mean of VWSPs for all stocks.
   - Example: Given the provided trades and stocks, the All Share Index is calculated.

## Modifying the Static Data

To test different scenarios, you can modify the static data directly in the JDoodle editor. Here’s how you can do it:

1. **Adding Stocks**:
   - Use the `addStock` method to add new stocks.
   - Example:
     ```java
     market.addStock(new Stock("XYZ", "Ordinary", 5, 0, 100));
     ```

2. **Recording Trades**:
   - Use the `recordTrade` method to record new trades.
   - Example:
     ```java
     market.recordTrade("XYZ", 200, "buy", 105);
     market.recordTrade("XYZ", 150, "sell", 110);
     ```

3. **Execute the Code**:
   - Click the **"Execute"** button again to see the updated results.

## Troubleshooting

- If you encounter any errors during execution, check for typos or missing parts of the code.
- Ensure the JDoodle editor is fully loaded and you have a stable internet connection.

## Conclusion

By following these instructions, you can easily run the Stock Market Calculator application on JDoodle, review the results, and modify the static data for further testing. This setup provides a convenient way to understand and verify the stock market calculations performed by the application.
