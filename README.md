
# Apple Stock Price
Description:

## Questions #1:
Which 10 dates have the highest close stock price in 2013?
```sql
SELECT date,
max(close) as Highest_Close_Price
From datasets.aapl_historical_stock_price
where year = 2013
group by date
order by Highest_Close_Price DESC
limit 10
```
![datasets_aapl_historical_stock_price](visualizations/q1.png)


## Questions #2:
Which 10 dates have the lowest stock price in 2012?
```sql
SELECT date,
min(low) as Lowest_Stock_Price
From datasets.aapl_historical_stock_price
where year = 2012
group by date
order by Lowest_Stock_Price ASC
limit 10
```
![datasets_aapl_historical_stock_price](visualizations/Q2.png)

## Questions #3:
Which 10 dates have the highest volume in 2013?
```sql
SELECT date,
max(volume) as Highest_volume
From datasets.aapl_historical_stock_price
where year = 2013
group by date
order by Highest_volume DESC
limit 10
```
![datasets_aapl_historical_stock_price](visualizations/Q3.png)

## Questions #4:
Which 10 dates have the lowest open price in 2012?
```sql
SELECT date,
min(open) as Lowest_Open_Price
From datasets.aapl_historical_stock_price
where year = 2012
group by date
order by Lowest_Open_Price ASC
limit 10
```
![datasets_aapl_historical_stock_price](visualizations/Q4.png)

## Questions #5:
How many ?
