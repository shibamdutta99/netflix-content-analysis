# 🎬 Netflix Content Classification

## 📌 Project Overview
This project builds a **machine learning model** to classify Netflix content as either a **Movie** or a **TV Show**.  
By analyzing a dataset of Netflix titles, we created a robust classifier for the fictional **"Streamlytics"** platform — improving content organization, enhancing user filtering, and providing insights for content strategy.

---

## 🔍 Methodology
We followed a standard **Data Science Pipeline**:

1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Converted data types
   - Cleaned `description` column text

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of content types, genres, ratings, release years
   - Identified significant **class imbalance** (movies dominate dataset)

3. **Feature Engineering**
   - Vectorized text using **TF-IDF**
   - Reduced dimensionality with **PCA**
   - Encoded categorical features (`rating`, `country`)

4. **Handling Class Imbalance**
   - Used **SMOTE** to oversample TV Shows for balanced training

5. **Modeling**
   - Trained Logistic Regression, Random Forest, Gradient Boosting
   - Hyperparameter tuning for optimal performance

6. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-Score
   - Focus on performance for minority class (TV Shows)

---

## 🏆 Results
**Tuned Random Forest Classifier** delivered outstanding performance:

| Metric (TV Shows)   | Score |
|---------------------|-------|
| Precision           | 0.99  |
| Recall              | 1.00  |
| F1-Score            | 1.00  |
| **Overall Accuracy**| 0.997 |

✅ **High precision & recall** for TV Shows → minimal misclassification and reliable detection.

---

## 📌 Conclusion
- **Business Impact:** Automates Netflix content categorization for **Streamlytics**  
- **User Experience:** More accurate filters for movies/TV shows  
- **Data-Driven Decisions:** Supports acquisition & strategy with reliable classifications

---

## ⚙️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📂 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/shibamdutta99/netflix-content-analysis.git
   cd netflix-content-analysis
