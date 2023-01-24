A spam detector built using Python.

Libraries used :
1) NumPy
2) Pandas
3) MatPlotLib
4) nltk
5) seaborn
6) string
7) wordcloud
8) collections
9) sklearn

The first step was to analyse the data. 

![image](https://user-images.githubusercontent.com/84259885/214371108-7c8f207d-f4af-479f-941f-b2a9d62925c3.png)
The above figure shows the percentage of data that is spam.

Next step was to calculate the no. of words and characters in each message.
Next step was to analyze the no of characters/words to the category of the data.
![image](https://user-images.githubusercontent.com/84259885/214378495-b9f7298c-b904-4429-b17c-3fff6356d4aa.png)
![image](https://user-images.githubusercontent.com/84259885/214378548-faab5503-debb-4dcb-88bf-f200f2500e86.png)

The next step was to use Porter Stemmer on the messages.

The next step was to find out the most occuring words in spam and ham messages.
![image](https://user-images.githubusercontent.com/84259885/214379140-694416c1-64a1-482c-ae13-b68a8377953c.png)
![image](https://user-images.githubusercontent.com/84259885/214379185-92663747-14d6-4425-b3b1-e3eaf5dee13f.png)

The next step was to transform the data using tf.idf vectorizer

The last step was to apply the Multinomial Naive Bayes ML algorithm.
( It had the best performance among many other ML agorithms tested)

CONFUSION MATRIX
 [[896   0]
 [ 30 108]]


CLASSSIFICATION REPORT
               precision    recall  f1-score   support

           0       0.97      1.00      0.98       896
           1       1.00      0.78      0.88       138

    accuracy                           0.97      1034
   macro avg       0.98      0.89      0.93      1034
weighted avg       0.97      0.97      0.97      1034

The above is the result.
