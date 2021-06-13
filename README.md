# Heartbeat_classification
Predicted whether heartbeat is Normal or not using sequence models

The dataset [Link](http://timeseriesclassification.com/description.php?Dataset=ECG5000) contains 5,000 Time Series examples (obtained with ECG) with 140 timesteps. Each sequence corresponds to a single heartbeat from a single patient with congestive heart failure.

The original dataset has 5 types of hearbeats (classes):
1.	Normal (N)
2.	R-on-T Premature Ventricular Contraction (R-on-T PVC)
3.	Premature Ventricular Contraction (PVC)
4.	Supra-ventricular Premature or Ectopic Beat (SP or EB)
5.	Unclassified Beat (UB).

The dataset used here has been modified slightly. I have combined 2,3,4,5 into one class. This is labelled as 0. So we will have binary classification task – predict whether the hearbeat is Normal or not based on sequence of 140 frequencies.

Models used:
1. Simple RNN (single layer)
2. LSTM (single layer)
