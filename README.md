# Data-Visualization-Libraries

# Matplotlib-Library  

1. import matplotlib.pyplot as plt.

2. The choice of graph depends upon type of data whether it is categorical or numerical.   

3. Types of analysis- Univariate, Bivariate, Multivariate.

4. A 2D line plot is one of the most basic and widely used data visualization techniques. It is primarily used to show the relationship between two variables, usually numerical, with one variable plotted along the x-axis (independent variable) and the other along the y-axis (dependent variable).  
Line plots are especially useful when we want to study patterns, trends, or changes in data over time.  

5. plt.title() is used to set the main title of the graph, which usually describes what the plot represents. It appears at the top of the figure and gives a quick idea about the data being visualized. The plt.xlabel() function is used to label the x-axis, indicating what type of data is plotted along the horizontal axis, while plt.ylabel() labels the y-axis, specifying the meaning of values plotted on the vertical axis. These labels make it easier to interpret the relationship between the two variables being plotted. The plt.legend() function is used when multiple plots or lines are drawn on the same figure. It displays a small box (legend) that identifies each line or dataset using the labels provided in the code.  

6. The function plt.xlim() allows the user to define the minimum and maximum values of the x-axis, while plt.ylim() sets the range of the y-axis. These functions help in zooming into specific areas of a graph, highlighting important trends, or ensuring that multiple plots are compared on the same scale.  

7. A scatterplot is a type of graph used to display the relationship between two numerical variables. Each data point is represented as a dot on the plot. Scatterplots are mainly used to observe how one variable changes with respect to another and to identify possible patterns, correlations, or clusters within the data. Scatterplots are particularly useful for showing whether there is a positive correlation (both variables increase together), a negative correlation (one variable increases while the other decreases), or no correlation (no clear pattern between the variables). They can also reveal outliers, which are points that deviate significantly from the overall trend.  

8. A bar chart is a graphical representation used to display and compare categorical data. In a bar chart, each category is represented by a rectangular bar, and the height (or length, in case of a horizontal bar chart) of the bar corresponds to the value or frequency of that category.

9. A histogram is a type of plot that shows the distribution of a numerical variable by dividing the range of values into intervals (called bins) and then counting how many data points fall into each bin. Each bin is represented as a bar, and the height of the bar corresponds to the frequency (count) of values in that interval.

10. A pie chart is a circular statistical graphic used to represent categorical data as slices of a circle. Each slice corresponds to a category, and the size of the slice is proportional to the value or percentage that the category contributes to the whole. The entire pie represents 100% of the data.

11. In Matplotlib, subplots let you create multiple plots within the same figure. Instead of opening a new figure for each plot, you divide one figure into a grid (rows × columns) and place plots inside it.  
