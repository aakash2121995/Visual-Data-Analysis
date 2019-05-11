## Multidimensional Data Filtering and Visualization

1. Read the data given in winequality-red.csv, available from the lecture webpage, and print the
first few rows. 
2. A numerical rating of sensory wine quality is given in the column“quality”. Display the distribution
of these scores with a histogram. What is the range of this score in the data? (1P)
3. Derive a coarser classification of quality into “low”, “medium”, and “high”, by grouping together
the two lowest, the intermediate, and the two highest quality scores that occur in the dataset,
respectively. Replace the original “quality” column with a new column “quality bin” that contains
these labels. 
4. We would like to investigate differences between high and low quality wines. Therefore, create a
filtered data frame in which the medium-quality wines are omitted. (1P)
5. Visualize all numerical attributes in a scatterplot matrix. Color the two quality levels differently.
(1P) Hint: Using seaborn, you can create this plot with a single (and simple) line of code.
6. Based on the visualization, name five attributes that appear to best distinguish between high and
low quality.
7. Now, use an automated feature selection technique to identify five attributes that distinguish
between high and low quality. More specifically, please use the F score from a one-way analysis
of variance (ANOVA) to rank the attributes, as implemented in scikit learn’s f_classif. What
are the five best attributes according to this measure? Are they the same as those you identified
visually? Create a filtered data frame that only contains the top five attributes, plus the “quality
bin”. 
8. Create a matrix similar to the one in Fig. 1: It should compare the two quality bins with respect
to the five top-ranking attributes, using density estimates (on the diagonal), scatterplots (in the
upper triangular part), and plots of pairwise linear regression models 
9. Based on the visualization, which attributes appear to be strongly correlated regardless of quality?
For which attributes does the amount of correlation appear to depend on the quality? Does any
of the attributes appear to have a multimodal distribution? Point out one or multiple data points
that appear to be outliers. 
9. Compute the distance consistency of all scatter plots. Which pair of variables leads to the highest
distance consistency? 