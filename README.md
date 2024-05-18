# Trading-and-Analysis

Instructions for Using the Stock Market Calculator on JDoodle
Overview
This Java application performs various stock market calculations using static data. The calculations include:

Dividend Yield
P/E Ratio
Volume Weighted Stock Price (VWSP)
All Share Index
The results are printed directly to the console.

How to Run the Application on JDoodle
Open the JDoodle Link:

Click on the following link to open the JDoodle project:
JDoodle Project
Review the Code:

The code for the Stock Market Calculator is already provided in the JDoodle editor.
Run the Code:

Click the "Execute" button located at the top of the JDoodle editor to compile and run the program.
Review the Output:

The output will be displayed in the console section below the editor.
Example Output
The output will display the results of the calculations for the static data provided in the code. Below is an example of what you should see:

yaml
Copy code
Calculations for static data:

Dividend Yield for TEA at price 100: 0.0
Dividend Yield for COF at price 200: 0.02

P/E Ratio for MIL at price 120: 15.0

VWSP for MIL: 113.0

All Share Index: 113.0
Understanding the Calculations
Dividend Yield:

For an ordinary share: Dividend Yield = Last Dividend / Price
For a preferred share: Dividend Yield = (Fixed Dividend * Par Value) / Price
Example: For TEA at price 100, the dividend yield is 0.0 because the last dividend is 0.
P/E Ratio:

P/E Ratio = Price / Dividend
Example: For MIL at price 120, the P/E ratio is 15.0 because the last dividend is 8.
Volume Weighted Stock Price (VWSP):

VWSP = (Sum of (Traded Price * Quantity)) / (Sum of Quantity)
Example: For MIL, after recording trades, the VWSP is 113.0.
All Share Index:

Calculated as the geometric mean of VWSPs for all stocks.
Example: Given the provided trades and stocks, the All Share Index is calculated.
Modifying the Static Data
To test different scenarios, you can modify the static data directly in the JDoodle editor. Here’s how you can do it:

Adding Stocks:

Use the addStock method to add new stocks.
Example:
java
Copy code
market.addStock(new Stock("XYZ", "Ordinary", 5, 0, 100));
Recording Trades:

Use the recordTrade method to record new trades.
Example:
java
Copy code
market.recordTrade("XYZ", 200, "buy", 105);
market.recordTrade("XYZ", 150, "sell", 110);
Execute the Code:

Click the "Execute" button again to see the updated results.
