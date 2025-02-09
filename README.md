# Olympic-Medals-Prediction
# 🏅 Olympic Medals Prediction  

This project analyzes Olympic team data and builds a **machine learning model** to predict the number of medals won. It involves **data preprocessing, exploratory data analysis (EDA), and regression modeling** to make accurate predictions.  

---

## 📌 Project Overview  

The goal of this project is to explore historical Olympic data and identify key factors that influence a country’s medal count. By leveraging **linear regression**, we predict the number of medals based on the number of athletes and previous medal wins.  

---

## 📂 Dataset  

The dataset `teams.csv` contains the following columns:  

| Column        | Description |
|--------------|-------------|
| `team`       | Name of the team |
| `country`    | Country name |
| `year`       | Year of participation |
| `athletes`   | Number of athletes in the team |
| `age`        | Average age of athletes |
| `prev_medals` | Medals won in previous years |
| `medals`     | Medals won in the current year (target variable) |

---

## 🔍 Exploratory Data Analysis (EDA)  

Before building the model, we analyze the dataset using **Pandas** and **Seaborn** to uncover key patterns.  

### 📊 Correlation Matrix  
- We measure how strongly each feature correlates with `medals`.  
- The most influential features are **athletes** and **prev_medals**.  

### 📉 Scatter Plots  
- **Athletes vs Medals**: More athletes generally lead to more medals.  
- **Previous Medals vs Medals**: Teams with a history of winning tend to continue their success.  
- **Age vs Medals**: Shows a weak correlation compared to other features.  

### 📌 Histogram  
- A histogram of `medals` shows that most teams win **fewer medals**, with a few outliers winning **many medals**.  

### 🚨 Handling Missing Data  
- We identify missing values and remove rows with incomplete data.  

---

## 🏗️ Model Training  

The project uses **Linear Regression** from `Scikit-Learn` to predict the medal count.  

### 🎯 Features Used  
- **Athletes**  
- **Previous Medals**  

### 🏋️‍♂️ Training & Testing Split  
The dataset is divided into:  
- **Training Set** (`year < 2012`)  
- **Test Set** (`year ≥ 2012`)  

The model is trained using the training set and evaluated on the test set.  

---

## 📈 Model Evaluation  

### ✅ Predictions  
- The model predicts medals for the test dataset.  
- Negative predictions are set to zero.  

### 📉 Mean Absolute Error (MAE)  
- **MAE** calculates the average difference between actual and predicted medals.  
- A lower MAE means better predictions.  

---

## 🛠️ Technologies Used  

- **Python** 🐍  
- **Pandas** 📊  
- **Seaborn** 🎨  
- **Scikit-Learn** 🤖  

---

## 🚀 How to Run  

### 1️⃣ Install Dependencies  
```bash
pip install pandas seaborn scikit-learn
```

### 2️⃣ Run the Script  
```bash
python main.py
```

---

## 🔍 Key Takeaways  

✔️ More athletes generally lead to more medals.  
✔️ Previous medal counts are strong indicators of future success.  
✔️ Linear regression provides a simple yet effective model for medal prediction.  

---

## 📌 Future Improvements  

🔹 Use advanced models like **Random Forest** or **XGBoost** for better accuracy.  
🔹 Include additional features like **GDP, training facilities, and government funding**.  
🔹 Improve data cleaning and handle **outliers** more effectively.  

---

## 💡 Conclusion  

This project demonstrates how **machine learning** can predict Olympic medals using simple yet effective techniques. It highlights the importance of **EDA, feature selection, and model evaluation** in building accurate predictions.  

---

