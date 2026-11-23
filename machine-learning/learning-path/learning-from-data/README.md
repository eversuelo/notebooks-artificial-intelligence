# Learning from Data

Study guide for module 1 of the learning path: what machine learning is, the three types of learning, the vocabulary and notation, the workflow of an ML project and the Python setup. It lists what the repository already covered and sets the order to study the module.

## What the repo covered before this module was added

The repo had no notebook for this module. Parts of it were spread across four notebooks, and several topics were missing.

| Topic | Status | Where it was | What was missing |
|---|---|---|---|
| What machine learning is | Partial | `introduction.ipynb` defines ML, DL and AI | The idea of learning rules from data instead of writing them, and the application examples |
| The three types of machine learning | Missing | The words "supervised", "unsupervised" and "reinforcement" appeared in no notebook | The whole taxonomy |
| Supervised learning: classification | Partial | `machine-learning/supervised-learning/perceptron/neuron-perceptron.ipynb` trains a classifier on the AND gate | Definitions of binary and multiclass classification, decision boundary on a 2D dataset |
| Supervised learning: regression | Covered | `machine-learning/supervised-learning/linear-regression/simple-linear-regression.ipynb` goes further than this module (least squares, metrics, a practical case) | Only the link back to the taxonomy |
| Reinforcement learning | Missing | Nowhere | Agent, environment, state, action, reward |
| Unsupervised learning: clustering | Partial | `machine-learning/supervised-learning/introduction.ipynb` covers distance and similarity measures, which clustering builds on | Clustering itself |
| Unsupervised learning: dimensionality reduction | Missing | Nowhere | The whole topic |
| Notation and conventions | Partial, with a conflict | `machine-learning/supervised-learning/introduction.ipynb` loads Iris and writes the data matrix | The repo uses the opposite index convention (see below) |
| Machine learning terminology | Partial | Terms such as feature, attribute and class appear in several notebooks | The synonym list, loss vs. cost function |
| Workflow: preprocessing | Partial | Phases of a data project in `introduction.ipynb`; scales and quantization in `data-analysis/datasets.ipynb` | Feature scaling, and fitting preprocessing on the training set only |
| Workflow: training and selecting a model | Partial | `train_test_split` is used in the linear regression notebook | No free lunch, accuracy, cross-validation, hyperparameters |
| Workflow: evaluating and predicting | Partial | Test-set metrics in the linear regression notebook | Generalization error as a concept |
| Python setup | Partial | `libraries/introduction.ipynb` and the NumPy and pandas notebooks cover the libraries in depth | Installing with pip and conda, virtual environments, pinned versions. The repo has no `requirements.txt` |

Other things the repo has that belong to later modules: Minkowski norms, Hamming distance, similarity measures, edit distance, sampling and quantization, seaborn and statsmodels.

### The notation conflict

This path writes $x_j^{(i)}$ with the superscript for the training example (row) and the subscript for the feature (column), which is the common convention in machine learning texts. `machine-learning/supervised-learning/introduction.ipynb` does the reverse: its matrix has $x_1^{(1)}, x_1^{(2)}, \dots, x_1^{(p)}$ in the first row, so the subscript is the example and the superscript is the feature.

Keep it in mind when you read that notebook, or change its matrix to match.

## What was added

`learning-from-data.ipynb` goes through the module section by section. It has short notes, demos drawn with code, and exercises with empty cells for you to solve.

| Notebook section | Demos | Exercises |
|---|---|---|
| 1. What machine learning is | | 1.1 |
| 2. The three types of learning | Classification boundary, regression line, k-means clustering, Swiss roll reduction | 2.1 to 2.4 |
| 3. Terminology and notation | Iris as a 150 × 4 matrix | 3.1, 3.2 |
| 4. Roadmap for an ML system | Split, scale, train and evaluate on Iris | 4.1 to 4.4 |
| 5. Python setup | Version check | 5.1, 5.2 |
| 6. Self-check | | 8 questions |

The regression demo uses synthetic data generated in the notebook.

## Study order

1. Skim `introduction.ipynb` at the repo root for the course framing.
2. In `learning-from-data.ipynb`, do sections 1 and 2 up to the regression demo.
3. Do the companion tutorial `machine-learning/supervised-learning/decision-trees/how-models-work.ipynb`. It is lesson 1 of Kaggle's Intro to Machine Learning, [How Models Work](https://www.kaggle.com/code/dansbecker/how-models-work). It shows what fitting and predicting mean with a small decision tree for house prices, and it has six exercises.
4. Finish section 2 of the module notebook (reinforcement and unsupervised learning).
5. Do section 3. Compare with `machine-learning/supervised-learning/introduction.ipynb` and note the index convention.
6. Do section 4. Its exercises are the longest in the notebook.
7. Do section 5. If the libraries are new to you, go through `libraries/introduction.ipynb`, `libraries/numpy/introduction.ipynb` and `libraries/pandas/introduction.ipynb` first.
8. Answer the self-check in section 6 without looking at the notes.

## Checklist

- [ ] Exercise 1.1
- [ ] Exercises 2.1 and 2.2 (supervised learning)
- [ ] Companion tutorial: How Models Work, exercises 1 to 6
- [ ] Exercise 2.3 (reinforcement learning)
- [ ] Exercise 2.4 (unsupervised learning)
- [ ] Exercises 3.1 and 3.2 (notation)
- [ ] Exercises 4.1 to 4.4 (workflow)
- [ ] Exercise 5.1: dedicated environment
- [ ] Exercise 5.2: `requirements.txt` or `environment.yml` in the repo
- [ ] Self-check, 8 questions
