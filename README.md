# Movie_Reviews_Classification

Three differnt machine learning algorithms were implemented from scratch ; ID3 , Random Forest and Logistic Regression 
in order to predict whether a movie review is positive or negative. The data used for the classification were from tensorflow library and more
specifically tf.keras.datasets.imdb. The original data were split to 25000 training and 25000 test data. Accuracy, precision, recall and F1 are calculated 
when ID3, Random Forest and Logistic Regression are called from the main, while at the same function plots for each of the aforementioned meters are displayed.

Accuracy scores for each algorithm are listed below with number of words being the number of words chosen for the creation of a vocabulary from
training data that refer to the most common used words in the imdb movie reviews, skip words being the number of words that should not be included at
the vocabulary, i.e articles and very common words which are not related with the user's opinion about a movie and max depth being the length of the decision 
tree that can be calculated by the algorithm.

ID3 :

| Accuracy | Number of Words | Skip Words | Max Depth
| -------- | --------------- | ---------- | -------- |
|0.642     |     100         |        10  |        10|
| 0.71096| 500| 100 |15|
|0.72048| 1000| 200| 20|
|0.67928| 4000| 400| 20|


Logistic Regression : an attempt to find the best λ , with a number of 1000 Iterations, 1000 words, 100 skipped words 100 and different λ
(learning rate) so as to increase the accuracy score resulted to a λ = 0.2, where accuracy stood at 0.843.

Random Forest:

| Accuracy | Number of Words | Skip Words | Max Depth|Number of trees|
| -------- | --------------- | ---------- | -------- |---------------|
|0.62328| 100| 10| 10| 2
|0.71972| 500| 100| 15|3
|0.72892| 1000| 200| 20|4
|0.73252| 1000| 200| 20|5




