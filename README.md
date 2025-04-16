# Data_Mining_2_Decision_Tree

This repository contains an R Markdown assignment report focused on applying decision tree classification techniques to a structured dataset. The analysis walks through preprocessing, model training, evaluation, and visualization using R's powerful modeling libraries.

---

### 🧩 Business Problem

In classification problems, especially in domains like customer segmentation, credit scoring, or risk assessment, having interpretable models that can provide clear decision rules is essential. Decision trees are widely used for this purpose due to their ease of interpretation and visual simplicity.

This assignment aimed to build and evaluate a decision tree classifier to predict a target outcome based on structured input variables. The project emphasized understanding how tree-based models work and how their performance can be measured using classification metrics.

---

### 🎯 Project Objective

The objective of this assignment was to:

- Preprocess a dataset for decision tree modeling
- Train and tune a **Classification Tree** using the `rpart` library
- Evaluate the model using a **confusion matrix**, **accuracy**, **precision**, and **recall**
- Visualize the decision rules using tree plots
- Interpret key variables and their decision boundaries

The overall goal was to gain hands-on experience with one of the most interpretable machine learning models in R.

---

### 🛠️ Group Solution

The assignment followed a well-structured modeling workflow:

- **Data Preparation**: Cleaned and split the dataset into training and test sets using stratified sampling techniques to ensure balanced class distribution.
- **Model Training**: Utilized `rpart` to train a classification tree with default and tuned hyperparameters (`cp` and `minsplit`).
- **Model Evaluation**:
  - Used `predict()` and `confusionMatrix()` from the `caret` package to assess test performance.
  - Compared classification metrics across different pruning levels to avoid overfitting.
- **Visualization**: Plotted decision trees using both `rpart.plot` and `fancyRpartPlot` for interpretability.
- **Feature Insights**: Interpreted which variables were most influential in classifying the target.

---

### 💡 Business Value

Although this was an academic assignment, the modeling approach aligns closely with real-world decision-making use cases:

- **Interpretability**: Decision trees are highly intuitive, allowing stakeholders to understand model logic without a technical background.
- **Rapid Prototyping**: Tree-based models can be trained quickly, enabling fast iteration.
- **Explainable AI (XAI)**: Trees provide clear “if-then” rules which are critical for regulated environments like finance, insurance, and healthcare.

---

### 🚧 Challenges Encountered

- **Overfitting**: Initial trees had high training accuracy but poor test generalization, requiring pruning and hyperparameter tuning.
- **Class Imbalance Sensitivity**: Balancing precision and recall was essential in the face of mildly imbalanced data.
- **Visual Complexity**: As trees grew deeper, their interpretability declined—requiring selective pruning.

---
