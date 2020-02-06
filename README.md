# Data Set and Code Repository for the Article, "Distributed Proprioception of 3D Configuration in Soft Sensorized Robots via Deep Learning"

In this SoftArm repository of SensoSoRo, we provide the data sets and relevant MATLAB scripts used in the journal article 

> "R L Truby, C Della Sandina, Daniela Rus. Distributed Proprioception of 3D Configuration in Soft Sensorized Robots via Deep Learning. IEEE Robotics and Automation Letters, 2020." [1]

Data sets provided here include the raw training and validation sets used in this publication, along with the training scripts used as well. We intend to update this repository over time as necessary and/or upon reasonable request.

## Getting Started and Navigation

We use MATLAB 2019 and MATLAB's Deep Learning Toolbox for all analysis, data processing, and training of neural networks. Data sets are currently provided as .mat files, and training scripts are provided as .m files.

In the repo, find the following data sets:

```
XTraining.mat
YTraining.mat
XValidation.mat
YTraining.mat
```
In these file names, "X" and "Y" refer to "inputs" and "outputs" to the model, respectively. Thus, XTraining.mat contains time series data from 12 sensor readings (all in units V), and YTraining.mat contains the time series data from 9 kinematic parameters, $q_i$. "Training" and "Validation" refer to which data sets are used for training and validation (and later testing, according to the practices introduced by Reference [2]), respectively.

## Data Sets

At present, we have provided the raw compiled data sets used for training and validation in our work. We are not yet providing discrete data sets from various actuation sequences, as we are still working with these for ongoing projects.  

```
Give the example
```
## Training script

The current training script is a portion of code taken from a master script that we used in our work. To train the neural network, which is currently specified with the hyperparameters used in the "RMSE = 1.27 mm", LSTM-based network investigated in our paper, load the data sets into the workspace, and run the script 

```
TrainNeuralNetwork.m
```

## Neural Network Training 

Please refer to our calculation for RMSE, not that used by MATLAB's Deep Learning Toolkit. 

## Authors

* **Ryan L. Truby, PhD** 
* **Cosimo Della Santina, PhD**

First authored on February 6, 2020. 

## References

[1] RL Truby, Cosimo Della Santina, Daniela Rus. Distributed Proprioception of 3D Configuration in Soft, Sensorized Robots via Deep Learning. IEEE Robotics and Automation Letters, 2020. In press.

[2] TG Thuruthel, B Shih, C Laschi, MT Tolley. Soft robot perception using embedded soft sensors and recurrent neural networks. SCience Robotics, 2019. Vol 4, No 26, eaav1488.




