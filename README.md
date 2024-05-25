# KNN_VS_SVM_Stock_Price_Prediction
**Purpose**

The purpose of this project is to compare the performance of K-Nearest Neighbors (KNN) and Support Vector Machine (SVM) models in predicting stock prices. Specifically, this analysis focuses on predicting the closing prices of Apple Inc. (AAPL) using historical stock price data from 2015 to 2020.


K-Nearest Neighbors (KNN) is a simple, non-parametric method that predicts based on the average value of the nearest neighbors, useful for capturing local trends in volatile markets. Support Vector Machine (SVM), a versatile model, performs both linear and non-linear regression, finding the best-fit hyperplane and handling high-dimensional data effectively to avoid overfitting. Comparing KNN and SVM helps evaluate predictive performance, understand model strengths and weaknesses, and ensure the best fit for financial data analysis.

**Methodology**

*Data Preprocessing*

Loaded historical stock price data from 2015 to 2020.
Selected relevant features (open, high, low, volume, adjClose, adjHigh, adjLow, adjOpen, adjVolume, divCash, splitFactor) and the target variable (close).
Split the dataset into training and testing sets with an 80-20 split.
Scaled the features using StandardScaler to ensure the models perform well.

*Model Training and Evaluation*

Trained a K-Nearest Neighbors (KNN) regression model with 5 neighbors.
Trained a Support Vector Machine (SVM) regression model with a linear kernel.
Used 5-fold cross-validation to evaluate the models' performance during training.
Predicted the closing prices using the trained models.
Calculated and compared the Mean Squared Error (MSE) for both models.

*Visualization*

Plotted the actual vs predicted prices for both models.
Created histograms to show the distribution of prediction errors for each model.
Plotted scatter plots comparing actual prices with predicted prices.
Generated learning curves for both models to illustrate their performance as the training size increases.

**Findings**
The results of the models' performance are as follows:

*Mean Squared Error (MSE)*

KNN: 9.70
SVM: 1.43

*Cross-Validation MSE*

KNN: 32.23
SVM: 1.64

These results indicate that the SVM model significantly outperformed the KNN model in predicting the closing prices of Apple Inc. The lower MSE values for SVM (1.43 for test set and 1.64 for cross-validation) suggest that it provides more accurate predictions and generalizes better to unseen data compared to KNN (MSE of 9.70 for test set and 32.23 for cross-validation). This implies that SVM is more effective in capturing the underlying patterns and trends in the stock price data, making it a more reliable choice for financial forecasting. These findings are crucial for investors and financial analysts as accurate stock price predictions can inform better investment decisions and risk management strategies.
Visualization

Actual vs Predicted Prices:
Shows a visual comparison between the actual closing prices and the predicted prices by both KNN and SVM models.

![github](https://github.com/pavelkimldn/KNN_VS_SVM_Stock_Price_Prediction/blob/main/Picture%201.png)

Distribution of Prediction Errors:
Histograms displaying the frequency of prediction errors for each model, providing insight into the distribution and magnitude of the errors.
![github](https://github.com/pavelkimldn/KNN_VS_SVM_Stock_Price_Prediction/blob/main/Picture%202.png)

Actual vs Predicted Scatter Plot:
Scatter plots illustrating the relationship between actual prices and predicted prices, highlighting the models' prediction accuracy.
![github](https://github.com/pavelkimldn/KNN_VS_SVM_Stock_Price_Prediction/blob/main/Picture%203.png)

Learning Curves:
Demonstrates the models' performance as the training set size increases, providing insights into the models' learning behavior and potential overfitting/underfitting.
This comprehensive analysis showcases the application of machine learning techniques to financial data, providing valuable insights into stock price prediction and model performance comparison.

![github](https://github.com/pavelkimldn/KNN_VS_SVM_Stock_Price_Prediction/blob/main/image%204.png)
![github](https://github.com/pavelkimldn/KNN_VS_SVM_Stock_Price_Prediction/blob/main/image%205.png)


