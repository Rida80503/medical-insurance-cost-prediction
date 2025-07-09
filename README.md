# medical-insurance-cost-prediction
 ML project to predict medical insurance charges after handling missing values and outliers.
 # 🏥 Medical Insurance Cost Prediction

This project predicts medical insurance charges based on patient attributes like age, BMI, smoking status, and region using regression models. The focus is on data preprocessing, including handling missing values, outlier detection, and feature encoding.

## 📌 Problem Statement

Medical insurance companies need to estimate insurance charges for individuals based on their health and demographic data. This project builds a machine learning model to predict those charges accurately.

---

## 📊 Dataset

- **Source:** [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Features:**
  - `age`: Age of primary beneficiary
  - `sex`: Gender of the person (male/female)
  - `bmi`: Body Mass Index
  - `children`: Number of dependents
  - `smoker`: Smoker or not (yes/no)
  - `region`: Residential region (northeast, southeast, etc.)
  - `charges`: Final medical insurance cost (target)

---

## ⚙️ Tools and Libraries

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

---

## 🔍 Key Steps

1. **Data Cleaning**  
   - Simulated missing values in `bmi` column and filled using mean
   - Verified no nulls in dataset

2. **Outlier Detection and Removal**  
   - Detected outliers in `charges` using boxplot and IQR method
   - Removed extreme charge values

3. **Encoding**  
   - Label encoded categorical features: `sex`, `smoker`, and `region`

4. **Modeling**  
   - Used **Linear Regression** to build the prediction model
   - Split data into training and test sets (80/20)

5. **Evaluation**  
   - **R² Score:** ~0.76  
   - **RMSE:** Around 5800  
   - Visualized feature coefficients to interpret model influence

---

## 📈 Result Highlights

- Smoking status and BMI are the most influential predictors of medical costs.
- Achieved reasonably high accuracy for a linear model.

---

## 📁 How to Run

1. Clone the repo or open the Colab notebook:
   ```bash
   git clone https://github.com/yourusername/medical-insurance-cost-prediction.git

