# Excel Step-By-Step Description
1. Downloaded .csv files from Baltimore City Open Data, converted to .xlsx files (loaced in original_data folder)
2. Copied and pasted datasets into mini_project_3.xlsx (main Excel workbook)
3. Cleaned the data to isolate the values needed: specifically, only 2012 values
4. Salary values were for each individual hire. In order to find the average values for the agency as a whole, used AVERAGEIF functions to isolate specific data
5. Residency values were changed from numerical count to percentages, compiled into three categories: Baltimore City, Baltimore County, and Outside of Baltimore
6. Newly edited values were combined on the "combined_data" tab
7. Found the MEAN and STDEV for all columns, used the STANDARDIZE function to find the z-values for each factor
8. In the rows above the dataset, chose four random cluster points, used VLOOKUP to determine which agency correlated and related z-values
9. Used SUMXMY2 function to determine distance of each agency from the random cluster points
10. Used MIN function to find which cluster point each agency was closest to
11. Used MATCH function to match the provided minimum value with the anchor number of the cluster point it was closest to
12. Used VLOOKUP to correlate the MATCH value with the name of the agency it correlated to
13. Used SUM function to find the sum of the minimum distance column
14. Used Solver tool to minimize the sum-value, constraints were (<=49, >=1, int)
15. Important values from newly rendered cluster analysis were copied and pasted on the "important_values" tab
