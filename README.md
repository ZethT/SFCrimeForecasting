# 🕵️ SF Crime Forecasting

This project aims to predict the **category of crime** in San Francisco using **time and location-based features**. By combining clustering, machine learning, and deep learning (LSTM), the notebook explores and models spatio-temporal crime trends.

---

## ✅ How to Use

- Using the API or download the dataset(SF Crime Forecasting.ipynb) to you local machine/Google Drive
- Upload or mount the dataset (CSV file with police incident reports) via Google Drive.
- For LSTM training, the notebook will automatically save the best model weights using ModelCheckpoint. If training is interrupted, reload the model using load_model('model_checkpoint.h5') and resume training.

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

| Model              | Notes                                 |
| ------------------ | ------------------------------------- |
| RandomForest       | Strong all-around baseline            |
| LogisticRegression | Fast, interpretable                   |
| DecisionTree       | Simple, transparent decision-making   |
| LSTM               | Uses 24-hour sliding window sequences |

All models are evaluated using accuracy, F1-score, and confusion matrix.

---

## 🔧 Requirements

```bash
pip install -r requirements.txt

```
