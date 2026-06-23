# 💊 Drug Prescription Prediction using Decision Trees

A machine learning project that predicts the most suitable drug for a patient based on their medical profile, using a Decision Tree Classifier built with Python and scikit-learn.

---

## 📌 Problem Statement

Given a dataset of 200 patients who all suffered from the same illness, the goal is to build a model that can predict which of 5 drugs (Drug A, Drug B, Drug C, Drug X, or Drug Y) a new patient should be prescribed — based on their age, sex, blood pressure, cholesterol level, and sodium-to-potassium ratio.

---

## 📊 Dataset

- **Source:** IBM Cognitive Class (drug200.csv)
- **Size:** 200 patient records
- **Features:**

| Feature | Description |
|---|---|
| `Age` | Age of the patient |
| `Sex` | Male or Female |
| `BP` | Blood Pressure level (LOW / NORMAL / HIGH) |
| `Cholesterol` | Cholesterol level (NORMAL / HIGH) |
| `Na_to_K` | Sodium-to-Potassium ratio in blood |

- **Target Variable:** `Drug` — one of Drug A, B, C, X, or Y

---

## 🧠 Approach

1. **Data Loading** — Load the CSV dataset using pandas
2. **Pre-processing** — Encode categorical variables (Sex, BP, Cholesterol) into numeric values using `LabelEncoder`
3. **Train-Test Split** — 70% training / 30% testing
4. **Model Training** — Fit a `DecisionTreeClassifier` with entropy criterion and max depth of 4
5. **Prediction** — Predict drug labels on the test set
6. **Evaluation** — Measure accuracy using `accuracy_score`

---

## 🛠️ Tech Stack

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/souravvrc/drug-prediction-ml-project.git
cd drug-prediction-decision-tree
```

### 2. Install dependencies
```bash
pip install numpy pandas scikit-learn matplotlib
```

### 3. Run the notebook
Open `DecisionTrees.ipynb` in Jupyter Notebook or Google Colab and run all cells.


---

## 📈 Results

The Decision Tree model achieves high accuracy on the test set, demonstrating that patient attributes like Na_to_K ratio and blood pressure are strong indicators of drug response.

---

## 💡 Key Concepts Covered

- Decision Tree Classification
- Label Encoding for categorical data
- Train-Test Split
- Model Evaluation with Accuracy Score
- Entropy as splitting criterion

---

## 📁 Project Structure

```
├── DecisionTrees.ipynb    # Main notebook with full code and explanations
├── drug200.csv            # Dataset (auto-downloaded in notebook)
└── README.md              # Project documentation
```

---

## 🙋 Author

**Sourav**  
Electronics & Computer Engineering | KJ Somaiya College of Engineering  
[GitHub](https://github.com/souravvrc) • [Portfolio](https://souravportfolio-nine.vercel.app)
