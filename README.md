# Mushroom-Classificaiton-Take-1

Using the UCI mushroom dataset, find the best model to classify mushrooms as edible or poisionous using supervised learning techniques with the 22 features in the dataset.  All features are nominal (categorical) with varying numbers of categories per feature.  
Begin by visualizing counts of the number of poisonous and edible mushrooms that have each category for each of the 22 features.  Then, several models were constructed.  The first two a simple decision models that classify mushroom observations as edible for certain categories of odor or spore print color.  
Next, the data set was encoded using the sklearn LabelEncoder.   Note that the LabelEncoder imposes an ordinal topological structure onto the data, and can thus introduce more bias into the subsequent models.  A better approach would be to use binary dummy variables, but that is performed in Mushroom Classification Take 2. 
Once data is encoded, build K-Nearest Neighbors and Logisitic Regression models.  
Model selection is performed by choosing the model that has the highest accuracy on the test data set, and the K-Nearest Neighbors model with K=3 performs the best with 99.93% training accuracy, 99.74% testing accuracy, and 99.59% validation accuracy.
