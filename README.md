
````markdown
# 🌾 Crop Recommendation System using Machine Learning

## 📌 Project Overview

This project aims to help farmers and agricultural stakeholders by predicting the **most suitable crop** to grow based on specific environmental and soil parameters using a machine learning model. Leveraging the **LightGBM classifier**, we provide highly accurate crop recommendations based on inputs such as:

- Nitrogen (N)
- Phosphorous (P)
- Potassium (K)
- Temperature
- Humidity
- pH level
- Rainfall


## 🧠 Machine Learning Model

We use **LightGBM (Light Gradient Boosting Machine)**, a fast, efficient, and accurate algorithm known for handling large-scale and high-dimensional data. It's particularly well-suited for tabular datasets like ours.

### ✅ Model Performance:
- **Accuracy:** `98.90%`
- **Classifier Report:** High precision and recall for almost all 22 crop classes.
- **Confusion Matrix:** Shows strong classification performance with minimal misclassifications.


## 📊 Features Used

| Feature      | Description                       |
|--------------|-----------------------------------|
| `N`          | Nitrogen content in the soil      |
| `P`          | Phosphorous content in the soil   |
| `K`          | Potassium content in the soil     |
| `temperature`| Average temperature (°C)          |
| `humidity`   | Relative humidity (%)             |
| `ph`         | Soil pH value                     |
| `rainfall`   | Rainfall in mm                    |


## 📈 Visualizations

- **NPK ratio comparison** using Pie Charts for various crops.
- **Scatter plots** to show temperature vs. humidity distribution by crop.
- **Bar Charts** for comparing environmental features.
- **Correlation Heatmap** to understand feature relationships.


## 🛠️ How to Use

1. Clone the repository or run the notebook on [Kaggle](https://www.kaggle.com/) / [Google Colab](https://colab.research.google.com).
2. Install required libraries:

```bash
pip install lightgbm seaborn plotly pandas numpy matplotlib
````

3. Load the dataset:

   * Dataset used: `Crop_recommendation.csv`
   * Make sure it's in the same directory or update the path in the notebook.

4. Run the Jupyter Notebook / Script and enter values for:

   * N, P, K
   * Temperature
   * Humidity
   * pH
   * Rainfall

5. The model will output the most suitable crop to grow in the given conditions.

## 🔍 Sample Prediction

```python
input = [[90, 42, 43, 20.879, 82.0, 6.5, 202.9]]
prediction = model.predict(input)
print("Recommended Crop:", prediction[0])
```


## 📂 Project Structure

```
├── Crop_Recommendation.ipynb
├── Crop_recommendation.csv
├── README.md
└── requirements.txt
```

---

## 💡 Outcome

This ML-based crop recommendation system can assist:

* Farmers with **data-driven decisions**
* Agricultural agencies for **sustainability**
* Researchers for **further agricultural data modeling**


