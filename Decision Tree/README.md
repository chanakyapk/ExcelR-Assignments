# Problems
- A cloth manufacturing company is interested to know about the segment or attributes causes high sale. 
Approach - A decision tree can be built with target variable Sale (we will first convert it in categorical variable) & all other variable will be independent in the analysis.  
- Use decision trees to prepare a model on fraud data 
treating those who have taxable_income <= 30000 as "Risky" and others are "Good"

## Company Data
- EDA & Data Cleaning
- Model Building (DecisionTreeRegressor)
- Hyper Parameter Tuning
```
Best Score: 0.42801966032638517
Best Parameters: {'criterion': 'friedman_mse', 'max_depth': 6}
```

- Visualizing

![image](https://user-images.githubusercontent.com/110924299/227697831-7fd8cd3b-8b61-4f64-b4b2-8d3dd9c48113.png)


## Fraud Data
- EDA & Data Cleaning
- Spliting
- Model Building (DecisionTreeRegressor)
- Hyper Parameter Tuning
```
Best Score: 0.7933333333333332
Best Parameters: {'criterion': 'gini', 'max_depth': 1}

```

- Visualizing


![image](https://user-images.githubusercontent.com/110924299/227697916-8505264c-2f50-47b7-ab90-7f4dca0ea416.png)


- Classification Report
