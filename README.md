# Parameter_Opt_Using_SVM
Parameter Optimization Using SVM

### Methodology
This project focuses on optimizing Support Vector Machine (SVM) parameters for a multi-class classification task using a dataset from the UCI Machine Learning Repository. The selected dataset is the Letter Recognition dataset, containing 20,000 samples of handwritten capital letters represented by 16 numerical features.

### Steps:
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

### Evaluation

Recorded the best accuracy and corresponding SVM parameters for each sample.

Identified the sample with the highest test accuracy.

Plotted a convergence graph

### Result Table

![image](https://github.com/user-attachments/assets/6234bbb5-b95d-457a-b432-99d82a37292a)


### Convergence Graph
![image](https://github.com/user-attachments/assets/f81a1faf-21b7-4c8f-babe-4b86ccf3b8b4)




