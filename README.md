# Linear-Regression-Tensorflow
This Jupyter Notebook demonstrates building a neural network for regression using Tensor Flow on the Kaggle Medical Cost Personal Dataset. The dataset contains information about the medical cost personal information for individuals who have bought insurance.

In this notebook, the dataset is preprocessed, scaled using feature scaling, and split into training and testing sets. Then, three different models are built, and each model is trained for 35 epochs using Tensor Flow.

# Dataset
The Kaggle Medical Cost Personal Dataset contains the following features:

- age: age of primary beneficiary
- sex: gender of primary beneficiary
- bmi: body mass index (kg/m^2)
- children: number of children covered by health insurance / number of dependents
- smoker: smoking status of primary beneficiary (yes/no)
- region: the beneficiary's residential area in the US
- charges: individual medical costs billed by health insurance
# Feature Scaling
Feature scaling is performed on the dataset to ensure that all features are in the same range. This is done to prevent any one feature from dominating the others during training.

# Models
Three different models are built in this notebook:

- First Model: This model is run for 100 epochs and has an adam optimizer of 0.001
- Second Model: This model is run for 175 epochs and has an adam optimizer of 0.08
- Third Model: This model is run for 100 epochs and has an adam optimizer of 0.001 but a min max scale and one hot encoder from sklearn library is used on the data 
All models use the same optimizer, loss function, and metric. The optimizer used is Adam, the loss function is mean squared error, and the metric is mean absolute error.

# Results
The performance of each model is evaluated by comparing the mean absolute error of the predicted values to the actual values on the testing set. The loss curves are plotted

#Dependencies
This Jupyter Notebook requires the following dependencies:

- Tensor Flow
- Pandas
- Matplotlib
Conclusion
This notebook demonstrates how to build a neural network for regression using Tensor Flow. By using feature scaling, the dataset is preprocessed to ensure that all features are in the same range. Three different models are trained for 35 epochs, and the performance of each model is evaluated. Finally, the results are plotted to show the performance of each model over the 35 epochs.
