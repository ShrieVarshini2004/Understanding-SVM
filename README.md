# 🔥 SVM Kernel Comparison: Linear vs. RBF vs. Polynomial vs. Sigmoid

## 📌 Introduction
This project demonstrates **Support Vector Machine (SVM) classification** using **four different kernel functions**:
- **Linear Kernel**
- **Radial Basis Function (RBF) Kernel**
- **Polynomial Kernel**
- **Sigmoid Kernel**

We compare their performance using **Confusion Matrices, F1-scores, and Jaccard Scores** to determine the best kernel for different datasets.

---

## 📖 Table of Contents
- [📌 Introduction](#-introduction)
- [⚙️ Technologies Used](#️-technologies-used)
- [📂 Dataset](#-dataset)
- [📊 Understanding SVM Kernels](#-understanding-svm-kernels)
- [🚀 How to Run the Code](#-how-to-run-the-code)
- [📈 Evaluation Metrics](#-evaluation-metrics)
- [📊 Results & Comparisons](#-results--comparisons)
- [🎯 Conclusion](#-conclusion)
- [🤝 Contributing](#-contributing)

---

## ⚙️ Technologies Used
- Python 🐍
- Pandas 🏗
- NumPy 🔢
- Scikit-learn 🤖
- Matplotlib 📊
- Google Colab (for running the notebook) 📝

---

## 📂 Dataset
We use the **Breast Cancer Cell Sample dataset**, where:
- **Class 2** → Benign (non-cancerous)
- **Class 4** → Malignant (cancerous)

Each cell is described using **9 features**, including `Clump Thickness`, `Uniformity of Cell Size`, and `Bare Nuclei`.

---

## 📊 Understanding SVM Kernels
| Kernel Type  | Best For | Pros | Cons |
|-------------|----------|------|------|
| **Linear Kernel** | Linearly separable data | Fast & simple | Cannot handle non-linear data |
| **RBF Kernel** | Complex non-linear data | High accuracy | Slower computation |
| **Polynomial Kernel** | Slightly curved decision boundaries | Flexible | Risk of overfitting |
| **Sigmoid Kernel** | Neural network-like decision boundaries | Unique transformation | Unstable & hard to tune |

---

## 🚀 How to Run the Code
1️⃣ **Clone this repository**  

2️⃣ Install dependencies

3️⃣ Run the Jupyter Notebook or Python script

---

##📈 **Evaluation Metrics**
We evaluate each kernel using:

Confusion Matrix 

Classification Report 📄 (Precision, Recall, F1-score)

F1-score 📊 (Higher is better)

Jaccard Score 📈 (Higher is better)

---

##📊 **Results & Comparisons**

Kernel	F1-score	Jaccard Score	Performance

Linear Kernel	Good	Moderate	Best for linearly separable data

RBF Kernel	Highest	Highest	Best for complex, non-linear data

Polynomial Kernel	Moderate	Moderate	Can overfit with high degree

Sigmoid Kernel	Lowest	Lowest	Often unstable, not recommended

🟢 RBF Kernel performs the best on non-linear data.

🟡 Linear Kernel is great when the data is already separable.

🔴 Sigmoid Kernel is the weakest without fine-tuning.

---

##🎯 **Conclusion**

If the data is linearly separable → Use a Linear Kernel.
If the data is non-linearly separable → Use RBF Kernel.
If you suspect curved separation → Try Polynomial Kernel.
Avoid Sigmoid Kernel unless well-tuned.
📌 Key Takeaway: If Linear and RBF perform similarly, then the data is linearly separable, and using Linear Kernel is the faster choice
