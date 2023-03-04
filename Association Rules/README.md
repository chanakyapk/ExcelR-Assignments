# Association Rule 

Prepare rules for the all the data sets 
- Try different values of support and confidence. Observe the change in number of rules for different support,confidence values
- Change the minimum length in apriori algorithm
- Visulize the obtained rules using different plots 

## Books Data

- EDA
- Apriori Algorithm
```bash
with, min_support =0.1
```
- Getting Rules
```
with, metric="lift", min_threshold=0.7
```
- Visualizing

![image](https://user-images.githubusercontent.com/110924299/222904679-ab761b4f-ca4d-40b5-b618-5688b59829dd.png)

- Changing Parameters
```
with, metric="lift", min_threshold=2
```
- Checking Confidence > 0.5
##### Therefore, for `support>0`, `confidence>0.5`, `lift>2` we get 25 rules, with *ItalCook* and *CookBks* as most optimum rule

## Movies Data

- EDA
- Apriori Algorithm
```bash
with, min_support =0.1
```
- Getting Rules
```
with, metric="lift", min_threshold=0.7
```
- Visualizing

![image](https://user-images.githubusercontent.com/110924299/222904704-e2963047-38f4-4f81-a335-62ed33bf85f6.png)

- Changing Parameters
```
with, metric="lift", min_threshold=5
```
- Checking Confidence > 0.5
##### Therefore, we get the most optimum results for `support>0.1`, `confidence>0.5`, and `lift>5`
