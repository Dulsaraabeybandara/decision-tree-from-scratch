# Decision Tree Classifier from Scratch

A Decision Tree classification algorithm implemented from scratch using Python and NumPy, without relying on Scikit-learn's built-in Decision Tree implementation.

## About the Project

The main goal of this project is to understand the mathematical concepts and internal working mechanisms behind Decision Tree classifiers by implementing the algorithm from scratch.

Instead of using an existing machine learning implementation, I built the core components of the algorithm using Python and NumPy and applied them to the Iris dataset.

This project focuses on understanding how a Decision Tree selects optimal features, determines splitting thresholds, recursively constructs a tree, and makes predictions.

## Key Concepts Implemented

- **Entropy:** Measures the impurity or uncertainty of class labels.
- **Information Gain:** Measures the reduction in entropy after a split.
- **Best Split Selection:** Finds the feature and threshold that produce the highest information gain.
- **Data Splitting:** Divides the dataset into left and right branches.
- **Recursive Tree Construction:** Builds the decision tree recursively.
- **Leaf Nodes:** Assigns class labels to terminal nodes.
- **Prediction:** Classifies new samples by traversing the constructed tree.
- **Accuracy Evaluation:** Evaluates classification performance using test accuracy.

## Dataset

This project uses the **Iris dataset**, a well-known dataset for classification tasks.

| Property | Description |
|---|---|
| Total samples | 150 |
| Features | 4 |
| Target classes | 3 |
| Feature types | Numerical |

**Features:**
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

**Target Classes:**
- Setosa
- Versicolor
- Virginica

## How the Algorithm Works

The implemented Decision Tree follows these steps:

1. Calculate the entropy of the current dataset.
2. Evaluate possible feature and threshold combinations.
3. Calculate information gain for each candidate split.
4. Select the split with the highest information gain.
5. Divide the dataset into left and right branches.
6. Recursively repeat the process to construct the tree.
7. Stop splitting when a stopping condition is reached.
8. Predict the class of a new sample by traversing the tree.

If a node cannot be split further, the implementation uses the majority class as its prediction.

## Model Evaluation

The dataset was divided into training and testing sets.

| Parameter | Value |
|---|---|
| Training data | 80% |
| Testing data | 20% |
| Random State | 42 |
| Test Accuracy | 100% |

The model achieved **100% test accuracy** on this particular train-test split.

Note: This result represents one specific split of the Iris dataset and does not necessarily indicate the same performance on other datasets.

## Technologies Used

- Python
- NumPy
- Scikit-learn (dataset loading and train-test splitting)
- Jupyter Notebook

**Important:** The Decision Tree algorithm itself was implemented from scratch. Scikit-learn's built-in Decision Tree classifier was not used for model training or prediction.

## Project Structure

```text
decision-tree-from-scratch/
│
├── decision-tree-from-scratch-iris.ipynb
│
└── README.md
```

## Installation and Usage

**1. Clone the repository**

```bash
git clone https://github.com/Dulsaraabeybandara/decision-tree-from-scratch.git
```

**2. Navigate to the project directory**

```bash
cd decision-tree-from-scratch
```

**3. Install the required libraries**

```bash
pip install numpy scikit-learn jupyter
```

**4. Start Jupyter Notebook**

```bash
jupyter notebook
```

**5. Open the notebook**

Open `decision-tree-from-scratch-iris.ipynb` and run the cells sequentially.

## What I Learned

Through this project, I developed a deeper understanding of:

- Entropy and Information Gain.
- Mathematical foundations of Decision Trees.
- Finding optimal splitting criteria.
- Recursive algorithms and tree structures.
- Implementing machine learning algorithms using NumPy.
- The relationship between mathematical concepts and their practical implementation.

Most importantly, this project helped me understand how a Decision Tree classifier works internally rather than treating it as a black-box machine learning model.

## Future Improvements

- Implement maximum tree depth.
- Add minimum samples per split.
- Support additional datasets.
- Compare results with Scikit-learn's Decision Tree implementation.
- Evaluate using precision, recall, F1-score and confusion matrix.

## Author

**Dulsara Abeybandara**

GitHub: [@Dulsaraabeybandara](https://github.com/Dulsaraabeybandara)
