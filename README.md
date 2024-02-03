frequency = c(0.6,0.3,0.4,0.4,0.2,0.6,0.3,0.4,0.9,0.2)
bloodpressure = c(103,87,32,42,59,109,78,205,135,176)
first = c(1,1,1,1,0,0,0,0,NA,1)
second = c(0,0,1,1,0,0,1,1,1,1)
final = c(0,1,0,1,0,1,0,1,1,1)
par(mfrow = c(1,3))
boxplot(frequency)
boxplot(bloodpressure)
boxplot(first, second, final)
par(mfrow = c(1,3))
hist(frequency)
hist(bloodpressure)
hist(c(first, second, final))

EXPLANATION

1.	Vectors Definition:
•	frequency: Contains numeric values representing some frequency data.
•	bloodpressure: Contains numeric values representing blood pressure readings.
•	first, second, final: These are vectors containing categorical variables, likely binary or ordinal explaining first second and final decision of doctors.
2.	Plotting Setup:
•	par(mfrow = c(1, 3)): Sets up the plotting layout to have 1 row and 3 columns. This means subsequent plots will be arranged in this format.
3.	Boxplots:
•	boxplot(frequency): Generates a boxplot of the frequency vector.
•	boxplot(bloodpressure): Generates a boxplot of the bloodpressure vector.
•	boxplot(first, second, final): Generates a boxplot comparing the distributions of the three categorical vectors first, second, and final. Since these are categorical variables, boxplots may not be the most informative representation, but this will display basic statistics (like median, quartiles, and outliers) for each category.
4.	hist(frequency): Creates a histogram of the Histograms:
•	frequency vector.
•	hist(bloodpressure): Creates a histogram of the bloodpressure vector.
•	hist(c(first, second, final)): Creates a histogram of the combined categorical variables first, second, and final. This  three vectors together before creating the histogram. However, this may not be the most meaningful representation for categorical variables, as histograms are typically used for continuous data.
