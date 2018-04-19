# `finance_now`


### Instructions

Use any setup : either local or [plnkr](https://plnkr.co/edit) OR [jsfiddle](https://www.jsfiddle.net) OR [jsbin](https://www.jsbin.com)

You are free to use any framework like AngularJS or jQeury or ReactJS

### Tasks

1. Fetch data in files [```fiscal_period.json``` and ```expenses.json``` under **resource** folder] OR
load data from URIs:
    - Fiscal periods: https://api.myjson.com/bins/180vgz
    - Expenses: https://api.myjson.com/bins/ebk3n
 
    And show the total records in UI using AJAX call.

    **Expected result:**  Records in  Fiscal Periods : \<COUNT> | Records in Expenses : \<COUNT>

2. Display Expense line for selected Fiscal Period.
    a. UI should have simple drop down to select fiscal periods
    b. Should show only those expenses which fall in that fiscal period.

    Use ```posting_date``` from expenses to compare date with fiscal period fields ```fiscal_start_date_time``` and ```fiscal_end_date_time```.
    
    Ideally ```fiscal_start_date_time``` <= ```posting_date``` <= ```fiscal_end_date_time```


3. Aggregate Expense lines per Fiscal Periods(Month)

Parse data in ```expenses``` and show total amount per each **fiscal periods**
Amount - field ```amount``` //in expenses
Date   - field ```posting_date``` //in expenses

Months are those which have ```"fiscal_type" = "month"``` in fiscal periods

    **Expected result:**
    Month wise data in a table format

    | Fiscal Period | Amount    |
    | ------------- |----------:|
    | FY18: M01     | 1600.12   |
    | FY18: M02     | 12121.90  |
    | ...           |      ...  |


4. Improve above task to provide choice of fiscal types: month, quarter or year

Add a drop down to choose aggregation type. 
It can be either month, quarter or year which would be driven by fiscal_type.


