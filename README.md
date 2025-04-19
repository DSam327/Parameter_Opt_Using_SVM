# Parameter_Opt_Using_SVM
Parameter Optimization Using SVM
Methodology
This project focuses on optimizing Support Vector Machine (SVM) parameters for a multi-class classification task using a dataset from the UCI Machine Learning Repository. The selected dataset is the Letter Recognition dataset, containing 20,000 samples of handwritten capital letters represented by 16 numerical features.

Steps:
Dataset Selection & Preprocessing

Used the Letter Recognition dataset.

Encoded target labels.

Normalized features using StandardScaler.

Train-Test Sampling

Performed 10 different random 70-30 train-test splits (S1 to S10) using different seeds.

SVM Optimization

For each sample:

Performed 100 iterations of hyperparameter tuning using RandomizedSearchCV.

Optimized over kernel types (rbf, poly, sigmoid), C, gamma, and degree.

Evaluated accuracy using 3-fold cross-validation.

Evaluation

Recorded the best accuracy and corresponding SVM parameters for each sample.

Identified the sample with the highest test accuracy.

Plotted a convergence grap

Result Table
Sample  Accuracy                         Best Params
0     S1  0.972333        rbf, C=9.92, degree=5, gamma=auto
1     S2  0.966667        rbf, C=9.92, degree=5, gamma=auto
2     S3  0.970667        rbf, C=9.90, degree=5, gamma=scale
3     S4  0.967500        rbf, C=9.76, degree=3, gamma=auto
4     S5  0.964333        rbf, C=9.10, degree=4, gamma=scale
5     S6  0.969333        rbf, C=9.92, degree=5, gamma=auto
6     S7  0.966000        rbf, C=8.66, degree=3, gamma=auto
7     S8  0.970167        rbf, C=9.90, degree=5, gamma=scale
8     S9  0.971333        rbf, C=9.92, degree=5, gamma=auto
9    S10  0.971333        rbf, C=9.76, degree=3, gamma=auto

Convergence Graph
![image](https://github.com/user-attachments/assets/f81a1faf-21b7-4c8f-babe-4b86ccf3b8b4)




