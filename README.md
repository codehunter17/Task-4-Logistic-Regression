# Task 4: Classification with Logistic Regression 🎯🔍

## 📌 Objective:
To build a binary classification model using Logistic Regression on the Breast Cancer dataset.

## 🛠️ Tools Used:
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## ✅ Steps I Followed:

### 1. Loaded the Dataset:
- Used the **Breast Cancer Wisconsin Diagnostic Dataset (data.csv)**.
- The dataset contains features like radius, texture, smoothness, compactness, etc.

### 2. Data Preprocessing:
- Dropped unnecessary columns like `id` and `Unnamed: 32`.
- Converted the target variable `diagnosis` into binary form:  
`M` → `1` (Malignant),  
`B` → `0` (Benign).
- Checked for null values.

### 3. Feature Scaling:
- Used `StandardScaler` to normalize the feature values for better model performance.

### 4. Train-Test Split:
- Split the data into **80% training set** and **20% testing set** using `train_test_split`.

### 5. Model Building:
- Trained a **Logistic Regression model** using `LogisticRegression()` from scikit-learn.

### 6. Model Evaluation:
- Evaluated model performance using:
  - **Confusion Matrix**
  - **Precision**
  - **Recall**
  - **F1-Score**
  - **ROC-AUC Score**
- Plotted the **ROC Curve** to visualize model performance.

### 7. Threshold Tuning:
- Changed the default classification threshold from 0.5 to 0.3 to see how it affects **Precision** and **Recall**.
- Observed the trade-off between False Positives and False Negatives.

---

## ✅ 8. Explanation of Sigmoid Function 🧠:

Logistic Regression uses the **Sigmoid Function** (also known as the **Logistic Function**) to convert raw linear model output into a **probability between 0 and 1**.

### 📍 Sigmoid Function Formula:

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

Where:  
- **x** = Linear combination of input features  
- **σ(x)** = Probability between 0 and 1

### 📍 Why Sigmoid?

- Logistic Regression needs probability outputs for binary classification.
- The **Sigmoid function "squashes" the output** to always stay between **0 and 1**.
- This allows us to interpret the output as the **probability of the positive class (class = 1)**.

### 📍 Example:

- If the sigmoid output = **0.85**, it means the model predicts **85% chance of being Malignant (class 1)**.
- If output = **0.25**, it means **25% chance of being Malignant**, i.e., likely Benign (class 0).

### 📍 Sigmoid Curve Shape:
- The curve is **S-shaped**, starting near 0, rising in the middle (around x=0), and flattening near 1.

---

## ✅ 📷 Screenshots:
*(Optional - Add screenshots of your confusion matrix, ROC curve, classification report if you took any)*

---

## ✅ ✅ Conclusion:
This task helped me learn the complete flow of building a **binary classification model using Logistic Regression**, starting from data preprocessing to evaluation metrics like ROC-AUC, and understanding the math behind the sigmoid function.

---

**Done by:** Krishna Kant 😊
