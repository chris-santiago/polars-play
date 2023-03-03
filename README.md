# Comparing Pandas, Polars and Vaex

Using 2020-2022 data from [NYC Taxi Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).

Number of rows: 91,809,949
Dataset size: 12.4GB

## Performance

|Framework|Read|Groupby|Total
|---|---|---|---|
|Pandas|23.2s|8.7s|31.9s|
|Polars|11s|17.2s|28.2s|
|Vaex|428ms|2.8s|2.8s|

### Notes

- Data is stored in parquet files on local disk
- Using M1 MBA with 8GB RAM-- unsure how memory swap impacts result