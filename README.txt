**/Steps followed

Sample data set was taken from the internet and imported to create a balance sheet report from scratch in Power BI.
Appended "assets", "equity" and "liabilities" table into one and labelled as "Item".
Merged queries of "Item" table with "Structure" table and labelled the new table as "Balance Sheet".
Sorted "Item" in the "Balance Sheet" table with respect to the "Code" column.
"Balance Sheet" table was used to visualize and build the report.
1 calculated column and 4 measures were created


**/DAX Used

1. Change in the last two years (£m) = [2021 (£m)] - [2020 (£m)]
2. Total Assets in 2021 = CALCULATE(SUM('Balance Sheet'[2021 (£m)]),'Balance Sheet'[Class] = "Assets" )
3. Total Equity in 2021 = CALCULATE(SUM('Balance Sheet'[2021 (£m)]),'Balance Sheet'[Class] = "Equity")
4. Total Liabilities in 2021 = CALCULATE(SUM('Balance Sheet'[2021 (£m)]),'Balance Sheet'[Class] = "Liabilities") 


**/The company logo used in the report is only for visualization purpose and has no relation to the data shown in the report.
