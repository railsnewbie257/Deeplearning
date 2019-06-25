https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html

<pre>
from sklearn.metrics import confusion_matrix

confusion_matrix(y_true, y_pred)
</pre>

Negatives | Positives
----------|----------
<b>T</b>rue <b>N</b>egatives | <b>F</b>alse <b>P</b>ositives
<b>F</b>alse <b>N</b>egatives | <b>T</b>rue <b>P</b>ositives

---------------------------------
https://towardsdatascience.com/understanding-confusion-matrix-a9ad42dcfd62

- <b>Recall</b> = <b>TP</b> / (<b>TP</b> + <b>FN</b>)  
Out of all the positive classes, how much we predicted correctly. It should be high as possible.

- <b>Precision</b> = <b>TP</b> / (<b>TP</b> + <b>FP</b>)  
Out of all the classes, how much we predicted correctly. It should be high as possible.

- Accuracy = (TP + TN) / Total

- <b>F Measure</b> (Fscore) = (<b>2</b> * <b>Recall</b> * <b>Precision</b>) / (<b>Recall</b> + <b>Precision</b>)  
It is difficult to compare two models with low precision and high recall or vice versa. So to make them comparable, we use F-Score. F-score helps to measure Recall and Precision at the same time. It uses Harmonic Mean in place of Arithmetic Mean by punishing the extreme values more.
