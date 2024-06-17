# lab9-356
## Part 1: Your final project- Ask a question
In a new notebook, describe a part of your project that you are not sure about. Ask the question, and display the related data, what tools you are using, and what you are trying to do and how far you have gotten. If your cells are loading slowly, you should save your processed data and load it in (should all be available in your github). Example of how to do this is in Week 9 slides and also I posted the code in slack.
## Part 2: Trees
The dataset mpg.csv contains information on miles per gallon (mpg) and engine size for cars sold from 1970 through 1982. The dataset has the features mpg, cylinders, displacement, horsepower, weight, acceleration, model_year, origin, and name.

1. Load the mpg.csv dataset
2. Create a dataframe, X, using weight and model_year as features
3. Create a dataframe, y, using mpg
4. Initialize a regression tree with random_state = 100 that has depth 3 and a minimum number of samples in each leaf of 5
5. Fit the regression tree on X
6. Visualize your tree (graphically, not just text)

If acceleration is used instead of weight, the output should be:
```
max_depth = 3, 100
|--- model_year <= 79.50
|   |--- acceleration <= 13.95
|   |   |--- model_year <= 78.50
|   |   |   |--- value: [15.78]
|   |   |--- model_year >  78.50
|   |   |   |--- value: [25.13]
|   |--- acceleration >  13.95
|   |   |--- model_year <= 76.50
|   |   |   |--- value: [21.94]
|   |   |--- model_year >  76.50
|   |   |   |--- value: [25.28]
|--- model_year >  79.50
|   |--- acceleration <= 20.60
|   |   |--- model_year <= 80.50
|   |   |   |--- value: [33.06]
|   |   |--- model_year >  80.50
|   |   |   |--- value: [30.84]
|   |--- acceleration >  20.60
|   |   |--- value: [38.32]
```
7. Use any tool we have covered (or not) to come up with the best model, and report, and run it
8. Analysis. What can you conclude from your lab work?
