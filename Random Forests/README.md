# Problems 
- A cloth manufacturing company is interested to know about the segment or attributes causes high sale. 
Approach - A Random Forest can be built with target variable Sales (we will first convert it in categorical variable) & all other variable will be independent in the analysis.  
- Use Random Forest to prepare a model on fraud data 
treating those who have taxable_income <= 30000 as "Risky" and others are "Good"

## Company Data
- EDA & Data Cleaning
- Spliting
- Model Building(RandomForestRegeressor)
- Hyperparameter tuning
```
Best Score: 0.6175260655803496
Best Parameters: {'criterion': 'squared_error', 'n_estimators': 48}
```
- Visualizing Feature importance


![image](https://user-images.githubusercontent.com/110924299/227698207-62a6b784-d6ab-404e-bf16-3d364ab045bd.png)
- Metrics(Mean Absolute Error)

## Fraud Data
- EDA & Data Cleaning
- Spliting
- Model Building(RandomForestClassifier)
- Hyperparameter tuning
```
Best Score: 0.7645833333333333
Best Parameters: {'criterion': 'log_loss', 'n_estimators': 6}
```
- Visualizing Feature importance

![image](https://user-images.githubusercontent.com/110924299/227698299-ffb28162-6633-422d-ae15-362b2d55d238.png)

- Classifiaction Report
