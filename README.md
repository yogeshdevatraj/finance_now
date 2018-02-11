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

2. Parse data in ```expenses.json``` and show total amount per each month
Amount - field ```amount```
Date   - field ```posting_date```

3. From ```accounts.json``` find out the account type (capex or opex)  from ```expense_type``` field.
And now display Total Capex amount and Opex Amount (per month) separately based on account number represented by field ```account_number```.

4. Draw ***Bar chart*** based on the data derived from Task 3.
```x-axis: months, y-axis : amount```

5. Build inline search for Account Numbers by Name or number.
   As you type it should show top 3 results.




[local-app-url]: http://localhost:8000/index.html
[node]: https://nodejs.org/
