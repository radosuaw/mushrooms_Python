# mushrooms
the mushroom dataset analysis
The dataset I worked on is the dataset available at the link
https://www.kaggle.com/uciml/mushroom-classification
It includes a set of 8124 samples of mushrooms in the Agaricus and Lepiota genera
of mushrooms from Agaricaceae family. Each sample has 23 nominal features
involving some characteristics of caps, veils, gills and stalks of the particular
mushrooms, their odor and signs of bruises. Each feature is a string (a letter to be
precise) meaning distinct category (full description is available at the link - as it’s
rather long I decided to omit it in the project description).
The purpose of the project is going to be prediction whether the sample belongs to
one class or another, in other words, classifying the data into one out of two
categories, namely predicting the membership to the class ‘e’ for edible mushroom or
‘p’ for poisonous one. To achieve that I plan to use all of the features that will be
encoded or not (depending on the used model; if yes - using One Hot Encoder for
features with more than two values and Dummy Variables for the binary ones) with
possibility to omit some of the less important ones (to be determined; using Random
Forests or binary encoding , depending on the performance of the models on full set
of features).
To achieve my goal, I’m going to try using models (from sklearn) such as Decision
Tree, Random Forest, K Nearest Neighbours, Support Vector Machine and
Logistic Regression . However, firstly I will perform some exploratory data
analysis using seaborn, matplotlib and numpy libraries. Having already explored
some data I can say that I will have to deal with some missing values as well. For
that purpose, I plan on imputing the missing values using K Nearest Neighbours or
maybe just drop the samples with missing values (depending on the number of such
samples). To tune the hyperparameters of the models (if needed) I will use Grid
Search. When it comes to evaluating the performance of the models, I will probably
try to validate them splitting the dataset into train and test set or perhaps use K-fold
Validation method to have a better insight into my models’ performances. To test the
accuracy I will use accuracy_score from sklearn and confusion_matrix.
