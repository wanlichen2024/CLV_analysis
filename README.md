I built a Customer Lifetime Value classification model using a public e-commerce dataset.
The goal was to segment customers by value so the marketing team could tailor personalized engagement strategies.
My task was to develop an accurate and interpretable classification model to predict whether a customer is high, medium, or low value.
I started by extracting and merging relevant variables from three relational tables.
After cleaning the data, I calculated RFM features and used them as inputs for K-Means clustering.
To determine the optimal number of clusters, I applied the Elbow method and Silhouette analysis, and found 3 clusters worked best—representing high, mid, and low value segments.
I then set the cluster labels as the target variable and trained two models: XGBoost classification and Random Forest.
Since the accuracy was very high (close to 99–100%), I applied cross-validation to check for overfitting.
The models remained stable, and I used SHAP to explain the feature importance of the Random Forest model.
 The final model accurately predicts CLV segments and can be used to support personalized marketing strategies—helping the business focus resources on high-value customers while nurturing others.
