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

## Full Data dataset
* No duplicate rows.
* No missing values in rows.
* Corrected the `date` column being ```object``` datatype instead of ```datetime```.
* Changed numbers to be standard notation instead of scientific notation for readability.