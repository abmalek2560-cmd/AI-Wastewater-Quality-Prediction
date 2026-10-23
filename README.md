
# 🌊 AI-Driven Wastewater Treatment Plant Quality Prediction & Anomaly Detection

## 📌 Project Overview
This hands-on data science project is inspired by research on autonomous AI and optimization frameworks for Water Resource Recovery Facilities (WRRFs), specifically influenced by the research directions of Prof. **SungKu Heo** at the [Greenest A.I. Lab](https://greenest-ai.kangwon.ac.kr/). 

The project utilizes machine learning models to predict treated effluent water quality from inlet sensor parameters and implements an automated anomaly detection system to flag critical operational risks or performance failures in wastewater treatment plants (WWTP).

---

## 📂 Dataset Source & References
* **Dataset Name:** Water Treatment Plant Dataset
* **Source / Repository:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
* **Direct Data Link:** [UCI Water Treatment Data](https://archive.ics.uci.edu/ml/machine-learning-databases/water-treatment/water-treatment.data)
* **Description:** The dataset contains daily sensor measurements (e.g., pH, biological and chemical oxygen demand, conductivity, and flow rates) collected from a real-world wastewater treatment plant.

---
### 🔍 Key Dataset Column Indices & Parameters
Since the UCI dataset uses numerical indices instead of direct parameter names, key environmental and operational parameters are mapped as follows:
* **Index 1 - 2:** Flow Rate and operational measurements.
* **Index 3 - 4:** Inlet/Operational pH sensor metrics.
* **Index 5 - 8:** Chemical and Biological Oxygen Demand (COD/BOD) indicators.
* **Index 9 to 37:** Various multi-sensor water quality parameters.
* **Index 38:** Target effluent water quality parameter.

## 🚀 Key Features & Methodology
1. **Data Preprocessing & Cleaning:** Handled missing values using statistical imputation and structured multi-sensor feature matrices.
2. **Model Benchmarking:** Evaluated and compared multiple machine learning architectures (**Random Forest** vs. **XGBoost**).
3. **High Predictive Performance:** Achieved an **$R^2$ Score of 0.86** using XGBoost for precise effluent parameter forecasting.
4. **Automated Anomaly Detection:** Implemented statistical standard deviation thresholding ($Mean + 2\times StdDev$) to flag operational performance drops and high-risk anomalies in real-time.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Google Colab
* **Libraries:** `Pandas`, `NumPy`, `Scikit-learn`, `XGBoost`, `Matplotlib`, `Seaborn`

---

## 📊 Model Performance Comparison
| Model | Mean Squared Error (MSE) | $R^2$ Score |
| :--- | :--- | :--- |
| **Random Forest** | 52.99 | 0.2088 |
| **XGBoost** | **9.32** | **0.8607** |

---

## 📈 Visualizations
* **Actual vs. Predicted Effluent Quality:** Scatter plot showing model alignment against the ideal 1:1 fit line.
* **Anomaly & Threshold Alerting Graph:** Time-series style visualization highlighting critical operational anomalies with distinct markers.

---

## 💡 Acknowledgement
Inspired by advanced computational methods in environmental engineering and water resource management systems.
