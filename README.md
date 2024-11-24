
---

# Employee Retention Prediction using Decision Tree Classifier

## Overview
This project implements a Decision Tree Classifier to predict whether an employee will leave the organization (`LeaveOrNot`) based on their attributes. The dataset is preprocessed using Label Encoding, and the model's performance is evaluated using a train-test split. The decision tree is visualized to better understand the decision-making process.

---

## Dataset
The dataset (`Employee.csv`) includes the following columns:

| Column Name       | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `Education`        | Educational level of the employee.                                         |
| `JoiningYear`      | Year the employee joined the organization.                                 |
| `City`             | Location where the employee is based.                                      |
| `Gender`           | Gender of the employee.                                                   |
| `EverBenched`      | Indicates whether the employee was ever benched (not assigned work).       |
| `LeaveOrNot`       | Target variable: 1 if the employee left the organization, 0 otherwise.     |

---

## Steps Followed
### 1. **Data Preprocessing**
- Handled categorical variables (`Education`, `City`, `Gender`, `EverBenched`) using Label Encoding.
- Verified for missing values and ensured data integrity.
- Split the dataset into features (`inputs`) and the target variable (`LeaveOrNot`).

### 2. **Train-Test Split**
- Used `train_test_split` to divide the data into training and testing sets (80% training, 20% testing).

### 3. **Model Building**
- Built a Decision Tree Classifier using the `scikit-learn` library.
- Used "entropy" as the criterion to calculate information gain.

### 4. **Visualization**
- Visualized the Decision Tree using `matplotlib` and `plot_tree` from `scikit-learn`.

### 5. **Model Evaluation**
- Predicted the target variable on test data.
- Calculated the model's accuracy using `accuracy_score`.
- Generated a classification report and confusion matrix for detailed performance insights.

---

## Model Results
### Accuracy
The model achieved an accuracy of **X%** on the test dataset.  
*(Replace X% with your model's accuracy after execution.)*

### Decision Tree Diagram
The decision tree is visualized to understand the factors influencing employee retention decisions. See the diagram below:

![Decision Tree Diagram](DecisionTreeDiagram.png)

Alternatively, you can find the file in the repository for a closer look.

---

## Installation and Usage
### Prerequisites
Ensure the following are installed on your system:
- Python 3.x
- Jupyter Notebook
- Required Python Libraries: `pandas`, `scikit-learn`, `matplotlib`

### Steps to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Decision-Tree-Employee-Analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas scikit-learn matplotlib
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook DecisionTreeEmployee.ipynb
   ```
4. Run the notebook cells sequentially to preprocess the data, train the model, and evaluate its performance.

---

## Dependencies
The following Python libraries are used in this project:
- **pandas**: For data manipulation and preprocessing.
- **scikit-learn**: For implementing the Decision Tree Classifier and evaluation metrics.
- **matplotlib**: For visualizing the decision tree.

Install them using:
```bash
pip install pandas scikit-learn matplotlib
```

---

## File Structure
```
Decision-Tree-Employee-Analysis/
│
├── Employee.csv                 # Dataset
├── DecisionTreeEmployee.ipynb   # Jupyter Notebook
├── DecisionTreeDiagram.png      # Decision Tree Diagram
└── README.md                    # Detailed Project Description
```

---

## Future Work
- Add hyperparameter tuning for the Decision Tree Classifier.
- Explore other algorithms like Random Forest and Gradient Boosted Trees.
- Perform feature importance analysis to identify the most critical factors affecting retention.

---
