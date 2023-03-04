# Comparing Pandas, Polars and Vaex

Using 2019-2022 data from [NYC Taxi Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).

Number of rows: 176,408,393
Dataset size: 25.4GB

## Performance

|Framework|Read|Groupby|Total
|---|---|---|---|
|Pandas|dies|n/a|n/a|
|Polars|28ms|19.1s|19.1s|
|Vaex|416ms|5.3s|5.3s|

### Notes

- Data is stored in parquet files on local disk
- Using M1 MBA with 8GB RAM-- unsure how memory swap impacts result