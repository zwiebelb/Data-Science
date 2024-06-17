In this lab we used the beans dataset and were asked to use the beans feauters to predict which bean it is. I also wrote up an update of my final project.

# lab7-356 Kaggle Competition
1. As explained in class, we will do this Kaggle-based competition 'Kaggle style' with a clean, mean notebook.
2. You know the drill now: look at your two datasets (recall second is for competition submission only) read in your data
3. summary, value_counts, the basics
4. use Scikit learn's K-nearest-Neighbor (your Zybook this week covers the same Bean dataset ideas)
5. How will you choose K? Explain in your notebook your choice and why
6. Split the labeled dataset into training and test
7. For simplicity, you can do something like this: 
``` # Initialize model
beanKnnClassifier = KNeighborsClassifier(n_neighbors=5)
# Split data
X = beans[["MajorAxisLength", "MinorAxisLength"]]
y = beans[["Class"]]
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
```

8. Scale only on X_train (we will not do student-style we will do kaggle-style)
9. Fit model and predict on your test data
10. Scatter plot of actual and predictions
11. Compute mse and R2, explain your findings
12. Optional: try to improve your model's accuracy
13. Optional: try XGBoost and see if that nets you better results!
14. For your project: instead of verbally or a notebook, write up in an md file or pdf or text file an update on your timeline, what you have done, what you plan to try to accomplish in the next three weeks.
