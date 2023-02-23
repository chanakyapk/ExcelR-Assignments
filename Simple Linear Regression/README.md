
# Simple Linear Regression

- Delivery_time -> Predict delivery time using sorting time
- Salary_hike -> Build a prediction model for Salary_hike




### Simple Linear Regression on Delivery Data
#### Predict delivery time using sorting time
Step 1 (Understanding Data):
    
delivery_time.info()

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 21 entries, 0 to 20
    Data columns (total 2 columns):
    #   Column         Non-Null Count  Dtype  
    ---  ------         --------------  -----  
    0   Delivery Time  21 non-null     float64
    1   Sorting Time   21 non-null     int64  
    dtypes: float64(1), int64(1)
    memory usage: 464.0 bytes

delivery_time.corr()

            Delivery Time	Sorting Time
    Delivery Time	1.000000	0.825997
    Sorting Time	0.825997	1.000000

Step 2: (Visualing)
    
    ![image](https://user-images.githubusercontent.com/110924299/220840837-8cabde37-2b38-41d6-b661-777c7c9df87d.png)
    ![image](https://user-images.githubusercontent.com/110924299/220840914-38a641f2-d2a1-4857-a968-f286eeb8ee05.png)
    ![image](https://user-images.githubusercontent.com/110924299/220840976-2352b6ba-137d-49ba-885a-336a350aea09.png)
    ![image](https://user-images.githubusercontent.com/110924299/220841107-e4893ab5-cccc-4cee-8505-900a65481c64.png)


Step 3: (Modeling and Evaluating with R-Squared error)

    - Building Simple Linear Regression model
    - We get R-squared value 0.68 
    - With Normal(Unimputed) model we get very poor R-squared value

Step 4: (Applying imputations)

    - We applied 3 differnet imputations
    - First, Log on Independent Features
    - Second, Log on both Features
    - Third, Squareroot on both Features

#### Log on both Independentand and dependent Features gave best r-squared value of 0.77

### Simple Linear Regression on Salary Data
#### Build a prediction model for Salary_hike

Step 1 (Understanding Data):
    
Salary.info()

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 30 entries, 0 to 29
    Data columns (total 2 columns):
    #   Column           Non-Null Count  Dtype  
    ---  ------           --------------  -----  
    0   YearsExperience  30 non-null     float64
    1   Salary           30 non-null     float64
    dtypes: float64(2)
    memory usage: 608.0 bytes
Step 2: (Visualing)
    
    ![image](https://user-images.githubusercontent.com/110924299/220841291-ddba7a16-677f-4310-89d9-29b502a64197.png)
    ![image](https://user-images.githubusercontent.com/110924299/220841241-454cf6a4-83c2-49c0-81db-1887028b62eb.png)

    
Step 3: (Modeling and Evaluating with R-Squared error)

    - Building Simple Linear Regression model
    - We get R-squared value 0.956
    - With Normal(Unimputed) model we got good R-squared value

Step 4: (Applying imputations)

    - We applied 4 differnet imputations
    - First, Log on Independent Features
    - Second, Log on dependent Features
    - Third, adding squared value in independent Features

#### Unimputed model gave best r-squared value of 0.95
