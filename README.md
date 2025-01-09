# K-Nearest-Neighbors.
# Zoo Classification Using K-Nearest Neighbors (KNN)

This project focuses on classifying animals based on their attributes using the K-Nearest Neighbors (KNN) algorithm. The dataset used is the Zoo dataset, which contains features describing various animals and their classifications.

## Dataset

The Zoo dataset contains:
- Animal features (e.g., hair, feathers, eggs, milk, etc.)
- Labels indicating the animal's name.

The target is to predict the `animal name` based on the features.

## Project Workflow

### 1. Data Exploration
- **Initial Insights**:
  - Used `.info()` and `.describe()` to understand the dataset structure and statistical summary.
  - Checked for missing values and handled them:
    - Numerical columns: Filled with the median.
    - Categorical columns: Filled with `'Unknown'`.
- **Visualization**:
  - Used `countplot` to visualize the distribution of animal types.
  - Created a correlation heatmap to analyze the relationships between numerical features.

### 2. Data Preprocessing
- Split the data into features (`X`) and target (`y`).
- Dropped the `animal name` column from the features.
- Scaled the data using `StandardScaler` for normalization.

### 3. Model Training and Evaluation
- Used the K-Nearest Neighbors (KNN) classifier with:
  - `k=5`
  - Euclidean distance as the metric.
- Metrics for evaluation:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-Score**
  - **Confusion Matrix**

### 4. Visualization
- Plotted the confusion matrix to evaluate the classifier's performance.
- Created a scatter plot of the features to visualize the data distribution.

## Requirements

Install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
