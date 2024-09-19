## Housing Price Prediction

This project involves predicting housing prices using various features like area, number of bedrooms, bathrooms, and more. The model is built using the XGBoost Regressor, a powerful machine learning algorithm for regression tasks.

### Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

### Project Overview
The goal of this project is to predict the price of a house based on several features. The dataset used contains 545 entries with 13 columns, providing a variety of information about each house.

### Dataset Description
The dataset `Housing.csv` includes the following columns:

1. `price`: Price of the house (target variable).
2. `area`: Area of the house in square feet.
3. `bedrooms`: Number of bedrooms.
4. `bathrooms`: Number of bathrooms.
5. `stories`: Number of floors.
6. `mainroad`: Access to the main road (`yes`/`no`).
7. `guestroom`: Presence of a guest room (`yes`/`no`).
8. `basement`: Presence of a basement (`yes`/`no`).
9. `hotwaterheating`: Availability of hot water heating (`yes`/`no`).
10. `airconditioning`: Presence of air conditioning (`yes`/`no`).
11. `parking`: Number of parking spaces.
12. `prefarea`: Located in a preferred area (`yes`/`no`).
13. `furnishingstatus`: Furnishing status of the house (`furnished`/`semi-furnished`/`unfurnished`).

### Exploratory Data Analysis (EDA)
- Analyzed the distribution and correlations of the features using visualizations like heatmaps and bar plots.
- Encoded categorical features such as `mainroad`, `guestroom`, and `basement` using Label Encoding for model training.

### Model Training and Evaluation
- **Model**: XGBoost Regressor was used for predicting house prices.
- **Train-Test Split**: 
  - Training set: 80% of the data.
  - Test set: 20% of the data.
- **Evaluation Metrics**: 
  - **Training R² Score**: 0.997
  - **Test R² Score**: 0.613
  - **Mean Squared Error (MSE)**: 1575.50

### Results
The model shows high accuracy on the training data but performs moderately on the test data, indicating potential overfitting. Future work may involve feature engineering and hyperparameter tuning to improve the model's generalization ability.

### Conclusion
This project demonstrates a comprehensive approach to housing price prediction using machine learning. While the model performs well on the training set, further improvements are needed for better test set performance.

### Future Work
- Implement more sophisticated feature engineering.
- Use advanced model tuning and cross-validation techniques.
- Experiment with different machine learning models and ensemble methods.

### Contributing
Contributions are welcome! Please create an issue or submit a pull request for any features, improvements, or bug fixes.

### License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
