# 📚 Multi-label Text Classification with Classifier Chains and Genetic Algorithm

This project explores and compares **multi-label classification** techniques using traditional **Classifier Chains** and an approach based on **Genetic Algorithms** to optimize the label order.

## 🚀 Objective

To investigate whether optimizing the label order in Classifier Chains using Genetic Algorithms can improve performance in text classification tasks.

## 🛠️ Technologies Used

* Python 3.x
* [Pandas](https://pandas.pydata.org/)
* [NumPy](https://numpy.org/)
* [scikit-learn](https://scikit-learn.org/stable/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [tqdm](https://tqdm.github.io/)

## 📁 Data Structure

The data should be organized in the following structure:

```
/data
  ├── train.csv
  └── test.csv

```

Each CSV must contain at least the following columns:

* `TITLE` — title of the text
* `ABSTRACT` — abstract or body of the text
* And the **label** columns (targets).

**Note**: The `ID` column, if it exists, will be dropped.

## 🧩 Steps

1. **Data Preprocessing**
* Removal of unnecessary columns
* Filling missing values
* Text vectorization using **TF-IDF**


2. **Modeling**
* Standard **Classifier Chain** using logistic regression
* **Genetic Algorithm** to optimize the label order in the chain


3. **Evaluation**
* Metrics used: F1-Score, Precision, Recall
* Multi-label confusion matrices



## 📈 Expected Results

Comparisons between:

* Classifier Chain with natural label order
* Classifier Chain with label order optimized via Genetic Algorithm
