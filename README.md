
---

# **FIFA 22 Player Ratings Prediction**

This project uses machine learning to predict FIFA 22 player ratings based on player attributes. By analyzing the dataset and applying regression models, we aim to develop an accurate predictive model and identify key features that influence player ratings.  

---

## **Project Overview**
The goal of this project is to predict FIFA player ratings using attributes such as "Reactions," "Composure," and "Shot Power." This is a regression problem where we evaluated various machine learning models to identify the best-performing one and optimize its performance.  

Key highlights include:
- Cleaning and preprocessing the data.
- Evaluating multiple regression models.
- Optimizing the Random Forest model using hyperparameter tuning.  
- Interpreting results to provide meaningful insights into player performance.

---

## **Dataset**
- **Source:** FIFA 22 player data containing 16,501 entries and 65 features.
- **Features Include:** Player attributes like "Pace," "Shooting," "Passing," and metadata such as nationality and club.
- **Target Variable:** Overall player rating.

### **Data Preprocessing**
1. Removed irrelevant features (e.g., Player IDs, Photos, and Current Club).  
2. Addressed missing values by dropping sparse columns (e.g., "Marking") and rows with missing data.  
3. Final cleaned dataset size: **15,612 entries**.  
4. Split data into training (70%) and testing (30%) sets, with `shuffle=True` for randomness.

---

## **Models and Evaluation**
Three regression models were tested:
- **Linear Regression**
- **Decision Tree**
- **Random Forest** (performed best)

### **Evaluation Metrics**
- **Root Mean Squared Error (RMSE):** Measures error magnitude.  
- **R² (Coefficient of Determination):** Indicates how well the model explains variance.  
- **Mean Absolute Error (MAE):** Shows average prediction error.

### **Best Model**
- **Random Forest** with an R² of **0.96** and RMSE of **1.26**.

---

## **Optimization**
Hyperparameter tuning using **GridSearchCV**:
- Tuned parameters:  
  - `n_estimators` (number of trees)  
  - `max_features` (number of features considered at each split)
- **Final Configuration:**  
  - 30 trees  
  - Maximum of 8 features  
- Achieved improved performance and accuracy.

---

## **Results**
- The model's predictions closely matched actual player ratings, validating its accuracy.
- Example:
  - Actual Rating: 69 → Predicted Rating: 69.63
  - Actual Rating: 75 → Predicted Rating: 75.73  

---

## **Installation and Usage**
### **Requirements**
- Python 3.7 or higher  
- Libraries:  
  - `pandas`  
  - `numpy`  
  - `matplotlib`  
  - `seaborn`  
  - `scikit-learn`  

### **How to Run**
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/fifa22-ratings-prediction.git
   cd fifa22-ratings-prediction
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook or Python script:  
   ```bash
   jupyter notebook fifa22_prediction.ipynb
   ```

---

## **Project Structure**
```
📁 fifa22-ratings-prediction  
├── 📂 data  
│   └── fifa22.csv  
├── 📂 notebooks  
│   └── fifa22_prediction.ipynb  
├── 📂 outputs  
│   └── screenshots/  
├── 📂 models  
│   └── random_forest.pkl  
├── README.md  
├── requirements.txt  
└── LICENSE  
```

---

## **Conclusion**
This project demonstrates the power of machine learning in sports analytics. By using a Random Forest model, we achieved highly accurate predictions of FIFA 22 player ratings. The process also highlights the importance of data preprocessing, model evaluation, and hyperparameter tuning.

---

## **Contact**
Feel free to connect if you have any questions or want to collaborate on similar projects!  
- **Name:** Ali Ebrahim Monir Sakr  
- **Email:** alimonirsakr@gmail.com  
- **LinkedIn:** [Ali Monir Sakr](https://www.linkedin.com/in/ali-monir-sakr)  

---

