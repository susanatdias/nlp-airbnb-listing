# nlp-airbnb-listing

## Predicting Airbnb Unlisting

#### Project Objectives

The goal of this project is to use Natural Language Processing (NLP) models to predict whether a property listed on Airbnb will be unlisted in the next quarter1. For this, you will resort to real Airbnb property descriptions, Airbnb host descriptions, and comments from previous guests. In summary, with the NLP techniques you will learn during the Text Mining course, you must implement an NLP classification model able to predict, for each property, if it was unlisted (1) or is still listed (0).

The project should be developed using Python and libraries such as NLTK, Scikit Learn, Keras or PyTorch. Also, the project can be solved in various ways, which means there is no exact correct solution. And, of course, groups should not use code from each other!

#### Corpora

The data is divided in following sets:
- ``Train (train.xlsx)`` (12,496 lines): Contains the Airbnb and host descriptions (“description”
and “host_about” columns), as well as the information regarding the property listing status (“unlisted” column). A property is considered unlisted (1) if it got removed from the quarterly Airbnb list and it is considered listed (1) if it remains on that same list.

- ``Train Reviews`` (train_reviews.xlsx) (72,1402): This file has all the guests’ comments made to each Airbnb property. Note that there can be more than one comment per property, not all properties have comments, and comments can appear in many languages!

- ``Test (test.xlsx)`` (1,389 lines): The structure of this dataset is the same as the train set, except that it does not contain the “unlisted” column. The teaching team is keeping this information secret! You are expected to provide the predicted status (0 or 1) for each Airbnb in this set. Once the projects are delivered, we will compare your predictions with the actual (true) labels.

- ``Test Reviews (test_reviews.xlsx)`` (80,877): The structure of this dataset is the same as the train reviews set, but the comments correspond to the properties present on the test set.

Note that you are not required to use all the textual fields from the provided corpora as input for your model. For example, your best solution may just use the “description” column as input.

#### Solution Requirements and Evaluation Criteria

Your solution should present the following points:

1. ``Data Exploration`` : Here you should analyze the corpora and provide some conclusions and visual information (bar charts, word clouds, etc.) that contextualize the data.

2. ``Data Preprocessing`` : You must apply a method to split your training corpus into train/validation sets to evaluate the performance of your model (you can also resort to K- Fold cross validation, or other methods). Moreover, you must correctly implement and experiment at least four (4) of the data preprocessing techniques shown in class (stop words, regular expressions, lemmatization, stemming, etc.).

3. ``Feature Engineering`` : You must correctly implement and experiment with two (2) of the feature engineering techniques seen in class (TF-IDF, GloVe embeddings, etc.).

4. ``Classification Models`` : You must correctly implement and test three (3) of the classification algorithms seen in class (KNN, LR, MLP, LSTM, etc.).

5. ``Evaluation`` : You must evaluate your models resorting, at least, to Recall, Precision, Accuracy and F1-Score.

Moreover, the development of extra work (more techniques than the minimum required in the previous points and/or techniques not shown in class).
