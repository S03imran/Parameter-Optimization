# Parameter Optimization of SVM

# ASSIGNMENT
Choose any multi-class dataset. Divide the dataset into 70-30 for training and testing with 10 dufferent samples. Optimize the SVM for every sample and report the best parameters.

# Dataset
The data used contains 14 columns and 10,000 rows. It is a synthetic dataset that reflects real predictive maintenance data encountered in industry. Out of 14 columns, the following 7 columns are used:

Type
-> Air temperature
-> Process Tempature
-> Rotational Speed
-> Torque
-> Tool wear

# Methodology
The dataset is split into training and testing set for 10 times and the following SVC classifier hyperparameter are selected for best accuracy:

-> Kernel - Selected from RBF, Polynomial, Linear and Sigmoid
-> C (Regularisation parameter) - Random integer values from 1 to 7
-> Gamma (Kernel coefficient) - Random integer values from -1 to 7. If the value is less than 1, then gamma is randomly set as auto or scale. It is used only by rbf,                                     poly and sigmoid kernel.
-> Degree - Random integer from 1 to 5. It is only used by poly kernel and represent the degree of polynomial kernel function.

The above hyperparameters are randomly selected from the given values for 100 iterations. The parameters that gave the best accuracy for each sample are shown in table below:

![Capture](https://user-images.githubusercontent.com/84433199/233135079-b3c22873-209b-4a22-a7be-bb28e67404a8.JPG)

# Convergence Graph is given below

![Capture](https://user-images.githubusercontent.com/84433199/233135580-952eb743-b5b4-4a01-8c8b-4ec593c0f7ef.JPG)

# Result
The best parameters of SVC for the given dataset are:->
-> Kernel : r->bf
-> C : 7
-> Gamma : scale
-> Degree : NA
The above parameter gave a maximum accuracy of 0.983667.
