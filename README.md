**S&P 500 Equity Analysis Terminal**
Historical Performance & Fundamental Multiples (2013-2018)

📌 **Project Overview**
This project is a Power BI terminal designed to analyze the fundamental health and market valuation of S&P 500 constituents. By synchronizing time-series pricing data (2013-2018) with fundamental snapshots, the dashboard provides deep insights into valuation "divergence"—identifying when stocks are trading significantly away from their 5-year historical norms.

🛠️ **Tech Stack**
*Power BI Desktop: Dashboard design and visualization.
*Power Query: Advanced data transformation and cleaning layer for reshaping and preparing data, price synchronization, and 52-week windowing.
*Data Modelling: Relationships established among tables to enable cross-filtering and aggregation.
*Financial Data: S&P 500 historical fundamentals and time-series pricing.

📊 **Data Source** (Kaggle)
*The dataset consists of historical S&P 500 fundamentals and stock prices (2013-2018).
*Data Integrity: Pricing data was specifically synchronized to Feb 7, 2018.
*Transformation: Negative P/E values were handled as 0 (N.M.) to prevent skewing.

💡 **Features & Highlights**
**Business Problem**: Standard spot-price P/E ratios are often "noisy." This terminal solves this by introducing Normalised P/E (5-Year Avg) to help analysts identify long-term valuation trends versus short-term market sentiment.

**Key Visuals** 
*Football Field Chart: Visualizes the 52-week trading range vs. current price.
*Scatter Matrix: Maps Dividend Yield vs. Earnings Multiples to find "Quality-Value" outliers.
*Dynamic Valuation Toggle: Uses Field Parameters to switch the entire dashboard between Current and Normalised P/E perspectives.

**Business Impact & Insights** 
This terminal provides a high-density, institutional-grade view of the S&P 500 during a historical window (2013-2018). By comparing Normalised P/E (long-term average) against Current P/E (spot valuation), we can identify significant market inefficiencies and "pricing disconnects."

**1. Core Valuation Insights (The "Divergence" Play)**
*This terminal reveals exactly where the market was potentially "overheating" or "undervaluing" assets relative to their 5-year history.

*Valuation Premium (Growth Overheating): In "Company / Peer Analysis", tickers like WAT, AMD, and CRM show a massive positive divergence. For instance, WAT had a Normalised P/E of 691.1 but a Current P/E of 1,063.1, a divergence of 371.9. This indicates extreme growth expectations that had moved far beyond historical norms.

*Deep Value / Recovery Plays: Conversely, (Screenshot 4) shows companies like CTL and KIM trading at a significant discount to their 5-year averages (Divergences of -11.2 and -11.3 respectively). These represent "mean reversion" candidates where the stock is historically cheap.

*Sector Rotations: The Telecommunication Services sector shows the lowest Current P/E (7.8) alongside the highest Dividend Yield (5.42%), suggesting it was being treated as a "defensive income" sector with little growth priced in.

**2. Risk & Resilience Analysis (52-Week Range)**
*The "Football Field" chart (Screenshot 1) provides a unique look at price momentum relative to historical "floors" and "ceilings."

*The "Top-Heavy" Giants: Large-cap stocks like PCLN (Booking) and AMZN are trading near the very top of their 52-week spreads. This suggests high momentum but limited "headroom" for further gains without a fundamental catalyst.

*Margin of Safety: Stocks in the middle of spread (like REGN or CMG) show a balanced risk-reward profile, as they are not "overextended" toward their yearly highs.

**3. Yield vs. Valuation Strategy**
*The scatter chart (Screenshot 1) maps the "Yield vs. Multiple" relationship, identifying unique outliers.

*The "Yield Trap" Warning: The dots in the far upper-left (High Yield, Low P/E) often signal distress. In the terminal, CTL (Lumen) stands out with a 12.66% yield but a low P/E. This often suggests the market expects a dividend cut.

*The "Sweet Spot" (Bottom-Left): Sectors like Financials and Industrials cluster in the 15x–25x P/E range with 1.5%–2% yields. This represents the "Market Core"—stable valuations with consistent but modest income.


🖼️ **Dashboard Preview**
Dashboard-Sector Analysis - ![Dashboard Preview](https://github.com/kaushal7781/SP500-Equity-Analysis-Terminal/blob/main/1.%20Dashboard%20-%20Sector%20Analysis.png)

Dashboard-Outliers Example - ![Dashboard Preview](https://github.com/kaushal7781/SP500-Equity-Analysis-Terminal/blob/main/2.%20Dividend%20Yield%20Outlier%20-%20CTL.png)

Sector Analysis Focused View - ![Dashboard Preview](https://github.com/kaushal7781/SP500-Equity-Analysis-Terminal/blob/main/3.%20Sector%20Analysis%20-%20Focused%20View.png)

Company/Peer Yield-Valuation Analysis - ![Dashboard Preview](https://github.com/kaushal7781/SP500-Equity-Analysis-Terminal/blob/main/4.%20Company_Peer%20Yield-Valuation%20Analysis.png)

⚠️ **Disclaimer**
This dashboard is for educational and portfolio purposes only. The analysis provided does not constitute financial advice. All valuations are based on historical data points.
