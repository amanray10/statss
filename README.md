# Statistics for ML & Data Science – Lab Experiments

Experiments **1, 2, 3, 4, 6, 8 and 9** on three datasets: **Iris**, **Titanic** and **House Price (California Housing)**.
There is one folder per experiment and **one notebook per dataset**. Every notebook has already been run, so all outputs and plots are visible on GitHub and in VS Code.

| # | Experiment | Iris | Titanic | House Price |
|---|---|---|---|---|
| 1 | Exploratory Data Analysis | [Iris](Exp1_EDA/Exp1_EDA_Iris.ipynb) | [Titanic](Exp1_EDA/Exp1_EDA_Titanic.ipynb) | [House Price](Exp1_EDA/Exp1_EDA_HousePrice.ipynb) |
| 2 | Data Preprocessing | [Iris](Exp2_Data_Preprocessing/Exp2_Preprocessing_Iris.ipynb) | [Titanic](Exp2_Data_Preprocessing/Exp2_Preprocessing_Titanic.ipynb) | [House Price](Exp2_Data_Preprocessing/Exp2_Preprocessing_HousePrice.ipynb) |
| 3 | Sampling Methods | [Iris](Exp3_Sampling_Methods/Exp3_Sampling_Iris.ipynb) | [Titanic](Exp3_Sampling_Methods/Exp3_Sampling_Titanic.ipynb) | [House Price](Exp3_Sampling_Methods/Exp3_Sampling_HousePrice.ipynb) |
| 4 | Hypothesis Testing (t, z, Chi-square, ANOVA, Tukey) | [Iris](Exp4_Hypothesis_Testing/Exp4_Hypothesis_Testing_Iris.ipynb) | [Titanic](Exp4_Hypothesis_Testing/Exp4_Hypothesis_Testing_Titanic.ipynb) | [House Price](Exp4_Hypothesis_Testing/Exp4_Hypothesis_Testing_HousePrice.ipynb) |
| 6 | Linear Regression and Diagnostics (VIF, residuals, Cook's distance) | [Iris](Exp6_Linear_Regression_Diagnostics/Exp6_Linear_Regression_Iris.ipynb) | [Titanic](Exp6_Linear_Regression_Diagnostics/Exp6_Linear_Regression_Titanic.ipynb) | [House Price](Exp6_Linear_Regression_Diagnostics/Exp6_Linear_Regression_HousePrice.ipynb) |
| 8 | Classification (Logistic, KNN, Naive Bayes, ROC) | [Iris](Exp8_Classification_Models/Exp8_Classification_Iris.ipynb) | [Titanic](Exp8_Classification_Models/Exp8_Classification_Titanic.ipynb) | [House Price](Exp8_Classification_Models/Exp8_Classification_HousePrice.ipynb) |
| 9 | Decision Trees and Random Forest | [Iris](Exp9_Decision_Tree_Random_Forest/Exp9_DecisionTree_RandomForest_Iris.ipynb) | [Titanic](Exp9_Decision_Tree_Random_Forest/Exp9_DecisionTree_RandomForest_Titanic.ipynb) | [House Price](Exp9_Decision_Tree_Random_Forest/Exp9_DecisionTree_RandomForest_HousePrice.ipynb) |

## Datasets (CSV files on the computer)

| Dataset | File name | Source | Rows |
|---|---|---|---|
| Iris | `Iris.csv` | Kaggle [uciml/iris](https://www.kaggle.com/datasets/uciml/iris) | 150 |
| Titanic | `train.csv` | Kaggle [Titanic competition](https://www.kaggle.com/competitions/titanic/data) | 891 |
| House Price | `housing.csv` | Kaggle [camnugent/california-housing-prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices) | 20,640 |

Every notebook loads its file with one line, for example:

```python
df = pd.read_csv("train.csv")
```

The CSV must be in the **same folder as the notebook**. If the file is somewhere else on the computer, write its full path instead:

```python
df = pd.read_csv(r"C:\Users\Lab\Desktop\train.csv")
```

## Running in VS Code
1. Install **Python** and, in VS Code, the **Python** and **Jupyter** extensions.
2. Install the libraries (once): `pip install -r requirements.txt`
3. Open a notebook, choose the Python kernel (top right), then press **Run All**.

The outputs are already saved in every notebook, so you can read the results without running anything.

## Notes
- Experiments 8 and 9 are binary classification: Iris uses **Versicolor vs Virginica**, and House Price uses **expensive vs not expensive** (value above / below the median).
- Each notebook saves its result tables as CSV files (e.g. `clean.csv`, `hypothesis.csv`) in the notebook's folder.
- Each notebook ends with a **Result / Conclusion** cell.

## Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`, `scikit-learn` (see `requirements.txt`).
