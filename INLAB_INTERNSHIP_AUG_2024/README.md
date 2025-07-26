# Breast Cancer Prediction Using Machine Learning

This project aims to predict the presence of breast cancer using a variety of supervised ML algorithms, including hybrid model combinations. Built as part of an in-lab internship, the solution emphasizes accuracy, generalization, and interpretability.

---

## Dataset

- **Source**: UCI Machine Learning Repository
- **Features**: Tumor-related metrics
- **Preprocessing**: Feature scaling, data augmentation, multiple train-test splits

---

## Algorithms Used

- Logistic Regression (LR)
- Support Vector Machine (SVM)
- Random Forest (RF)
- Gradient Boosting (GB)
- Naive Bayes (NB)
- Decision Tree (DT)
- K-Nearest Neighbors (KNN)
- **21 hybrid model combinations** using 7C2 algorithm pairs

---

## Methodology

- Evaluated using multiple splits: 70:30 and 80:20
- Applied confusion matrix, ROC-AUC, F1 score, precision, recall
- Compared performance across models and combinations

---

## Best Results

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 98% | 0.97 | 1.00 | 0.98 |
| GB + LR | 94% | 0.94 | 0.94 | 0.95 |
| SVM + DT | 89% | 0.94 | 0.85 | 0.91 |

---

## Tools and Libraries

- Python (Google Colab)
- NumPy, Pandas, Matplotlib
- Scikit-learn

---

## Future Scope

- Introduce Deep Learning / CNNs for image-based datasets
- Integrate real-world hospital datasets
- Deploy as a web-based clinical decision support system
