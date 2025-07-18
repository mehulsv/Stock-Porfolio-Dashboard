# Stock Portfolio Dashboard

A Google Sheets-based stock portfolio dashboard designed to help you track, analyze, and visualize your investment performance. Inspired by tutorials and modern finance dashboard techniques, this template allows both beginners and experienced investors to manage their portfolios efficiently and transparently.

## Features

- **Portfolio Overview**: Real-time summary of total value, gains/losses, and allocation.
- **Stock Tracking**: Auto-updating data tables for each individual stock’s performance.
- **Transactions Log**: Simple interface for recording buys, sells, and dividend activity.
- **Visual Analytics**: Charts for sector allocation, value trends, and performance breakdowns.
- **Customizable**: Easily adapt to your preferred stocks, currencies, and formats.

## How to Use

### 1. Clone or Make a Copy

- Open the dashboard in Google Sheets.
- Go to `File > Make a copy` to save your own editable version.

### 2. Enter Your Portfolio

- Use the `Transactions` sheet/tab to record historical and new transactions (buy/sell/dividend).
- Enter stock tickers as per Yahoo Finance or your data provider’s standards.

### 3. Data Refresh

- Stock prices and related data will auto-update if you use integrated GoogleFinance functions.
- For manual updates, add your own price data to the appropriate columns.

### 4. View Dashboard

- The main dashboard provides key metrics, tables, and visual charts.
- Analyze allocation, performance, and risk at a glance.

## File Structure

| Tab/Sheet       | Purpose                                      |
|-----------------|----------------------------------------------|
| Dashboard       | Main summary with visuals and KPIs           |
| Transactions    | Input for buys, sells, dividends             |
| Stock Data      | Back-end data processing and queries         |
| Lookups         | Reference tables (tickers, sectors, etc.)    |
| Charts          | Source data for main charts                  |

## Customization Tips

- Make sure column formats match your local currency and date formats.
- Double-check that all tickers are correctly spelled and supported.
- Update sector/company metadata as needed in Lookups sheet.
- Adjust chart ranges or calculations if you add more stocks.

## Example QUERY (for advanced users)

Sample query used for sorting data by ascending/descending order (ensure no blanks disrupt your queries):

```excel
=QUERY('Stock Data'!1:1000, "SELECT A,B,E,G,K WHERE K IS NOT NULL ORDER BY K ASC LIMIT 10")
```

## Troubleshooting

- If visuals or data tables appear blank, check for empty cells or formatting inconsistencies (especially in price and ticker columns).
- Ensure all formulas and functions (e.g., `GOOGLEFINANCE`) are enabled and properly referenced.
- For issues with sorting, add `WHERE` clauses in your queries to skip empty data, as demonstrated above.



## Contribution

- Fork the repo and submit pull requests for improvements or bug fixes.
- Please open issues for suggestion or support.

## Disclaimer

This dashboard template is provided for informational and educational purposes only. Always verify financial information with your broker or financial advisor before making investment decisions.

