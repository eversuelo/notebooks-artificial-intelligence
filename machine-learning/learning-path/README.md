# Learning Path

A self-study route through machine learning, organized by topic. The notes are a compendium drawn from several books and tutorials and rewritten in my own words. Each module gets a folder here with a study guide and a notebook. The topic notebooks in the rest of the repo plug in as companions.

Paths in these guides are written from the repository root.

## How each module works

1. Read about the topic in the sources you are using.
2. Open the module folder. `README.md` lists what the repo already covers, sets the study order and has a checklist.
3. Work through the module notebook: read the notes, run the demos, solve the exercises.
4. Do the companion notebooks listed in the study guide.
5. Answer the self-check at the end of the notebook, tick the checklist and update the table below.

Every figure is drawn with code. Exercise cells are left empty for you to solve.

## The path

Module 1 has been compared with the repo topic by topic. For the other modules the mapping is a first pass based on the headings of the existing notebooks. Review each one when you reach it.

| # | Module | Topics | Material in this repo | Status |
|---|---|---|---|---|
| 0 | Python tools | NumPy, pandas, Matplotlib, seaborn, statsmodels | `libraries/introduction.ipynb`, `libraries/numpy/introduction.ipynb`, `libraries/pandas/introduction.ipynb` | Available |
| 1 | Learning from data | What ML is, the three types of learning, notation, the ML workflow, Python setup | [Study guide](learning-from-data/README.md), [notebook](learning-from-data/learning-from-data.ipynb). Companions: `introduction.ipynb`, `machine-learning/supervised-learning/introduction.ipynb`, `machine-learning/supervised-learning/decision-trees/how-models-work.ipynb` | Ready to study |
| 2 | Data and exploratory analysis | Datasets, data types and scales, distance and similarity measures, sampling | `data-analysis/datasets.ipynb`, `machine-learning/supervised-learning/introduction.ipynb` | Available, no study guide yet |
| 3 | Math for machine learning | Linear algebra, calculus, probability, optimization | | Not started |
| 4 | First classifiers | Perceptron, adaptive linear neurons, gradient descent | `machine-learning/supervised-learning/perceptron/neuron-perceptron.ipynb` (perceptron on the AND gate, convergence, XOR) | Partial |
| 5 | Regression | Simple and multiple linear regression, least squares, regression metrics | `machine-learning/supervised-learning/linear-regression/simple-linear-regression.ipynb` | Partial |
| 6 | A tour of classifiers | Logistic regression, support vector machines, decision trees, k-nearest neighbors | `machine-learning/supervised-learning/decision-trees/how-models-work.ipynb` (decision tree intuition only) | Partial |
| 7 | Data preprocessing | Missing values, categorical data, feature scaling, feature selection | `data-analysis/datasets.ipynb` (scales, quantization) | Partial |
| 8 | Dimensionality reduction | PCA, LDA, nonlinear methods | | Not started |
| 9 | Model evaluation and tuning | Pipelines, cross-validation, learning curves, hyperparameter search, metrics | | Not started |
| 10 | Ensembles | Voting, bagging, random forests, boosting | | Not started |
| 11 | Clustering | k-means, hierarchical clustering, density-based clustering | Distance measures in `machine-learning/supervised-learning/introduction.ipynb` | Groundwork only |
| 12 | Neural networks from scratch | Multilayer perceptron, backpropagation | | Not started |
| 13 | Deep learning with PyTorch | Tensors, automatic differentiation, training loops | | Not started |
| 14 | Computer vision | Convolutional neural networks, image classification | | Not started |
| 15 | Sequences and language | Recurrent networks, attention, transformers, language models | | Not started |
| 16 | Generative models | Autoencoders, GANs | | Not started |
| 17 | Reinforcement learning | Agents, rewards, value functions, Q-learning | | Not started |

## Outside tutorials

| Tutorial | Source | Where it lives | Used in |
|---|---|---|---|
| How Models Work | [Kaggle Learn, Intro to Machine Learning, lesson 1](https://www.kaggle.com/code/dansbecker/how-models-work) (Dan Becker, Apache 2.0) | `machine-learning/supervised-learning/decision-trees/how-models-work.ipynb` | Module 1 (fitting and predicting), module 6 (decision trees) |

## Adding a module

1. Create `machine-learning/learning-path/short-name/`.
2. Write `README.md`: a table of the module's topics against the repo (covered, partial, missing), the study order and a checklist.
3. Write `short-name.ipynb`: notes, demos and exercises with empty solution cells.
4. Update the table above.
