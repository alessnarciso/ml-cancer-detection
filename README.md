# ml-cancer-detection
Predicting if breast cancer tumors are malignant or benign using machine learning techniques.

In this Jupyter notebook, I will be working with the following data set from UC Irvine's Machine Learning Repository.

The wdbc.data data set used can be found here:

https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29 

https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/

In this notebook, I first pre-process and visualize the data using Seaborn and Numpy. 

Then I build 2 shallow neural networks and compare the results between those solutions and conventional machine learning techniques like logistic regression, random forest, and decision tree classifiers. 

The neural networks were built using TensorFlow and Keras. The second neural network utilized dropout, batch normalization, and He normalization.

The other machine learning techniques were implemented using Sklearn.

Overall, the most accurate solutions were the basic shallow neural network and the linear regression classifier, likely because most of the data was linearly separable. This had an test accuracy of around 98% and an AUC of about 0.99 in the test data AUC ROC curve. 

When conducting feature importance analysis on the linear regression model, it seems that the most important feature for predicting malignant tumors is the mean fractal dimension.

This seems consistent with various medical studies where it has been determined that fractal dimension displays diagnostic potential in distinguishing malignant from benign cells in breast cancer. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6349609/)