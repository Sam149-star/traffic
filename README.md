# 🚦 Smart Traffic Insights for Indian Cities

## 📌 Objective
This project builds a **mini AI-powered system** that predicts traffic levels (Low, Mid, High) using historical traffic data.  
The aim is to help **citizens, delivery services, and city officials** gain insights into traffic patterns and improve mobility in cities like **Indore**.

---

## 📊 Dataset
- Source: Kaggle Traffic Prediction Dataset (or similar traffic data).  
- Preprocessing steps:  
  - Extracted **hour** from DateTime.  
  - Created **dummy variables** for hours.  
  - Computed **quantile thresholds** to categorize traffic levels.  
  - Removed unused columns and prepared features (`X`) and target (`Y`).  

---

## 🔄 Workflow
The workflow is shown in the flowchart below:

![Flowchart](flowchart.png)

**Steps**:  
1. Start with raw data.  
2. Feature engineering: extract hour, create dummies, categorize traffic.  
3. Prepare features (X) and labels (Y).  
4. Split into **train/test sets**.  
5. Train models (Random Forest, Logistic Regression).  
6. Evaluate with **classification report** and **confusion matrix**.  

---

## 🤖 Models & Results
- **Random Forest Classifier** (tuned with RandomizedSearchCV)  
  - ✅ Test Accuracy: **100%**  
  - ✅ Perfect precision, recall, F1-score across *Low, Mid, High* categories  

- **Baseline Logistic Regression Model** also included for comparison.  

---

## 💡 Business Use Cases
- **Citizens** → Plan trips when traffic is lighter  
- **Delivery Companies** → Optimize delivery times and routes  
- **City Officials** → Monitor congestion patterns and improve infrastructure planning  

---

## 🛠️ Tech Stack
- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)  
- Jupyter Notebook / Google Colab  
- Random Forest, Logistic Regression  

---

## 📂 Repository Structure
```
smart-traffic-insights/
│
├── Welcome_To_Colab.ipynb          # Main notebook
├── traffic.csv                     # Dataset
├── final_traffic_model.pkl         # Trained Random Forest model
├── logistic_regression_model.pkl   # Baseline Logistic Regression model
├── flowchart.png                   # Workflow diagram
└── README.md                       # Project documentation
```

---

## 🎥 Demo
A short demo video (2–3 minutes) showing the workflow and predictions can be added here.  
👉 [Demo Link Placeholder]  

---

## ✨ Conclusion
This project demonstrates how **AI can provide actionable insights** into urban traffic patterns.  
The proof-of-concept can be extended into **real-time traffic prediction systems** for smart cities.
