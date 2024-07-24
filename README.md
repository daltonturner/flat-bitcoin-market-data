# Bitcoin Market Data

*Note:* Github actions for this repo have been disabled. Archiving to maintain a reference. 

A [Flat Data](https://octo.github.com/projects/flat-data) GitHub Action demo repo that pulls market data for Bitcoin from the markets api on [Bitcoincharts.com](https://bitcoincharts.com/about/markets-api/) using a cron job. 

The resulting `.json` file is updated every five minuets, keeping the data fresh and explorable through the Flat Viewer UI [here](https://flatgithub.com/daltonturner/flat-bitcoin-market-data?filename=btc-market-data.json&sha=38246b6899899b2adc3ef150fac7b0d80af604d5).

---

According to [Bitcoincharts.com](https://bitcoincharts.com/about/markets-api/), the column descriptions for returned fields are as follows:

- **symbol**: short name for market
- **currency**: base currency of the market (USD, EUR, RUB, JPY, ...)
- **bid**: highest bid price
- **ask**: lowest ask price
- **latest_trade**: unixtime of latest trade. Following fields relate to the day of this field (UTC)!
- **n_trades**: number of trades
- **high**: highest trade during day
- **low**: lowest trade during day
- **close**: latest trade
- **previous_close**: latest trade of previous day
- **volume**: total trade volume of day in BTC
- **currency_volume**: total trade volume of day in currency
