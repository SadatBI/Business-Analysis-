* Expense Efficiency %
  
  %_Efficiency_Expenses = DIVIDE([Total_Budgeted_Expenses],[Total_Actual_Expenses])
  

* Revenue Efficiency %** 
  
  %_Efficiency_Revenue = DIVIDE([Total_Actual_Revenue],[Total_Budgeted_Revenue])
 

* Total Sales
   Total Sales = SUM(Sales[SalesAmount])
  
* Sales YTD
   Sales YTD = TOTALYTD([Total Sales], 'Date'[Date])