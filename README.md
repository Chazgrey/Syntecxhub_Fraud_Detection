# 🌸 Syntecxhub Fraud Detection

This project is for building a model to detect fraudulent transactions using **Random Forest** and **XGBoost** models, with **SMOTE** sampling to handle class imbalance.  
It provides interactive visualizations, performance metrics,end-to-end data analysis, model training and evaluation.

---
## 📂 Project Structure


- **Fraud_detection.ipynb** 
- **Class_Distribution_Pie_chart.png** → <img width="1800" height="1800" alt="Class_Distribution_Pie_chart" src="https://github.com/user-attachments/assets/6009f0db-7fc7-4d21-b654-fd4ee6160a53" />

- **Correlation_Heatmap.png** → <img width="3600" height="3000" alt="Correlation_Heatmap" src="https://github.com/user-attachments/assets/12d9e6f2-c43c-4f85-8c68-b15b13a28e3e" />

- **Class_Distribution.png** → <img width="1920" height="1440" alt="Class_Distribution" src="https://github.com/user-attachments/assets/662a76db-ba08-4ddd-b14b-a1272c17b22d" />


- **README.md** → Project documentation.

## 🚀 Features

- Upload dataset → EDA + class imbalance visualization
- Train Random Forest & XGBoost with SMOTE
- Interactive threshold slider for precision/recall tradeoffs
- Precision‑Recall and ROC curves
---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Chazgrey/Syntecxhub_Fraud_Detection.git
cd Syntecxhub_Fraud_Detection
```
---
## 📊 Usage
### Run Jupyter Notebook
```bash
jupyter notebook Frauddetection.ipynb
```

---
## 📈Precision vs Recall Tradeoffs

- Precision (few false positives)
- High precision means that when the model flags a transaction as fraud, it’s almost always correct.
- Business impact: fewer legitimate customers inconvenienced, better customer experience.
- Risk: lower recall → some fraud slips through, leading to financial losses.
- Recall (few false negatives)
- High recall means the model catches nearly all fraudulent transactions.
- Business impact: minimizes fraud losses.
- Risk: lower precision → more false alarms, frustrating customers and increasing manual review workload.
---
# Business Decision Thresholds
The threshold determines the probability cutoff for classifying a transaction as fraud. Adjusting it shifts the balance:
| Threshold | Precision | Recall | Business Implication | 
|-----------|-----------|--------|----------------------|
|0.3  |Lower  |Higher  |Aggressive fraud detection, more false alarms. | 
|0.5  |Balanced  |Balanced  |Default cutoff, good starting point.| 
|0.7  |Higher  |Lower  |Conservative detection, fewer false alarms but some fraud missed. | 
|0.9  |Very High  |Low  |Only flags near-certain fraud, excellent customer experience but risk of missed fraud. | 

---
## 🛠️ Technologies Used
- Python
- Scikit-learn
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook
