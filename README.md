# `finance_angular` — the starter for AngularJS apps

Starter for angular


### Prerequisites


You must have Node.js and its package manager (npm) installed. You can get them from [here][node].


### Install Dependencies

We have preconfigured `npm` to automatically run `bower` so we can simply do:

```
npm install
```

### Run the Application

We have preconfigured the project with a simple development web server. The simplest way to start
this server is:

```
npm start
```
Now browse to the app at [`localhost:8000/index.html`][local-app-url].

### Tasks

1. Fetch data in files [```accounts.json``` and ```expenses.json``` under **resource** folder] and show the total records in UI.

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
    | Jan 2018      | 1600.00  | 1800.40 |   3400.40 |
    | Feb 2018      | 12121.90  | 1234.05| 14355.95|
    | ...           |      ...  | ...|...|

4. Draw ***Bar chart*** based on the data derived from Task 3.
```x-axis: months, y-axis : amount```

    ![Chart][chart]

5. Build inline search for Account Numbers by Name or number.
   As you type it should show top 3 results.


[local-app-url]: http://localhost:8000/index.html
[node]: https://nodejs.org/
[chart]: https://github.com/ServiceNow-Hiring/finance_angular/blob/master/resource/chart.png
