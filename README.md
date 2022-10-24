# certificate_tutorial_week6_aglo
week6 algo trading certificate project
**Prediction-based Trading & Event-based Backtesting**

Implement a class that uses **event-based backtesting** to backtest the following prediction-based strategy:

* Data from `http://hilpisch.com/ref_eikon_eod_data.csv`.
* Select one symbol from the data set.
* Create the following features:
    * log return
    * direction (up or down)
    * log return as 5 categories
    * two SMAs (short and long window)
    * difference between the SMAs
    * two EWMAs (short and long window)
    * difference between the EWMAs
    * two rolling volatilities (short and long window)
* Split the data set into training (70%) and testing data.
* Normalize the training features data to have
    * zero mean and
    * standard deviation of one.
* Normalize the test features data by the same moment values as the training data.
* Create lagged features data for 5 lags.
* Train and (back-)test the following algorithms for directional (long/short) trading (from `scikit-learn`):
    * `GaussianNB()`
    * `LogisticRegression()`
    * `DecisionTreeClassifier()`
    * `SVC()`
    * `MLPClassifier()`
* Compare the performance of the different models numerically.

For the implementation, you can rely e.g. on the Python classes as presented in the PyAlgo class sessions and the resources.
