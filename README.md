## Flight Fare Regression

### **Objective**
Predict flight fares based on flight details using machine learning regression models.

### **Dataset Overview**
- Dataset includes features such as:
  - `Date_of_Journey`: Date of travel.
  - `Dep_Time` and `Arrival_Time`: Flight departure and arrival times.
  - `Total_Stops`: Number of stops during the journey.
  - `Price`: Target variable indicating flight fare.

### **Workflow**
1. **Data Cleaning**:
   - Handled missing values by removing affected rows.
   - Removed unnecessary columns (`Route`, `Additional_Info`) for simplicity.

2. **Feature Engineering**:
   - Extracted new features:
     - `j_month`, `j_date`: Month and day of travel from `Date_of_Journey`.
     - `d_total_min`, `a_total_min`: Total minutes for departure and arrival times.
   - Processed `Duration` to split into hours and minutes.
   - Encoded `Total_Stops` using ordinal encoding.
   - Created dummy variables for `Source` and `Destination`.

3. **Model Development**:
   - Models evaluated:
     - Linear Regression
     - Random Forest Regressor
     - Support Vector Regressor (SVR)
     - K-Nearest Neighbors Regressor (KNN)
     - Decision Tree Regressor
     - Gradient Boosting Regressor
   - Hyperparameter tuning for Random Forest using `RandomizedSearchCV`.
   - Cross-validation used to ensure robust performance.

4. **Results**:
   - Random Forest Regressor provided the best performance after tuning.
   - Feature importance identified top predictors of flight prices.

5. **Visualization**:
   - Bar plots showing feature importance for fare prediction.
   - Comparison of model performance metrics.


### **Key Highlights**
#### Financial Fraud Detection
- Comprehensive preprocessing to handle outliers and irrelevant features.
- Visual analysis revealed key trends in fraudulent transactions.
- Logistic Regression demonstrated high accuracy.

#### Flight Fare Regression
- Extensive feature engineering, including date and time manipulations.
- Random Forest Regressor emerged as the most effective model.
- Feature importance analysis provided actionable insights.


## Future Enhancements
2. **Flight Fare Regression**:
   - Explore additional regression models, such as neural networks.
   - Incorporate external data, e.g., weather or holiday information, to improve predictions.
