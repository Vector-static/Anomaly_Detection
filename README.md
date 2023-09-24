# Anomaly_Detection
this project uses python and a concept of big data to find anomaly in large datasets in order to be precise in cases of crucial datasets of big companies.



so initially we import all the necessary libraries we can use kaggle but an other libraries including open sources ones are welcomed
then we need to have a package called 'IsolationForest' which will the main tool to detect the anomaly(firstly install by pip then  import it)
then we need to import the 'blob' feature for our visualisation
Using make_blobs synthetic clustered data of 300 samples is generated additionally 50 random outlier data points are created using np.random.uniform.

Then model training:
An IsolationForest model is initialized specifying that an estimated 10% (contamination=0.1) of the data are outliers.
The model is then trained (fit) on the combined dataset of normal data and outliers


Anomaly Detection and Visualization:
The trained model is used to predict whether each data point is normal or an anomaly normal points are labeled 1 and anomalies are labeled -1.
The results are visualized using matplotlib where green points represent normal data  and red points represent detected anomalies
