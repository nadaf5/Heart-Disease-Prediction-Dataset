# Heart-Disease-Prediction-Dataset
This project uses the Heart Disease Dataset to predict heart disease and explore patterns with Logistic Regression, Naive Bayes, K-Means, and PCA for visualization.

## Project Overview
This project analyzes the **Heart Disease Dataset** from Kaggle to predict the presence of heart disease and explore patterns in the data. The analysis uses **supervised learning** (Logistic Regression, Naive Bayes) and **unsupervised learning** (K-Means clustering) along with **dimensionality reduction (PCA)** for visualization and pattern discovery.

---

## Short Description
Predict and analyze heart disease using clinical features. Applies supervised and unsupervised learning techniques with PCA for visualization and insights.

---

## Dataset Description
- **Number of rows:** 1025  
- **Number of columns:** 14  

### Features
| Feature | Description |
|---------|-------------|
| age     | Age of patient |
| sex     | Gender |
| cp      | Chest pain type |
| trestbps | Resting blood pressure |
| chol    | Serum cholesterol |
| fbs     | Fasting blood sugar |
| restecg | Resting electrocardiographic results |
| thalach | Maximum heart rate achieved |
| exang   | Exercise-induced angina |
| oldpeak | ST depression induced by exercise |
| slope   | Slope of the peak exercise ST segment |
| ca      | Number of major vessels colored by fluoroscopy |
| thal    | Thalassemia type |
| target  | Heart disease: 0 = no, 1 = yes |

- **Data types:** 13 integers, 1 float (`oldpeak`)  
- **Clean data:** No missing or duplicate values

---

## Data Preparation
1. Features (`X`) and target (`y`) separated  
2. Train-test split: 80% training, 20% testing  
3. Feature scaling using `StandardScaler` for better model performance

---

## Supervised Learning

### Logistic Regression
- Trained on scaled features  
- Feature importance visualized using model coefficients  
- Accuracy: ~**80%**  
- Important features indicate key heart disease risk factors

### Naive Bayes
- Gaussian Naive Bayes trained on scaled data  
- Accuracy: **80%**  
- Classification report shows balanced precision and recall  
- Confusion matrix shows distribution of predictions

### Correlation Heatmap
- Visualized relationships between features using a heatmap  

---

## Unsupervised Learning

### K-Means Clustering
- Applied to scaled features  
- Number of clusters (`k`) = 2  
- Cluster counts and contingency table vs. `target`:

## Visualizations

![Logistic Regression Feature Importance](images/Logistic_Regression_Feature_Importance.png)  
*Logistic Regression Feature Importance*

---

![Feature Correlation Heatmap](images/Feature_Correlation_Heatmap.png)  
*Feature Correlation Heatmap*

---

![K-Means Clustering 2D PCA](images/KMeans_Clustering_2D_PCA.png)  
*K-Means Clustering 2D PCA*

---

![PCA Projection of Heart Disease Data](images/PCA_Projection_of_Heart_Disease_Data.png)  
*PCA Projection of Heart Disease Data*
