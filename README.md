# Netflix Content Classification

### Project Overview

This project focuses on building a machine learning model to automatically classify Netflix content as either a movie or a TV show. By analyzing a dataset of Netflix titles, we developed a robust classification model for the fictional "Streamlytics" platform. This solution can be used to improve content organization, enhance user experience through better filtering, and provide valuable insights for content strategy.

### Methodology

The project followed a standard data science pipeline:

- **Data Cleaning and Preprocessing:** Handled missing values, converted data types, and cleaned the textual data in the `description` column.
- **Exploratory Data Analysis (EDA):** Discovered key insights into the distribution of content types, genres, ratings, and release years. A significant class imbalance was identified, with movies being the dominant content type.
- **Feature Engineering:** Text data was vectorized using TF-IDF, and dimensionality reduction was applied using PCA. Other categorical features like `rating` and `country` were encoded.
- **Handling Imbalance:** The SMOTE (Synthetic Minority Over-sampling Technique) algorithm was used to balance the training data, ensuring the model could effectively learn from the minority class (TV Shows).
- **Modeling:** We trained and tuned several classification models, including Logistic Regression, Random Forest, and Gradient Boosting.
- **Evaluation:** Model performance was evaluated using a comprehensive set of metrics including Accuracy, Precision, Recall, and F1-Score, with a specific focus on the minority class.

### Results and Key Findings

The **Tuned Random Forest Classifier** emerged as the best-performing model, achieving exceptional results:

| Metric                | Score (TV Shows) |
|-----------------------|------------------|
| **Precision** | 0.99             |
| **Recall** | 1.00             |
| **F1-Score** | 1.00             |
| **Overall Accuracy** | 0.997            |

The high precision and recall for the minority class (TV Shows) are particularly significant, demonstrating the model's ability to reliably identify all TV show content without misclassifying movies. This makes the model highly suitable for deployment in a production environment.

### Conclusion

This project successfully demonstrates the application of machine learning to a practical business problem. The developed model is a powerful tool for Streamlytics, capable of automating content categorization, enhancing user experience through accurate filters, and providing data-driven insights for content acquisition. The project showcases skills in data preprocessing, handling class imbalance, model tuning, and performance evaluation, making it a valuable addition to a data science portfolio.

### Technologies Used

-   Python
-   Pandas
-   Scikit-learn
-   Numpy
-   Matplotlib
-   Seaborn
