# Decision Tree Classifier from Scratch — Iris Dataset

## About the Project

I built this project to understand how a Decision Tree classifier works internally, rather than relying entirely on a machine learning library.

Using Python and NumPy, I implemented the main parts of a Decision Tree algorithm from scratch and tested it on the Iris dataset. The project helped me understand how a tree selects features, splits data, and makes predictions.

## What I Implemented

- **Entropy** — measures how mixed the class labels are in a dataset.
- **Information Gain** — measures how much a split reduces uncertainty.
- **Best Split Selection** — searches for a feature and threshold that provide the highest information gain.
- **Data Splitting** — divides samples into left and right branches based on a threshold.
- **Recursive Tree Construction** — builds the tree by repeatedly splitting the data.
- **Leaf Nodes** — stores a class label when a node becomes a leaf.
- **Prediction** — follows the decision rules from the root to a leaf to predict a sample's class.
- **Accuracy Evaluation** — compares predictions with actual labels to calculate test accuracy.

## Dataset

This project uses the Iris dataset, a commonly used dataset for learning classification.

It contains:

- 150 flower samples
- 4 numerical features
- 3 target classes: Setosa, Versicolor, and Virginica

The four features are sepal length, sepal width, petal length, and petal width.

## How the Algorithm Works

The classifier starts by measuring the impurity of the current dataset using entropy.

It then evaluates possible splits and uses information gain to select the best one. The dataset is divided into two branches according to the selected feature and threshold.

This process continues recursively until all samples in a node belong to the same class or no split with positive information gain is found. In the latter case, the implementation predicts the majority class.

To classify a new sample, the model follows the learned decision rules until it reaches a leaf node.

## Train and Test

The dataset is divided into training and testing sets:

- Training set: 80%
- Testing set: 20%
- Random state: 42

The model is trained using the training set and evaluated on the test set.

The test accuracy obtained from this split was **100%**. This result applies only to this particular split and does not guarantee the same accuracy on other datasets.

## Technologies Used

- Python
- NumPy
- scikit-learn — for loading the Iris dataset and splitting the data
- Jupyter Notebook

The Decision Tree algorithm itself is implemented from scratch rather than using scikit-learn's built-in Decision Tree classifier.

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

   `pip install numpy scikit-learn jupyter`

3. Open Jupyter Notebook:

   `jupyter notebook`

4. Open `decision-tree-from-scratch-iris.ipynb`.
5. Run the cells in order.

## What I Learned

Through this project, I gained practical experience with entropy, information gain, recursive algorithms, and classification.

More importantly, implementing the algorithm myself helped me connect the mathematical concepts behind Decision Trees with the code that makes predictions.

## Future Improvements

- Add a maximum tree depth to control tree growth.
- Implement minimum sample requirements for splitting.
- Compare the results with scikit-learn's Decision Tree classifier.
- Evaluate the model using additional classification metrics.

## Author

**Dulsara Abeybandara**

GitHub: [Dulsaraabeybandara](https://github.com/Dulsaraabeybandara)
