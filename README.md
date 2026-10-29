# Power System Load Type Prediction

## Project Overview

This project focuses on predicting power system load types using machine learning classification techniques. It uses historical power consumption data and electrical measurements to classify energy demand into different load categories.

The objective is to preprocess the dataset, perform exploratory data analysis, train and compare classification models, and evaluate their performance on unseen data.

## Objectives

- Clean and preprocess the power consumption dataset.
- Perform Exploratory Data Analysis (EDA) using visualizations.
- Engineer useful time-based features from date and time information.
- Build and compare multiple machine learning classification models.
- Evaluate model performance using standard classification metrics.
- Test the selected model on the final month of available data.

## Dataset

**File:** `load_data.csv`

The dataset contains historical power consumption measurements, timestamps, electrical parameters, and the target variable `Load_Type`.

The target classes are:

- `Light_Load`
- `Medium_Load`
- `Maximum_Load`

The dataset is provided with this assignment.

## Technologies Used

- **Programming Language:** Python
- **Environment:** Jupyter Notebook
- **Data Processing:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn

## Machine Learning Models

The notebook compares the following classification models:

1. Dummy Classifier — baseline model
2. Logistic Regression
3. Decision Tree Classifier
4. Random Forest Classifier
5. Extra Trees Classifier

The best-performing model is selected based on the macro F1-score measured on the held-out test set.

## Project Workflow

1. Load the dataset.
2. Inspect and preprocess the data.
3. Handle missing values.
4. Perform exploratory data analysis.
5. Extract time-based features such as month, day, weekday, and hour.
6. Split the data chronologically, reserving the final month for testing.
7. Train and compare classification models.
8. Evaluate performance using classification metrics and a confusion matrix.
9. Analyze feature importance where supported by the selected model.

## Evaluation Metrics

The models are evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted class labels that are correct.
- **Recall:** Proportion of actual class instances correctly identified.
- **Macro F1-score:** Average F1-score across classes, giving each class equal weight.
- **Confusion Matrix:** Shows correct and incorrect predictions for each class.

## Project Structure

```text
power-system-load-prediction/
├── Power_System_Load_Type_Prediction.ipynb
├── load_data.csv
└── README.md
```

## How to Run the Project

### Prerequisites

Install Python and the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Steps

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `Power_System_Load_Type_Prediction.ipynb`.
5. Run the notebook cells sequentially.

Ensure that `load_data.csv` is in the same directory as the notebook and that the dataset path is set correctly.

## Results

The notebook generates a model comparison table containing accuracy, macro precision, macro recall, and macro F1-score. It also displays a classification report and confusion matrix for the selected model.

**Best-performing model:** To be filled in after execution.

**Test accuracy:** To be filled in after execution.

**Macro F1-score:** To be filled in after execution.

## Conclusion

This project demonstrates the application of supervised machine learning classification techniques to power system load prediction. It covers data preprocessing, exploratory analysis, feature engineering, model training, and evaluation using a chronological test split.

The results can help compare classification approaches for identifying different power demand levels. Model performance and limitations should be interpreted using the actual evaluation results produced by the notebook.

## Author

**Keerthana K.**

Machine Learning Classification Assignment
