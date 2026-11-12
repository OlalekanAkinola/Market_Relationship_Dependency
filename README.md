Testing Popular Market Relationships with Rolling Correlations

This project tests whether some of the best-known relationships across the foreign-exchange, commodity, equity and bond markets have remained reliable over the past five years.

Using daily market data, the analysis calculates 20-day and 60-day rolling correlations to show how these relationships change over time. It also compares their average strength, absolute strength, directional consistency and latest 60-day reading.

Market Relationships Tested

Relationship

Traditional expectation

Gold vs DXY

Negative

Gold vs US 10-Year Treasury yield

Negative

EUR/USD vs GBP/USD

Positive

DXY vs S&P 500

Usually negative

AUD/JPY vs S&P 500

Positive

USD/JPY vs US 10-Year Treasury yield

Positive

Instruments and Yahoo Finance Tickers

Instrument

Ticker

Gold Futures

GC=F

US Dollar Index

DX-Y.NYB

EUR/USD

EURUSD=X

GBP/USD

GBPUSD=X

S&P 500

^GSPC

AUD/JPY

AUDJPY=X

USD/JPY

JPY=X

US 10-Year Treasury Yield

^TNX

Methodology

Download five years of daily closing data with yfinance.

Align the instruments by date and remove observations where either market has missing data.

Calculate daily percentage changes rather than correlating the price levels directly.

Calculate 20-day and 60-day rolling correlations for each relationship.

Compare the relationships using:

Mean 60-day correlation

Mean absolute 60-day correlation

Directional consistency

Latest 60-day correlation

The 20-day correlation captures shorter-term changes in market behaviour, while the 60-day correlation provides a smoother view of the underlying relationship.

How to Interpret the Results

Correlation ranges from -1 to +1:

A value close to +1 indicates that both instruments generally move in the same direction.

A value close to -1 indicates that they generally move in opposite directions.

A value close to 0 indicates a weak or inconsistent linear relationship.

Directional consistency measures the percentage of valid rolling windows in which a relationship moved in its traditionally expected direction. Mean absolute correlation measures strength regardless of whether the relationship was positive or negative.

Key Question

The purpose of the project is not simply to confirm that these relationships exist. It is to determine:

Which traditional market relationships remain strong and dependable, and which ones are weakening or changing under current market conditions?

Tools Used

Python

pandas

NumPy

yfinance

Matplotlib

Jupyter Notebook


Important Note

Correlation does not imply causation, and market relationships are not permanent. Their strength and direction can change because of monetary policy, inflation expectations, interest-rate movements, geopolitical events and shifts in investor risk sentiment. The results should therefore be treated as analytical context rather than trading signals.

Author

Olalekan Akinola
Market Analyst | Investment Research | Financial Data Analytics

- [GitHub Profile](https://github.com/OlalekanAkinola)

- [LinkedIn](https://www.linkedin.com/in/olalekan-akinola)

- [Olalekan Akinola](https://olalekanakinola.substack.com/)


Disclaimer

This project is for educational and research purposes only. It does not constitute investment advice or a recommendation to buy or sell any financial instrument.
