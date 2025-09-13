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



# Seaborn-Learnings  

1. Matplotlib → Low-level, powerful, very customizable, but verbose and plain by default.
Seaborn → High-level, built on Matplotlib, makes plots cleaner, easier, and adds built-in support for statistical visualizations.
Key difference: Matplotlib gives control, Seaborn gives convenience + good defaults.
They are complementary: Seaborn uses Matplotlib under the hood.

2. Axes-level = one plot, you control details.
Figure-level = whole figure with possibly many subplots, Seaborn controls layout.

3. When we plot data, we usually map variables to the x-axis and y-axis.But real-world data often has more than two variables. To represent them in the same plot, Seaborn provides aesthetic mappings like hue, style, and size.These add extra dimensions of information without needing extra axes.
hue maps a categorical or numerical variable to color.
style maps a categorical variable to marker shapes (like circles, squares, triangles).
size maps a numerical or categorical variable to marker size.

4. If the legend appears inside the axes (top-right corner by default) → Axes-level function.If the legend appears outside the axes, usually on the right side → Figure-level function.

5. A Facet plot in Seaborn is created using figure-level functions (like relplot, catplot, displot) and allows splitting data into multiple subplots. The row and col parameters let you arrange plots across rows and columns based on categorical variables. This functionality is only available in figure-level functions, not axes-level ones.

6. rugplot() is an axes-level function in Seaborn.It draws small vertical (or horizontal) ticks along the axis to represent individual data points.Each tick = one observation → so it shows the distribution of raw data in a very compact form.It is often combined with histograms or KDE plots to give context about actual data points.

7. point of confusion:
Histplot → counts or density of raw values (distribution).
KDEplot → smooth probability distribution.
Barplot → aggregated statistic (mean by default, can be changed).

8. A heatmap visualizes 2D data using colors instead of numbers, making it easy to detect patterns, high/low values, and relationships (like correlations).  

9. cluster map is similar to heatmap but internally performs clustering on data dendograms, A dendrogram is a diagram that shows the hierarchical merging of data points into clusters, with branch height representing the distance (similarity) between them. It’s widely used in hierarchical clustering to understand data structure.

10. A boxplot is a standardized way of displaying the distribution of data based on a five number summary (“minimum”, first quartile [Q1], median, third quartile [Q3] and “maximum”). It can tell you about your outliers and what their values are. Boxplots can also tell you if your data is symmetrical, how tightly your data is grouped and if and how your data is skewed.

11. Regression plots:
Use regplot for simple regression on one plot.
Use lmplot when you want regression + faceting across groups.
Use residplot to evaluate how well your regression fits by inspecting residuals.

12. The Seaborn pairplot() is a powerful figure-level function used for exploratory data analysis (EDA). It automatically creates a grid of plots that show the pairwise relationships between multiple numerical variables in a dataset. On the diagonal, it usually shows univariate distributions (like histograms or KDE plots), while the off-diagonal shows scatter plots between every pair of variables.

13. The Seaborn jointplot() is a figure-level function that combines a bivariate plot (like scatter, hex, or regression) with the univariate distributions of each variable on the top and right axes. 



