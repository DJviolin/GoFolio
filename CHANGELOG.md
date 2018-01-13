1.0.6 / 2018-01-13
==================

  * New columns: `Price IF total supply $` shows what the price will be if Total Supply kicks in immediately. `Price IF max supply $` shows what the price will be if Max Supply kicks in. Read about what are Circulating, Max, Total supply is on [CoinMarketCap FAQ](https://coinmarketcap.com/faq/). `Unreleased coins %` shows the coins that's not released at all right now (eg. keeping for scheduled release or themselves, because it's a stupid scam).

1.0.5 / 2018-01-13
==================

  * Green cells means in `Portfolio` and `Info` tables that you should edit it.

1.0.4 / 2018-01-13
==================

  * CoinMarketCap API had a massive slowdown in response times in the last weeks. I had to drop every query strings from url except `?limit=0` which seems like fixing the `DataSource.Error` most of the time.
  * Re-design
  * New table columns
  * Now you can specifiy your initial investments in `Info` table.
  * Colored price changes columns at -5%, 0, 20% via Conditional Formatting.

1.0.3 / 2017-12-28
==================

  * Github repository launched with big fat donation links, hence the important version pump. :)

1.0.2 / 2017-12-27
==================

  * In the `Info` table at `B1` cell, you can define your national currency easily. In `B2` cell, the `1 USD to <your-currency>` value is calculated by a formula. EUR also calculated with an if else, originally not part of ECB API.

1.0.1 / 2017-12-26
==================

  * European FIAT currencies added into ECB table from the European Central Bank API.


1.0.0 / 2017-12-25
==================

  * Initial release
