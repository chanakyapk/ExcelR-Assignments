# Problem statement
Build a recommender system by using cosine simillarties score.

## Steps
- EDA and Pre-processing
- Visualizing

![image](https://user-images.githubusercontent.com/110924299/224015292-79cbac93-9ebf-42fd-b978-d546ca5fe1fd.png)


- Making Pivot Table
- Model Building
```
Pairwise distances
Filling Diagonal
```
- Function creation for recommendation
```
def recommend_new(custID):
    simID = list(user_sim_df.sort_values(custID,ascending = False).head(5).index)
    simID_title = [books[books['Id'] == each].Title for each in simID]
    simID_title = np.concatenate(simID_title)
    custID_title = books[books['Id'] == custID].Title
    return set(simID_title) - set(custID_title)
```
