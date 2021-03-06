# The Weight Loss/Gain Tracker

Whether your goal is to lose weight or to gain it, you will want to track your progress. This CLI will allow a user to enter a the name of a person, their weight, and date of the weigh in.

A user should also be able to run a report to see the progress of a person over time.

The application should write to a single .csv file (e.g. `WeightTracker.csv`).

Prompt the user if they wish to log a wigh in, or run a report.

```
What would you like to do?

1) Log weight
2) Reports
3) Exit

Please select an option: 
```

If the user chooses to log weight they should be prompted for data.

``` 
Weigh in
----------------------------------------------
Enter the name of the person weighing in: Gary
Enter the date of the weigh in (Blank = today): 2022-03-19
Enter the weight (in pounds)? 172

172 lbs has been logged for Gary on 2022-03-19
```

If a weight is entered for a date that already has a weight tracked, the weight should be overwriten.

When running a report a the user should specify the name of the person for whom the report should be run. They should also specify a date range for which the report whould be run.

```
Reports
-------------------------------------------------
Enter the name of the person for the report: Gary
Start date (Blank = 7 days before today): 2022-03-13
End date (Blank = today): 2022-03-19

```

The report should display 1 row for each date, and include a total amount of water that was consumed on that date.

```
Name: Gary
---------------------------------
Date            Weight
----------      -----------------
2022-03-13      175 lbs
2022-03-14      174 lbs
2022-03-15      175 lbs
2022-03-16      174 lbs
2022-03-17      173 lbs
2022-03-18      172 lbs
2022-03-19      172 lbs
...
```

All data that is input by the user should be written to the `WeightTracker.csv` file so that the data is available for reporting in the future.

```
WeightTracker.csv

Gary,2022-03-12,176
Marin,2022-03-12,111
Gary,2022-03-13,175
Marin,2022-03-13,111
Gary,2022-03-14,174
Marin,2022-03-14,111
Gary,2022-03-15,175
Marin,2022-03-15,110
Gary,2022-03-16,174
Marin,2022-03-16,110
Gary,2022-03-17,173
Marin,2022-03-17,110
Gary,2022-03-18,172
Marin,2022-03-18,110
Gary,2022-03-19,172
Marin,2022-03-19,110
Gary,2022-03-20,171
Marin,2022-03-20,109
Gary,2022-03-21,171
Marin,2022-03-21,109
Gary,2022-03-22,170
Marin,2022-03-22,109
```
