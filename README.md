# Linear_Regression_Model

Initially, this project aims to predict house prices using *linear regression* techniques based on features from the King County housing dataset. The dataset contains housing sale prices along with 21,613 rows of information such as the number of bedrooms, bathrooms, living area size, floors, and other physical attributes of the houses. The goal is to understand the relationship between these features and the house price, and to build a predictive model that generalizes well on unseen data.

The workflow begins with loading and exploring the dataset. Irrelevant features such as the ID, date, latitude, longitude, and zipcode are removed to avoid noise and geolocation bias in the model. The remaining numerical features are scaled using standardization, which is essential for linear models—especially when applying regularization.

Three different regression models are developed: standard Linear Regression, Ridge Regression (L2 regularization). The Linear Regression model serves as a baseline. Ridge is used to reduce overfitting while retaining all features. Cross-validation is applied during the tuning of the regularization parameter (alpha) for Ridge to find the best model.

The models are evaluated using the R² score and Root Mean Squared Error (RMSE) on a held-out test set. In addition, several plots such as Actual versus Predicted prices and residual distributions are created to visualize model performance. Furthermore, the results show that regularization techniques improve model generalization. Ridge regression tends to provide more stable predictions, especially when many features are relevant.

Eventually, this project demonstrates the importance of data preprocessing, model tuning, and visual diagnostics in regression analysis. It also highlights how linear models can be enhanced with regularization to produce reliable and interpretable predictions in real-world applications such as housing price estimation.
