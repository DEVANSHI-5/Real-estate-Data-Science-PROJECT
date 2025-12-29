# 🏠 Real Estate Price Prediction

## 🎯 Objective
Build a machine learning model to **predict house price per unit area** using real-estate features such as house age, MRT distance, and location.

---

## 📊 Dataset
- **414 rows × 8 columns**
- Key features:
  - House age  
  - Distance to nearest MRT station  
  - Latitude & longitude  
  - Transaction date  
- **Target:** `Y house price of unit area`

---

## 🧠 Approach (Steps)
1. Loaded and inspected the dataset using Pandas  
2. Removed the `X4 number of convenience stores` column  
3. Checked for missing values (none found)  
4. Engineered features  
   - Rounded house age → `Age`  
   - Created `DISTFROMMRT` and `LONGITUDE`
5. Performed EDA using correlation heatmaps and pairplots  
6. Split the data into train and test sets  
7. Trained a **Linear Regression model**  
8. Evaluated performance and ran cross-validation  

---

## 🛠 Tech Stack
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-Learn  

---

## 📈 Results
- **R² Score on Test Set:** ~ **0.70**
- **Cross-validation scores:** ~ **0.41 – 0.62**
- Key insights:
  - **Closer to MRT → Higher price**
  - **Location (latitude & longitude) is highly influential**
  - **Older houses generally cost less**

---

## ✅ Conclusion
- Linear Regression predicts real-estate price per unit area with **~70% accuracy**
- **Location and MRT accessibility are the strongest price drivers**
- Feature engineering improved model interpretability

---

## 🚀 Future Improvements
- Try Ridge / Lasso / Tree-based models  
- Hyperparameter tuning  
- Build a Streamlit / Flask web app for live predictions  

---

📌 *Built for learning and showcasing machine learning workflow on real estate data.*

