# SVM
SVM stands for Support Vector Machines. It is a popular supervised machine learning algorithm used for classification and regression tasks. 

In SVM, the algorithm takes a set of labeled training data and tries to find the optimal hyperplane that separates the data points of different classes with the largest margin. The hyperplane is a decision boundary that maximizes the distance between the closest data points of different classes, known as support vectors.

The main idea behind SVM is to transform the input data into a higher-dimensional feature space using a kernel function, which allows for nonlinear separation of classes in the original input space. SVM aims to find the hyperplane that not only separates the data points accurately but also generalizes well to new, unseen data.

SVM can be used for both binary classification, where it separates data points into two classes, and multiclass classification, where it extends the binary classification approach to handle multiple classes. In the case of regression, SVM aims to find a hyperplane that best fits the data points with a minimal error.

SVM has several advantages, including its ability to handle high-dimensional data, effectiveness in dealing with nonlinear separation, and robustness against overfitting. However, SVM can be computationally expensive, especially for large datasets, and it may require careful selection of hyperparameters to achieve optimal performance.

### Grid Search in SVM
Grid search can be applied to SVMs to find the optimal combination of hyperparameters for the SVM model. The key hyperparameters that can be tuned in SVM include:

1. C: The regularization parameter that controls the trade-off between achieving a low training error and a low complexity model. A smaller C value emphasizes a larger margin, allowing more training points to be misclassified, while a larger C value enforces a stricter classification of training points.

2. Kernel: The kernel function used to transform the data into a higher-dimensional space. Common choices include linear, polynomial, radial basis function (RBF), and sigmoid kernels.

3. Gamma: The parameter used in certain kernel functions (such as RBF) to define the influence of a single training example. A smaller gamma value leads to a larger influence and a smoother decision boundary, while a larger gamma value results in a more complex and wiggly decision boundary.

To perform grid search for SVM, you need to define a grid of possible values for each hyperparameter. For example, you can specify a range of values for C, a list of kernel functions to try, and a range of gamma values. The grid search algorithm will then train and evaluate the SVM model for each combination of hyperparameters in the grid.

The evaluation can be done using a suitable performance metric, such as accuracy, precision, recall, or F1 score. You can use cross-validation to obtain reliable estimates of the model's performance for each set of hyperparameters.

The grid search algorithm will identify the combination of hyperparameters that achieves the best performance on the validation set. This combination can then be used to train the final SVM model, and the performance can be evaluated on an independent test set.

Grid search helps in automating the process of hyperparameter tuning and finding the best hyperparameter values for SVM, optimizing its performance for a given dataset and task.
## Project:
In this project, we will be analyzing the famous iris data set!
#### The Data
We will be using the famous Iris flower data set.

The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by Sir Ronald Fisher in the 1936 as an example of discriminant analysis.

The data set consists of 50 samples from each of three species of Iris (Iris setosa, Iris virginica and Iris versicolor), so 150 total samples. Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters.
The iris dataset contains measurements for 150 iris flowers from three different species.

The three classes in the Iris dataset:

Iris-setosa (n=50)
Iris-versicolor (n=50)
Iris-virginica (n=50)
The four features of the Iris dataset:

sepal length in cm
sepal width in cm
petal length in cm
petal width in cm

