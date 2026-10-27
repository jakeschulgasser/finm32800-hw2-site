# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ)

Daily ohlcv-1d bars from the CME Globex dataset (GLBX.MDP3), pulled with the parent symbol ZQ.FUT, which returns every listed ZQ contract. Columns: date, symbol, open, high, low, close, volume. The data includes calendar-spread symbols such as ZQU6-ZQZ6 alongside the outright monthly contracts such as ZQU6; filter to outrights before use. A contract settles at 100 minus the average effective fed funds rate over its month, so the implied rate is 100 minus the close. Thinly traded contracts may have no bar on some days, and the single year digit in a symbol is ambiguous across decades.


## DataFrame Glimpse

```
Rows: 11751
Columns: 7
$ date   <datetime[ns]> 2026-10-25 00:00:00
$ symbol          <str> 'ZQF7'
$ open            <f64> 95.895
$ high            <f64> 95.895
$ low             <f64> 95.89
$ close           <f64> 95.895
$ volume          <u64> 396


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ)                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Futures, Fed Funds, Monetary Policy                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Python client                                                   |
| Data available up to (min)     | 2026-10-25 00:00:00                                                             |
| Data available up to (max)     | 2026-10-25 00:00:00                                                             |
| Dataframe Path                 | C:\Users\Jake Schulgasser\projects\hw2-jakeschulgasser\_data\fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file://C:/Users/Jake Schulgasser/projects/hw2-jakeschulgasser/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-26 22:37:34           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

