Classifying a given text comment as toxic or non-toxic using natural language processing

First of all I got the data from an expired kaggle competition.
The data consisited of more than hunderd thousand twitter comments each already classified as toxic or non-toxic.

I cleaned the data by removing puctuations, line breaks, stop words etc. and then divided it into training and testing set.
Using scikit-learn with natural language processing I trained my training set and used that to predict results for testing set.
I created seven classifiers: KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, LogisticRegression, SGDClassifier, 
MultinomialNB and SVC.
All of these were combined in voting classifier which gave an accuracy of 94.05 on my test set.
