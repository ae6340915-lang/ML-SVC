# Dry Bean Classification using SVC

## Project Overview

This project uses a Support Vector Classifier (SVC) to classify dry beans into seven categories based on numerical measurements of their shape and size.

The project demonstrates a complete introductory machine-learning workflow, including data exploration, duplicate removal, target encoding, feature scaling, model training, and evaluation.

## Dataset

The project uses the **Dry Bean Dataset**, stored in an Excel file named `Dry_Bean_Dataset.xlsx`.

* **Original dataset size:** 13,611 rows
* **Rows after removing duplicates:** 13,543
* **Number of columns:** 17 (16 numerical features and 1 target column)
* **Missing values:** None were found
* **Duplicate rows removed:** 68

### Target Classes

The target column is `Class`, containing seven dry bean varieties:

* BARBUNYA
* BOMBAY
* CALI
* DERMASON
* HOROZ
* SEKER
* SIRA

### Features

The dataset contains 16 numerical features:

* Area
* Perimeter
* MajorAxisLength
* MinorAxisLength
* AspectRation
* Eccentricity
* ConvexArea
* EquivDiameter
* Extent
* Solidity
* roundness
* Compactness
* ShapeFactor1
* ShapeFactor2
* ShapeFactor3
* ShapeFactor4

## Project Workflow

1. Import the required Python libraries.
2. Load the Excel dataset using pandas.
3. Explore the data using `head()`, `info()`, and `describe()`.
4. Check for missing values and duplicate rows.
5. Remove duplicate rows.
6. Explore the target classes.
7. Separate the features (`X`) from the target (`y`).
8. Split the data into training and testing sets using an 80/20 split and stratification.
9. Encode the target labels using `LabelEncoder`.
10. Scale the numerical features using `StandardScaler`.
11. Explore feature correlations using a heatmap.
12. Train and evaluate the SVC model.

**Note:** The notebook creates a separate `df_clean` DataFrame for correlation-heatmap exploration after selecting some columns to drop. However, the SVC model is trained using the scaled features from `X`, created from the duplicate-cleaned dataset. Therefore, the selected columns are not excluded from the model's training features.

## Model

The project uses `SVC` from `scikit-learn` with the following configuration:

```python
SVC(
    kernel="rbf",
    C=10,
    gamma=0.1,
    random_state=42
)
```

### Data Preparation

* **Training/testing split:** 80% training and 20% testing
* **Random state:** 42
* **Stratification:** Enabled to preserve class proportions
* **Target encoding:** `LabelEncoder`
* **Feature scaling:** `StandardScaler`

The scaler is fitted on the training features and then applied to the test features to avoid data leakage.

## Results

The notebook reports the following test-set results:

| Metric            |  Score |
| ----------------- | -----: |
| Accuracy          | 92.54% |
| Weighted F1-score | 92.54% |

### Classification Report

| Class    | Precision | Recall | F1-score | Support |
| -------- | --------: | -----: | -------: | ------: |
| BARBUNYA |      0.93 |   0.91 |     0.92 |     265 |
| BOMBAY   |      1.00 |   1.00 |     1.00 |     104 |
| CALI     |      0.92 |   0.94 |     0.93 |     326 |
| DERMASON |      0.92 |   0.93 |     0.92 |     709 |
| HOROZ    |      0.97 |   0.94 |     0.95 |     372 |
| SEKER    |      0.94 |   0.95 |     0.95 |     406 |
| SIRA     |      0.88 |   0.87 |     0.88 |     527 |

These results indicate that the model achieves good overall performance on the test dataset. Performance may vary if the dataset, preprocessing, or model settings change.

## Requirements

Install the required Python packages:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn openpyxl jupyter
```

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/ae6340915-lang/ML-SVC.git
   ```

2. Open the project folder:

   ```bash
   cd ML-SVC
   ```

3. Place `Dry_Bean_Dataset.xlsx` in the same folder as the notebook, or update the file path in the notebook.

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `9999.ipynb` and run the cells in order.

### Dataset Path

For easier sharing and reproducibility, the notebook should load the dataset using a relative path if the Excel file is stored beside the notebook:

```python
df = pd.read_excel("Dry_Bean_Dataset.xlsx")
```

If the dataset is stored in another location, replace the path with its actual location.

## Repository Contents

```text
ML-SVC/
├── 9999.ipynb
├── README.md
└── Dry_Bean_Dataset.xlsx
```

**Important:** The Excel dataset may not be included in the repository. Make sure you have the dataset file before running the notebook. Only upload and redistribute the dataset if its license permits it.

## Technologies Used

* Python
* NumPy
* pandas
* Matplotlib
* Seaborn
* scikit-learn
* Jupyter Notebook

## Author

**Abdelrahman Elsayed**

GitHub Profile: https://github.com/ae6340915-lang

Project Repository: https://github.com/ae6340915-lang/ML-SVC
