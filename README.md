# **E-commerce User Churn Prediction**

This repository contains the implementation for predicting user churn on an e-commerce platform. The project involves analyzing user behavior data, engineering features, and building a machine learning model to identify users at risk of churn. Insights derived from the analysis are also used to recommend actionable strategies to improve user retention.


## **Features**

- **Data Preprocessing**: Cleaning and preparation of the event dataset for analysis.
- **Exploratory Data Analysis (EDA)**: Visualizations and key metrics to understand user behavior.
- **Feature Engineering**: Deriving meaningful user-level features like Recency, Frequency, and Monetary (RFM) metrics, session counts, and behavioral patterns.
- **Machine Learning Model**: A Random Forest model is trained to predict user churn.
- **Model Interpretation**: Use of SHAP values and feature importance to understand the model's predictions.
- **Business Recommendations**: Actionable insights to retain users and reduce churn.


## **Technologies Used**

- **Programming Language**: Python
- **Libraries**:
  - `pandas`, `numpy` for data manipulation.
  - `matplotlib`, `seaborn` for visualizations.
  - `sklearn` for model training and evaluation.
  - `shap` for model interpretability.


## **Installation and Usage**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/repo-name.git
   cd repo-name
   ```

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Place the `events.csv` file in the same directory as the notebook.

4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

5. Open and execute the `user_churn_prediction.ipynb` file step by step.


## **Dataset**

The dataset, `events.csv`, contains user activity logs with the following columns:
- `event_time`: Datetime of the user event.
- `event_type`: Type of the event (`view`, `cart`, or `purchase`).
- `product_id`: Identifier of the product.
- `category_code`: Human-readable product category.
- `price`: Price of the product.
- `user_id`: Identifier of the user.
- `user_session`: Identifier of the user's session.


## **Project Workflow**

1. **Data Preprocessing**: Handling missing values, converting data types, and ensuring consistency.
2. **EDA**: Identifying key trends, such as the distribution of events and popular product categories.
3. **Feature Engineering**: Creating user-specific features that indicate churn signals.
4. **Model Training**: Training a Random Forest classifier to predict churn.
5. **Model Evaluation**: Assessing model performance using metrics like AUC and F1-score.
6. **Interpretation**: Understanding the impact of features using SHAP values.
7. **Recommendations**: Providing strategies to enhance user retention.


## **Results**

- **Model Performance**:
  - AUC: `e.g., 0.85`
  - F1-Score: `e.g., 0.78`
- **Key Insights**:
  - Users with high recency and low session frequency are more likely to churn.
  - Product categories with low purchase conversion rates are associated with higher churn.


## **Business Recommendations**

- Focus on re-engaging users with high recency but low frequency through targeted marketing campaigns.
- Offer personalized discounts on products with high view-to-cart ratios but low purchases.
- Improve product recommendations to align with user preferences.


## **Contributing**

Contributions are welcome! Feel free to submit a pull request or open an issue.


## **License**

This project is licensed under the MIT License.
