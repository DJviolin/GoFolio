# GoFolio

Your personal cryptocurreny portfolio, no more spying in what you have!

## Motivation:

The origin of the spreadsheet was in [this](https://www.reddit.com/r/ethtrader/comments/6b16fk/how_to_import_coinmarketcap_data_into_excel_and/) subreddit. This example creating new API requests for every coin. If you have a dozen coin to watch and you working in the spreadsheet, this means every 1 minute your spreadsheet is blocked for 5-10 seconds until flashing through every API request and it's highly annoying.

I achieved this simplified table structure with the help of [INDEX & MATCH](https://www.ablebits.com/office-addins-blog/2014/08/13/excel-index-match-function-vlookup/) formulas.

My modification only requires two API requests: one for [CoinMarketCap](https://coinmarketcap.com/api/) (every minute) and one for the [European Central bank](http://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html) (60 minute).

Which is my another addition: auto-updating fiat currencies, if your national currency different then USD. Right now, only European Union currencies supported.

## Requirements

* Microsoft Office Excel 2016
* If you use older version, you need to have [Power Query](https://www.microsoft.com/en-us/download/details.aspx?id=39379) installed.
* Make sure that the Decimal separator is set to dot (.) rather then comma (,), otherwise the formulas not work. You can set it in `File -> Options -> Advanced` window and uncheck `Use system separators` and set `Decimal separator` to `.`.
* All formulas written in their english form. If some formulas not work, install english language pack.

## Usage

1. Set your national currency at `Info` table in `B1` cell.
2. In the `Portfolio` table, rename the wallet/exchange headers to the ones you use. Feel free to delete or add new columns.
3. Enter your coins into the green area. Feel free to delete or add new lines.
4. If a coin is not included, duplicate a coin line, then change the name in column `A` and enter your values in the wallets. One thing to note that the name needs to match with the one in `Ticker` table with `Coin.symbol` column. Otherwise formulas not gonna work.
5. Final step: watch your money burns (in 1 minute intervals)...

## TODO

* Implement [CrytoCompare](https://www.cryptocompare.com/api) API and test against CoinMarketCap.
* After CoinMarketCap releasing the historical API, implement growth rate

## Donations

Although you can laugh that I launched a repo for an Excel table, but my future commercial pilot training highly under financed right now, so donations are welcome!

**ETH:** 0x9d9c860158d6f4AE0696c9783A7B9d8d85206Cee

**BTC:** 13nE3VP2L9mthVcj3o6cSsV2745HGEaEsG

**DOGE:** DEoPGWAqFF986yK6MwJLv71fVoNFHFSfPw
