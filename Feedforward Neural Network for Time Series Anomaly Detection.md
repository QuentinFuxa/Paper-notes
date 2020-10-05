https://arxiv.org/pdf/1812.08389.pdf

In this article, the authors propose to use a fully connected neural network for the **detection of anomalies in time series**. 

The network is trained to calculate the probability that a new data is an anomaly. Training takes place over labeled time series.
The interest of the publication is not so much in the type of network used, which is classic here, but rather in the features extracted from the time series.
Thus, while the majority of methods use a single time window on the data passed, the length of which can sometimes adjust automatically during training, the idea here is to use several temporal windows to better capture the temporal patterns likely to appear at different scales. 
Thus, in the publication problem, the authors noticed that their temporal problem depended at the same time on very close data, ie on a temporal window from t-1 to t-k, but also larger and difficult to describe time scales.
They therefore took the time information from the day before at the same instant, and therefore a window from t-k-24h to t + k-24h. 

Finally, the authors noticed a periodicity within the week, and therefore include the time window of a week before: from t-k-7days a t+k-7 days. 

![](https://github.com/QuentinFuxa/Paper-notes/blob/master/Feedforward_Neural_Network_for_TS_Anomaly_Detection.png)


This method illustrates a way of easily adding problem knowledge (i.e. periodicities that have an impact), working uniquely on the data.
