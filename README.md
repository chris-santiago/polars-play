# Comparing Pandas, Polars and Vaex

Using 2019-2022 data from [NYC Taxi Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).

Number of rows: 179,807,942
Dataset size: 24.4GB

## Performance

|Framework|Read|Groupby|Total
|---|---|---|---|
|Pandas|dies|n/a|n/a|
|Polars|1ms|2.3s|2.3s|
|Vaex|416ms|5.3s|5.3s|

### Notes

- Data is stored in parquet files on local disk
- Using M1 MBA with 8GB RAM-- unsure how memory swap impacts result