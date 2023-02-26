# Insightful-Analysis-of-Pakistan-s-Economy-Using-World-Development-Indicators

## Objective:
The code reads in an Excel file containing World Development Indicators, filters the data for the years between 1998 and 2022, and creates visualizations to analyze GDP growth, exports, and imports in Pakistan.

## Explination:
The code first imports necessary libraries: pandas, matplotlib.pyplot, matplotlib.ticker, and numpy. Then, it reads in an Excel file "World_Development_Indicators.xlsx" and transposes the data, so that the countries are in rows and the indicators are in columns. After resetting the index and dropping the "index" column, the code applies a lambda function to convert the "Year" column to an integer by extracting the first four digits of the string. Missing values are handled by filling GDP with 0 and using forward filling method for exports, imports, and debt. Then, the filtered data is created using a boolean expression filtering the data between 1998 and 2022.

The first visualization shows the GDP growth in Pakistan between 1998 and 2022 using a line plot and a bar chart. The code creates two subplots with titles, labels, and tick marks for both the x and y axes. The first subplot shows a line plot with the growth rate of GDP over the years. The second subplot shows a bar chart with the same data. For both subplots, the code adds annotations to the plot with the corresponding GDP growth rate for each year. Finally, the subplots are displayed with plt.tight_layout() and plt.show().

The second visualization analyzes exports and imports in Pakistan between 1998 and 2022. The code defines custom colors for exports and imports and creates three subplots with titles, labels, and tick marks for both the x and y axes. The first subplot shows a bar chart with the value of exports over the years. The second subplot shows a bar chart with the value of imports over the years. The third subplot shows a line plot with both exports and imports over the years. For each subplot, the code adds annotations to the plot with the corresponding value for each year. The y-axis of each subplot is formatted with a function to divide the values by 1 billion. Finally, the subplots are displayed with plt.tight_layout() and plt.show().

## Conclusion:
The analysis above shows the GDP growth, exports, and imports trends in Pakistan from 1998 to 2022. The GDP growth rate has fluctuated over the years, with the highest growth rate observed in 2005, and the lowest in 2010. The Exports and imports have increased consistently over the years, with imports generally higher than exports. The analysis was conducted using two different types of plots - line plots and bar charts - to better understand the trends and variations in the data. Overall, the analysis suggests that Pakistan's economy has been growing steadily over the years, with a strong focus on exports and imports.
