# AnomalyDetection

## Project: Anomaly detection in wide area network mesh using two Machine Learning anomaly detection algorithms

### Install
This project requires Python 2.7 and the following Python libraries installed:

* [NumPy](http://www.numpy.org/)
* [Pandas](http://pandas.pydata.org/)
* [matplotlib](https://matplotlib.org/)
* [scikit-learn](http://scikit-learn.org/stable/)
* [Keras](https://keras.io/)

You will also need to have software installed to run and execute a [Jupyter Notebook](https://jupyter.org/)

If you do not have Python installed yet, it is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included.

### Code
The code for each experiment can be found in the AnomalyDetection file along with this README. You will be required to use the simulated_data.py Python file for all code using Boosted Decision Trees (BDT) involving simulated data.

The following is a summary of each file in the order of its use in the paper.

*A. Boosted Decision Trees*

*A.1. Decision Stumps vs. Decision Trees*  
TestingBDTonSimulatedDataSTUMPS.ipynb  
Tested the effectiveness of boosted decision trees utilizing trees of depth one (decision stumps) on simulated data.  

TestingBDTonSimulatedDataTREES_6.ipynb  
Tested the effectiveness of boosted decision trees utilizing trees of depth 6 on simulated data.  

*A.2. Anomaly Duration vs. Degree of Anomalous Behavior*  
BDTonSimulatedDataDegreeDurationTest.ipynb  
Data fluctuates the degree to which an anomaly differed from normal data, the duration of anomalous behavior, and the number of timeseries affected for a simulated data set.

*A.3 Application on real data*  
PacketLossWithAnalysis&Delay-30days.ipynb
Tested the decision trees on a period of 30 days of real data.

*B. Simple feed forward neural network*

*B1. Application on simulated data*

*B2. Impact of duration, magnitude of anomaly, and number of affected timeseries*

*B3. Performance on actual data*

The code is provided in the  
You will also have be required to use the included 

BDTonSimulatedDataDegreeDurationTest.ipynb

### Data
We use two different datasets to test the functionality of the new machine learning algorithms as applied to network anomaly detection: one a simulated data, the other, real data.  

Features

Throughput: the amount of data that can be transferred over a period of time (25s)  
Packet loss rate: the percentage of lost packets over the total transferred packets in one-minute intervals  
One-way delay (OWD): delay (in ms) separately for each direction of a path  
Traceroute: the path and transition time between the source and destination  
