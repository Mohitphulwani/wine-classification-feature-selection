# wine-classification-feature-selection
Feature selection and classification on the Wine dataset using a custom Sequential Forward Selection (SFS) implementation with K-Nearest Neighbors.
# Wine Classification with Feature Selection

## Project Overview
This project demonstrates **feature selection using Sequential Forward Selection (SFS)** on the Wine dataset and applies a **K-Nearest Neighbors (KNN) classifier** to classify wines into different categories.  

By selecting the most relevant features, the project aims to:
- Improve model performance
- Reduce computational complexity
- Highlight important chemical properties of wine for classification

---

## Objectives
- Implement a **custom SFS algorithm** to select optimal features.
- Apply the SFS-selected features to a **KNN classifier**.
- Evaluate classification performance on the Wine dataset.
- Visualize the improvement of validation accuracy as features are added.

---

## Methodology

### 1. Data Loading
- Wine dataset from `sklearn.datasets`  
- Split into training (70%) and testing (30%) sets  
- Standardized using `StandardScaler` for proper scaling

### 2. Feature Selection
- Implemented **Sequential Forward Selection (SFS)**:
  - Starts with an empty set of features.
  - Iteratively adds features that improve validation accuracy.
  - Stops when the desired number of features is reached.
- Selected top **4 features** for classification.

### 3. Model Building
- **Classifier**: K-Nearest Neighbors (`n_neighbors=3`)
- Trained on selected features from SFS.
- Performance evaluated using **validation accuracy**.

### 4. Results
- Selected Features:
  ```text
  [list of selected features]

