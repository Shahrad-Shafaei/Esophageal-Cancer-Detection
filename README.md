# Esophageal-Cancer-Detection

Ref: 
- https://www.kaggle.com/search?q=Esophageal_Dataset.csv
- https://www.kaggle.com/code/nirmalgaud/esophageal-cancer-detection/input
- https://www.kaggle.com/datasets/abhinaba1biswas/esophageal-cancer-dataset/code


Data Cleaning & Preparation 
- Filtered out features with over 50% missing values and dropped unnecessary columns to refine our dataset. 
- Handled remaining missing values with targeted imputions—using mode for categorical features and mean for continuous.

Feature Engineering & Classification 
- Classified features as categorical, continuous, or discrete for structured handling. 
- Applied chi-square tests to identify high-impact categorical features, giving us a clearer view of predictors.

Exploratory Data Analysis (EDA) 
- Leveraged histograms, box plots, and count plots to explore distributions and identify patterns in cancer progression. 
- Created pivot tables for demographics and disease status to uncover trends across gender, race, and age in esophageal cancer outcomes.

Data Visualization for Deeper Insights 
- Built correlation heatmaps to study relationships among continuous features, highlighting predictors and feature interactions. 
- Used distribution plots to analyze differences in patient habits, cancer stages, and survival metrics.

Model Testing & Results 
After data preparation, I tested several algorithms to identify the best-performing model for cancer detection:
- Logistic Regression
 - Accuracy: 64.87%
 - Confusion Matrix: [[60, 4, 3], [84, 292, 71], [46, 72, 165]]
 - Classification Report: Precision - 32% (Class 0), 79% (Class 1), 69% (Class 2); Recall - 90% (Class 0), 65% (Class 1), 58% (Class 2)
- Decision Tree Classifier
 - Accuracy: 99.75%
 - Confusion Matrix: [[66, 1, 0], [0, 446, 1], [0, 0, 283]]
 - Classification Report: Perfect precision, recall, and F1-scores across all classes
