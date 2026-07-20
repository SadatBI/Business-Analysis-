DEFINE
    MEASURE 'CalMeasures'[Total_Actual_Revenue] = SUMX(FILTER(NFData,NFData[Revenue/Expenses]="Revenues"),NFData[Actual Amount])
    MEASURE 'CalMeasures'[Total_Budgeted_Revenue] = SUMX(FILTER(NFData,NFData[Revenue/Expenses]="Revenues"),NFData[Budget Amount])
    MEASURE 'CalMeasures'[%_Efficiency_Revenue] = DIVIDE([Total_Actual_Revenue],[Total_Budgeted_Revenue])
    MEASURE 'CalMeasures'[Total_Actual_Expenses] = SUMX(FILTER(NFData,NFData[Revenue/Expenses]="Expenses"),NFData[Actual Amount])
    MEASURE 'CalMeasures'[Total_Budgeted_Expenses] = SUMX(FILTER(NFData,NFData[Revenue/Expenses]="Expenses"),NFData[Budget Amount])
    MEASURE 'CalMeasures'[%_Efficiency_Expenses] = DIVIDE([Total_Budgeted_Expenses],[Total_Actual_Expenses])

EVALUATE
    SUMMARIZECOLUMNS(
        "Total_Actual_Revenue", [Total_Actual_Revenue],
        "Total_Budgeted_Revenue", [Total_Budgeted_Revenue],
        "%_Efficiency_Revenue", [%_Efficiency_Revenue],
        "Total_Actual_Expenses", [Total_Actual_Expenses],
        "Total_Budgeted_Expenses", [Total_Budgeted_Expenses],
        "%_Efficiency_Expenses", [%_Efficiency_Expenses]
    )