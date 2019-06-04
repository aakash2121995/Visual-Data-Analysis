## Multidimensional Data Filtering and Visualization

a) Read the breast-cancer-wisconsin.xlsx file. Note that there are some instances with missing
data, which have to be imputed before we can run PCA. Pandas offers convenient functions for
this. Apply an imputation method that makes sense for this dataset, and briefly explain your
decision. 

b) Create a plot that, for any number n, shows what fraction of the overall variance in the data is
contained in the first n principal components. Make sure that you only include the nine relevant
numerical attributes in the PCA, not the sample codes or class IDs. How many components do
we need to cover ≥ 90% of the variance?

c) Each sample is now characterized by a point in PCA space. Create a scatter plot matrix that
shows the first five principal components. Each diagonal cell should contain two overlaid density
plots, one for the benign and one for the malignant class. Use different colors to distinguish
between the classes, and add a legend that clearly states which samples are benign or malignant.


d) Which PCA mode shows the strongest difference between the benign and the malignant samples?
Name the original variables that have the highest and lowest weights in its definition, respectively.

e) Scatterplot matrices often reveal outliers in the data. Visually identify at least one sample that
is far away from the others, remove it from the dataset, and re-generate the scatterplot matrix
without it.


f) In the breast cancer dataset, all variables x i have a similar range, x i ∈ [1, 10]. If the variables of
a dataset have very different ranges, for example one variable x 1 ∈ [1000, 2000] and another onex 2 ∈ [1, 5], how would this affect the PCA? Could it make sense to pre-process the data in such
cases? Why and how?

g) Explain why, on this dataset, we cannot use Linear Discriminant Analysis (LDA) to create an
alternative 5D embedding in which the classes are more clearly separated. Use the LDA imple-
mentation in scikit-learn to perform a 1D LDA embedding and plot it (in a scatterplot) against
the first principal component. Do they show a clear correlation? Is this true in general, or specific
to the dataset?