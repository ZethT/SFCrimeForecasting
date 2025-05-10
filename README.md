# 🕵️ SF Crime Forecasting

This project aims to predict the **category of crime** in San Francisco using **time and location-based features**. By combining clustering, machine learning, and deep learning (LSTM), the notebook explores and models spatio-temporal crime trends.


---


## ✅ How to Use

1. Open the `SF Crime Forecasting - Colab.ipynb`
2. Download the dataset into your local device or use API from https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data
3. Run cells in order — all steps are labeled L1–L10
4. LSTM will auto-stop using early stopping and save its best weights

---


## 🧠 Project Goals

- Predict `crime_type_group` from time/location patterns
- Discover spatial crime hotspots (DBSCAN)
- Group crimes by behavior (KMeans)
- Evaluate model performance using traditional classifiers and LSTM

---


## 📊 Features Used

- **Temporal**: hour, day, month, year, day of week
- **Spatial**: neighborhood, police district, DBSCAN cluster
- **Frequency-based**: crime counts by time and area
- **Target**: `crime_type_group` (KMeans result from `incident_category`)

---

## 🧪 Models Trained

| Model              | Notes                                  |
|-------------------|----------------------------------------|
| RandomForest       | Strong all-around baseline             |
| LogisticRegression | Fast, interpretable                    |
| DecisionTree       | Simple, transparent decision-making    |
| LSTM               | Uses 24-hour sliding window sequences  |

All models are evaluated using accuracy, F1-score, and confusion matrix.

---

## 🔧 Requirements

```bash
pip install -r requirements.txt

