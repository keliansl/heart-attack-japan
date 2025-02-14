# Heart Attack Prediction in Japan

## 📌 Project Overview
This project aims to predict the risk of heart attacks in Japanese individuals. Using machine learning techniques, we analyze a dataset containing various health and lifestyle factors to determine their impact on cardiovascular diseases.

## 📊 Dataset
- **Source**: [Kaggle - Heart Attack in Japan (Youth vs Adult)](https://www.kaggle.com/datasets/ashaychoudhary/heart-attack-in-japan-youth-vs-adult)
- **Features**: The dataset includes medical indicators such as cholesterol levels, blood pressure, and alcohol consumption, among others.
- **Target Variable**: Presence or absence of heart disease.

## 🔍 Data Preprocessing
- **Feature Selection**: Removal of irrelevant columns (e.g., `Extra_Column_X`).
- **Handling Missing Data**: Null values were imputed using the most frequent class.
- **Class Imbalance**: Since the dataset was highly imbalanced (90/10 ratio before resampling), techniques such as **SMOTE** and **SMOTE-Tomek** were applied.

## 🚀 Machine Learning Models
- **Algorithms Used**:
  - Random Forest
  - LightGBM
  - XGBoost
  - Voting Classifier (planned but not implemented due to dataset restrictions)
- **Optimization**:
  - **Hyperparameter Tuning**: Performed using GridSearch.
  - **Metric Focus**: Training was optimized for **F1-score**, ensuring a balance between precision and recall.

## 📈 Results
- The best performing models were **LightGBM and XGBoost**, both trained on SMOTE-Tomek resampled data.
- The **recall achieved was around 68-69%**, meaning that approximately **68-69% of heart disease cases were correctly identified**.
- Metrics were evaluated using **cross-validation**, given that the test set was no longer accessible.

## ⚠️ Limitations
- **Dataset Unavailability**: The dataset has been set to private on Kaggle, preventing further modifications or improvements.
- **Oversampling Bias**: The cross-validation results might be optimistic since resampled data were used.

## 🔬 Future Improvements
Although further modifications are not possible due to dataset restrictions, potential improvements could include:
- **Stacking models** to enhance predictive performance.
- **Feature engineering** to extract more meaningful health indicators.
- **Exploring advanced balancing techniques** like **ADASYN** for smarter synthetic data generation.

---
### 📢 Conclusion
This project demonstrates the potential of machine learning in predicting cardiovascular diseases, emphasizing the importance of handling imbalanced data. While results are promising, access to more diverse and real-world datasets would enhance the robustness of the predictions.

