# `finance_now`


### Instructions

Use any setup : either local or ![plunkr][plunkr] or ![jsbin][jsbin] or ![jsfiddle][jsfiddle]

You are free to use any framework like AngularJS or jQeury or ReactJS

### Tasks

1. Fetch data in files [```accounts.json``` and ```expenses.json``` under **resource** folder] and show the total records in UI using AJAX call.

    **Expected result:**  Records in  Accounts: <COUNT> | Records in Expenses: <COUNT>

2. Parse data in ```expenses.json``` and show total amount per each **month**
Amount - field ```amount```
Date   - field ```posting_date```

    **Expected result:**
    Month wise data in a table format

    | Month         | Amount    |
    | ------------- |----------:|
    | Jan 2018      | 1600.12   |
    | Feb 2018      | 12121.90  |
    | ...           |      ...  |


3. From ```accounts.json``` find out the account type (capex or opex)  from ```expense_type``` field.
And now display Total Capex amount and Opex Amount (per month) separately based on account number represented by field ```account_number```.

    **Expected result:**
    
    |Month          |Capex Amount | Opex Amount |   Total |
    | ------------- |----------:|----------:|----------:|
    | Jan 2018      | 1600.00  | 1800.40 |   3400.40     |
    | Feb 2018      | 12121.90  | 1234.05| 14355.95      |
    | ...           |      ...  | ...    |...            |

4. Draw ***Bar chart*** based on the data derived from Task 3.
```x-axis: months, y-axis : amount```

    ![Chart][chart]

5. Build inline search for Account Numbers by Name or number.
   As you type it should show top 3 results.

[chart]: https://github.com/ServiceNow-Hiring/finance_angular/blob/master/resource/chart.png
[plunkr]: https://www.plunkr.co
[jsbin]:https://www.jsbin.com
[jsfiddle] https://www.jsfiddle.com
