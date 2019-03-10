## Amazon fine food reviews

This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

Source: https://www.kaggle.com/snap/amazon-fine-food-reviews


## What have I done with it?

I explored this dataset through the eyes of various machine learning algorithms, Most of these algorithms are from https://scikit-learn.org/stable/#. Since one of the important feature of this dataset is text reviews, We have the four widely used vectorizations such as CountVectorizer, TfidfVectorizer, avgw2v and tfidfw2v induvidually to process the text data. In text data, Every word is a feature and hence I've managed to find the so called important features or top features of the dataset for both count and tfidf vectorizer. We have used cross validation techniques such as simple CV, K-fold CV, gridsearch, randomsearch etc to find the right hyperparameters. Thanks for patiently reading through this. Hope you find it helpful!
