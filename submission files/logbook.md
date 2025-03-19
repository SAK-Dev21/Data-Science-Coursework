The purpose of this logbook is to record weekly the progress of this coursework. 

> ## Abbreviations
> * **Trips_by_Distance (1).csv**: Distance dataset
> * **Trips_Full Data (2).csv**: Full Data dataset

# 2.3.25

- The objective of this session was to clean the datasets for ```Trips_by_Distance (1).csv``` and ```Trips_Full Data (2).csv```. I will call Trips by Distance as the **Distance dataset** and Trips Full Data as the **Full Data dataset** from now on. This is so it's simpler to write out.
- I found out that the full data dataset has no missing values nor duplicates, so no work was required for me. The same could not be said for the distance dataset.

## Distance dataset
* Had missing values. So I removed all rows which had missing values.
* Had some columns that were the incorrect data type.
    * `Date` :  Object instead of datetime.
* No duplicate values.
* All values were appropriate to their columns.
* Exported dataset to be used for data analysis.

## Full Data dataset
* No duplicate rows.
* No missing values in rows.
* Corrected the `date` column being ```object``` datatype instead of ```datetime```.
* Changed numbers to be standard notation instead of scientific notation for readability.
* Exported dataset to be used for data analysis.

# 11.3.25

## Full Data (cleaned) dataset

* Calculated weekly averages of the following:
    * Travel distance for those traveling.
    * The weekly number of people of those staying at home.
* Identified high frequency travel days for people who traveled:
    * 10-25 miles.
    * 50-100 miles.
* Created visualisations for both prior bullet points.
    * A histogram for weekly averages.
    * A line chart for high frequency travel days.

# 19.3.25

* Compared the run times of processing with Pandas vs Dask.
* I randomly chose the task for both tools to be finding the mean of a column.
* With Dask, I obtained the results of using 5, 10, 15 and 20 workers. Surprisingly, 10 produced the shortest runtime.
* Even more shockingly, Pandas produced a much quicker time of 0.37 seconds (2dp). This probably is because the dataset is quite short, in comparison to much larger datasets worth terabytes.
    * An apt analogy is having a short list and using Merge sort (Dask) to sort it rather than Bubble sort (Pandas).
* I outputted the results via a line chart of all runtimes
