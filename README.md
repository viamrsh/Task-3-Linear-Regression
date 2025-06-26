# Task-3-Linear-Regression
1.Import and preprocess the dataset.

2.Split data into train-test sets.

3.Fit a Linear Regression model using sklearn.linear_model.

4.Evaluate model using MAE, MSE, R².

5.Plot regression line and interpret coefficients.


---
 # Objective: 
Implement and understand simple & multiple linear regression.

---
 # Tools: 
 
Scikit-learn, Pandas, Matplotlib


---
# code explanation 

 1.Importing essential Python libraries:

Pandas and NumPy: For handling and manipulating data.

Matplotlib and Seaborn: For creating graphs and visualizations.

Scikit-learn: For performing machine learning operations like regression, data splitting, and evaluation metrics.



---

2. Load Dataset

load the housing data (CSV file) into a table-like structure (DataFrame) for easy manipulation and analysis.


---

3. Explore the Data


Display the first few records to understand structure.

Summarize the data (mean, std, min, max).

Check for missing values that might affect the model.



---

4. Convert Categorical Columns

Any column with text (e.g., location) is converted into numeric format using one-hot encoding. This is important because machine learning models can’t understand text directly.


---

 5. Define Input (Features) and Output (Target)

Select all the independent variables (e.g., area, bedrooms, bathrooms) as features.

Select the dependent variable (house price) as the target.



---

6. Split Data into Training and Testing Sets

divide the dataset into two parts:

Training set (80%): Used to train the model.

Testing set (20%): Used to test how well the model performs on unseen data.



---

7. Train the Linear Regression Model

A linear regression model is created and trained using the training data. The model learns the best-fitting straight-line relationship between the input features and the target.


---

8. Make Predictions

The model is then used to predict house prices based on the test input data.


---

9. Evaluate Model Accuracy
 use evaluation metrics to check how well the model did:

MAE (Mean Absolute Error): Average absolute difference between actual and predicted prices.

MSE (Mean Squared Error): Average of squared errors.

RMSE: Square root of MSE, gives error in original units.

R² Score: How much variance in price is explained by the features (1 means perfect).



---

10. Interpret Model Coefficients

inspect how each feature affects the predicted price.

The coefficient tells how much the price changes per unit increase in that feature.

The intercept is the base value when all features are 0.



---

11. Visualize Results

Depending on number of features:

If one feature: Plot a regression line (predicted vs actual).

If multiple features:

Plot Actual vs Predicted prices: Helps see how well the model is doing.

Plot Residuals (errors): Helps check if errors are normally distributed (good sign).

---
12. Correlation Heatmap

You create a heatmap to visualize how strongly each feature is related to the others and to the price. This helps understand which features are most influential.

