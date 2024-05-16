# Zomato Restaurant Rating Prediction

This project aims to predict restaurant ratings using machine learning techniques. The dataset used in this project is obtained from Zomato, a popular restaurant search and discovery service. The dataset contains various features such as restaurant name, location, type, cuisines, cost, and rating. The goal is to build a predictive model that can accurately predict the rating of a restaurant based on its features.

## File Structure

- `main.ipynb`: Jupyter notebook containing the code for data preprocessing, exploratory data analysis (EDA), feature engineering, model building, and deployment.
- `zomato.csv`: Dataset obtained from Zomato.
- `locations.csv`: CSV file containing latitude and longitude information for different locations.

## Getting Started

To run the project, follow these steps:

1. Ensure you have Python installed on your system.
2. Install the required dependencies listed in `requirements.txt`.
3. Run `main.ipynb` in a Jupyter notebook environment.

## Dataset

The dataset (`zomato.csv`) contains the following columns:

- `url`: URL of the restaurant on the Zomato website.
- `address`: Address of the restaurant in Bengaluru.
- `name`: Name of the restaurant.
- `online_order`: Whether online ordering is available at the restaurant or not.
- `book_table`: Whether table booking is available at the restaurant or not.
- `rate`: Overall rating of the restaurant (target variable).
- `votes`: Total number of ratings for the restaurant.
- `phone`: Phone number of the restaurant.
- `location`: Neighborhood in which the restaurant is located.
- `rest_type`: Type of restaurant.
- `dish_liked`: Dishes people liked in the restaurant.
- `cuisines`: Food styles, separated by commas.
- `approx_cost(for two people)`: Approximate cost for a meal for two people.
- `reviews_list`: List of tuples containing reviews for the restaurant.
- `menu_item`: List of menus available in the restaurant.
- `listed_in(type)`: Type of meal.
- `listed_in(city)`: Neighborhood in which the restaurant is listed.

## Exploratory Data Analysis (EDA)

The notebook includes various visualizations and analyses to understand the dataset better. It explores factors influencing restaurant ratings, popular cuisines, restaurant chains, location analysis, and more.

## Feature Engineering

- Categorical columns such as `online_order`, `book_table`, `location`, `rest_type`, and `type` are converted into numerical using one-hot encoding.
- Feature importance is extracted using the Extra Trees Regressor to select the top features for the model.

## Model Building

- Decision Tree Regressor is used to predict restaurant ratings based on selected features.
- Model performance metrics such as R-squared score, Mean Absolute Error (MAE), and Accuracy are calculated.
- The trained model is saved as `Decision_tree_model.pkl` for deployment.

## Deployment

The trained model can be deployed in production environments for real-time rating prediction.

