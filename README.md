# 🚕 Surge Pricing Prediction for Sigma Cabs

## 📝 Project Description

This project is focused on developing a machine learning model to predict the surge pricing type for **Sigma Cabs**, an Indian cab booking aggregator. This aggregator allows users to book cabs via an app by selecting optimal offers from various service providers operating in the cities where they are present.

The **goal** of the project is to create a model that can forecast the surge pricing type for each ride, enabling the company to manage customer expectations and improve driver allocation. This will ensure that customers receive quicker and more reliable service.

> This dataset was sourced from a [Kaggle competition](https://www.kaggle.com/datasets/arashnic/taxi-pricing-with-mobility-analytics) and was part of the coursework for a **Machine Learning Engineering** program. 

## 📊 Dataset

The dataset was provided by Sigma Cabs and includes a year’s worth of ride data and surge pricing factors. Key features:

- **Trip Data**: Includes details like trip distance, time of day, number of available cars nearby, and other factors potentially influencing surge pricing.
- **Target Feature**: `surge_pricing_type`, classifying each trip by the level of surge pricing applied.

## 🚀 Project Workflow

1. **Exploratory Data Analysis (EDA)**: Analyzing the data to uncover trends, outliers, and factors that influence surge pricing.
2. **Data Preprocessing**: Cleaning and processing the data, including scaling, handling missing values, and generating additional features to enhance model accuracy.
3. **Model Building and Training**: Training multiple machine learning models to predict `surge_pricing_type`. We compared two multi-class classification strategies:
    - **One-vs-One** (OvO)
    - **One-vs-Rest** (OvR)
4. **Model Evaluation**: Evaluating model prediction accuracy with metrics like `precision`, `recall`, and `F1-score`, averaged using micro, macro, and weighted methods.

## 🔧 Tools and Libraries

- **Python** 🐍: Main programming language
- **Pandas** and **NumPy**: For data processing and analysis
- **Scikit-Learn**: For model building and evaluation
- **Matplotlib** and **Seaborn** 📊: For data visualization and analysis

## 📈 Results

The model we developed accurately predicts the surge pricing type for rides, which can help Sigma Cabs manage demand and supply more effectively. This enables customers to locate available cabs faster, while drivers receive higher-value assignments, enhancing satisfaction for all parties.

## 🛠️ Installation and Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/surge-pricing-prediction.git
    cd surge-pricing-prediction
    ```

2. Install required libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. Launch Jupyter Notebook and open `surge_pricing_model.ipynb` to run the analysis and train the model:

    ```bash
    jupyter notebook surge_pricing_model.ipynb
    ```

## 🎉 Conclusion

Accurately predicting surge pricing is essential to enhancing efficiency and improving the service experience for Sigma Cabs. With this model, the aggregator can anticipate demand in advance, ensuring a better match between cabs and customers.
