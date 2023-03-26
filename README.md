# Forecasting the Future: Exploring Patterns and Trends in Weather Data
This project explores a weather dataset containing 3,271 days of weather information with 22 variables on each day, including Date, Rainfall, Sunshine, Rain_Today, and many others. The main goal of the exploration was to determine the factors that affect rainfall and to use machine learning algorithms to predict the possibility of rain tomorrow.

## `About The Dataset`
The original source of the data is the Australian Government's Bureau of Meteorology, and the latest data can be gathered from http://www.bom.gov.au/climate/dwo/. The dataset used in this project has extra columns like 'Rain_Today' and our target is 'Rain_Tomorrow', which was gathered from the Rattle at https://bitbucket.org/kayontoga/rattle/src/master/data/weatherAUS.RData. This dataset contains observations of weather metrics for each day from 2008 to 2017. Column definitions were gathered from http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml.

## `Summary of Findings`
The findings suggest that there is a relationship between various weather variables and the occurrence of rain. Specifically, lower temperatures and higher humidity are associated with a higher probability of rain, while higher wind speeds and cloud coverage also increase the likelihood of rain. Wind direction and average temperature also play a role in determining the probability of rain.

Overall, the plots and charts illustrate that low temperature, high humidity, low sunshine hours, and high cloud coverage increase the likelihood of rain. Wind direction, on the other hand, is not a strong predictor of rain, but when combined with temperature, it can provide valuable information for determining the likelihood of rain. The correlations between the variables are generally low or negative, except for a strong correlation between cloud coverage and humidity, and a strong negative correlation between sunshine hours and cloud coverage.

The report provides the evaluation metrics for four machine learning algorithms (KNN, Decision Tree, Logistic Regression, and SVM) on the Weather dataset. Logistic Regression performs consistently well across all metrics, with the highest values for accuracy, Jaccard index, and F1 score, and the lowest log loss value. KNN performs well in accuracy, Jaccard index, and F1 score, but has a relatively high log loss value. SVM has similar accuracy and Jaccard index values to KNN, but has a much lower F1 score. Decision Tree performs poorly across all metrics, with the lowest values for accuracy, Jaccard index, and F1 score.

## `Evaluation Metrics`
`Accuracy Score:` The accuracy score measures the proportion of correctly classified instances over the total number of instances. Based on the table, Logistic Regression (LR) and KNN have the highest accuracy score, with a value of 0.841221 and 0.838168, respectively. The Decision Tree algorithm has the lowest accuracy score, with a value of 0.81374.

`Jaccard Index:` The Jaccard index measures the similarity between two sets of data. In this case, it measures the similarity between the predicted and actual labels. Based on the table, LR has the highest Jaccard Index value of 0.809174, followed by KNN with a value of 0.717188. The Decision Tree algorithm has the lowest Jaccard Index value of 0.691308.

`F1 Score:` The F1 Score is the harmonic mean of precision and recall, with equal weight given to both. Based on the table, LR has the highest F1 Score value of 0.833983, followed by KNN with a value of 0.825782. The Decision Tree algorithm has the lowest F1 Score value of 0.809162.

`Log Loss:` The performance of a classification model where the predicted output is a probability value between 0 and 1. Lower values indicate better performance. Based on the table, LR has the lowest log loss
