### For Java Developer Only

### Instructions
A MySQL instance with & expense_line & fiscal_period table are given.
We will provide IP and port for the MySQL DB instance.
OR 
You can use your own local development instance to connect using JDBC.

### Tasks
0. Get development setup done. Connected to mysql, and server up and running.

## Build APIs for 
1. Get Fiscal Period for given date.
Ideally ```fiscal_start_date_time``` <= ```given_date``` <= ```fiscal_end_date_time```
```getFiscalPeriod(date)``` // dates in string format
return: ```name``` of fiscal period.

2. Get Fiscal periods between date range ```getFiscalPeriods(start, end)``` // dates in string format
return: List<String> of fiscal periods with ```name``` of fiscal period.

3. Add support above to APIs for type of fiscal period.
type is driven by property: ```fiscal_type``` and values could be month, quarter and year.
```getFiscalPeriod(date, fiscalType)``` and ```getFiscalPeriods(start, end, fiscalType)```
Usecase: When requested for only quarter types, we should get only quarters.

4. Get expenses occurred between two dates ```getExpenses(start, end)```.
 Use ```posting_date``` in expenses table to compare dates
return: List<String> of expenses. Expense with ```posting_date``` and ```amount``` in string

5. Get expenses occurred in given fiscal period
```getExpenses(fiscalPeriod) //fiscalPeriod could be of pojo class or sys_id of fiscal_period```