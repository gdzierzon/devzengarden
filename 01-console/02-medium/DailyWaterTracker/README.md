# The Daily Water Drinking Tracker

Water is the source of life, and yet for some it is difficult to drink enough water every day. This CLI is intended to allow a user to enter the how much water they drink each day, and store the data in a .csv file.

A user should also be able to run a report to see how much water they drank on a given day.

The application should write to a single .csv file (e.g. `WaterData.csv`).

Prompt the user if they wish to log a drink, or run a report.

```
What would you like to do?

1) Log water consumption
2) Run drinking reports
3) Exit

Please select an option: 
```

If the user chooses to log water consumption they should be prompted for data.

``` 
Enter the date of consumption (Blank = today): 2022-03-19
How much water did you drink (ounces)? 64

64 oz has been logged for 2022-03-19
```

The report should display 1 row for each date, and include a total amount of water that was consumed on that date.

```
Date            Water Consumption
----------      -----------------
2022-03-18      80 oz
2022-03-19      68 oz
...
```

All data that is input by the user should be written to the `WaterData.csv` file so that the data is available for reporting in the future.

```
WaterData.csv

2022-03-18,32
2022-03-18,32
2022-03-18,16
2022-03-19,64
2022-03-19,4
```
