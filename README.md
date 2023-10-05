# R-DATA-ANALYSIS-PROJECT

This data analysis report focuses on analyzing a dataset related to healthcare costs. The key tasks and insights from this analysis can be summarized as follows.

The report begins by loading a CSV file into a dataframe named costDF. It then uses the summary function to provide descriptive statistics of the variables in the dataset, including counts, means, quartiles, and more. The dataframe contains 7,582 observations across 14 different variables.

Missing values are identified using the is.na function, and it is found that there are 158 missing values in the dataset. The report proceeds to impute missing values in the 'bmi' and 'hypertension' columns with their respective means.

The report generates tables for three categorical response variables: 'location,' 'yearly_physical,' and 'education_level.' These tables show the distribution of data within each category, providing insights into how different factors relate to these variables.

A new attribute named 'expensive' is created based on whether a person's cost is above the average cost of all patients in the dataset. This attribute is used for further analysis.

The report creates histograms for 'cost,' 'age,' and 'expensive' variables. These histograms visually represent the distribution of these variables, with additional analysis to show the mean on the graphs. The histograms provide insights into the distribution of healthcare costs and the age of patients.

The dataset is aggregated at the state level, calculating the average cost for each state. The analysis identifies that New York has the highest average cost per person.

The report attempts to identify patterns of attributes associated with being 'expensive' using Association Rules Mining. The attributes 'location' and 'smoker' are mentioned as having high confidence rules associated with being 'expensive,' suggesting potential correlations.

Supervised Machine Learning: The data is partitioned into a training set and a test set. Support Vector Machine (SVM) and Decision Trees (rpart) models are created to predict high-cost individuals. Model performance is evaluated using confusion matrices.

The report suggests that the SVM and Decision Tree models provide similar results, as expected, since both models use the same dataset and target variable.

The most important actionable insight is related to the impact of location on healthcare costs. It is recommended that efforts be made to ensure that healthcare costs are more related to patients' conditions and needs rather than their geographical location to maintain ethical and equitable pricing for patients.
