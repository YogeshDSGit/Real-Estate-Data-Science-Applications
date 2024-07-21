# Real Estate Data Science Application

## Project Overview

In this comprehensive capstone project, we leveraged data science techniques to provide insights, predictions, and recommendations in the real estate domain. The project unfolds through various stages, covering data gathering, cleaning, exploratory analysis, modeling, recommendation systems, and the deployment of a user-friendly application.

## Table of Contents
- [Data Gathering](#data-gathering)
- [Data Cleaning and Merging](#data-cleaning-and-merging)
- [Feature Engineering](#feature-engineering)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Outlier Detection and Missing Value Imputation](#outlier-detection-and-missing-value-imputation)
- [Feature Selection](#feature-selection)
- [Model Selection & Productionalization](#model-selection--productionalization)
- [Building the Analytics Module](#building-the-analytics-module)
- [Building the Recommender System](#building-the-recommender-system)
- [Deploying the Application on AWS](#deploying-the-application-on-aws)
- [Conclusion](#conclusion)
- [How to Use](#how-to-use)
- [Prerequisites](#prerequisites)
- [Repository Structure](#repository-structure)
- [Contact](#contact)

## Data Gathering
The project commenced with the collection of real estate data, which was self-scraped from the 99acres website. Similar datasets from other property listing websites were also explored, ensuring a diverse and representative dataset.

## Data Cleaning and Merging
To prepare the dataset for analysis, a meticulous data cleaning process was undertaken, handling missing values and ensuring consistency. The data was then merged, bringing together information on houses and flats into a unified dataset.

## Feature Engineering
The dataset underwent feature engineering to enhance its richness and informativeness. New features, such as additional room indicators, area with type specifications, age of possession, furnish details, and a luxury score, were introduced to provide a more detailed representation of the properties.

## Exploratory Data Analysis (EDA)
Univariate and multivariate analyses were conducted to uncover patterns and relationships within the data. The use of Pandas Profiling facilitated a deeper understanding of data distribution and structure.

## Outlier Detection and Missing Value Imputation
Outliers were identified and removed to ensure the robustness of subsequent analyses. Missing values, particularly in critical columns like area and bedroom, were addressed using appropriate imputation techniques.

## Feature Selection
Multiple feature selection techniques were employed to identify the most impactful variables for modeling. These included correlation analysis, random forest and gradient boosting feature importance, permutation importance, LASSO, recursive feature elimination, and SHAP (Explainable AI).

## Model Selection & Productionalization
An exhaustive comparison of various regression models was conducted to determine the most effective model for predicting property prices. The process involved implementing a detailed price prediction pipeline that incorporated encoding methods, ensuring the robustness and accuracy of the chosen model. The selected model was then deployed using Streamlit, creating an intuitive and user-friendly web interface for end-users.

### Regression Models Considered
- **Linear Regression**: A foundational regression model that assumes a linear relationship between the input features and the target variable.
- **Support Vector Regression (SVR)**: A regression technique that leverages support vector machines to find a hyperplane that best fits the data, allowing for nonlinear relationships.
- **Random Forest Regressor**: An ensemble learning method that builds a multitude of decision trees during training and outputs the average prediction of the individual trees.
- **LASSO Regression**: A linear regression technique that incorporates L1 regularization, encouraging sparsity in the coefficient estimates.
- **Ridge Regression**: A linear regression technique with L2 regularization, which helps prevent multicollinearity and stabilizes the model.
- **Gradient Boosting Regressor**: An ensemble learning method that builds trees sequentially, with each tree correcting the errors of the previous ones.
- **Decision Tree Regressor**: A non-linear regression model that splits the dataset into subsets based on the most significant attribute at each node.
- **K-Nearest Neighbors Regressor**: A regression model that predicts the target variable by averaging the values of its k-nearest neighbors.
- **ElasticNet Regression**: A linear regression technique that combines L1 and L2 regularization terms.

The comparison involved assessing the performance of each model on relevant evaluation metrics, considering factors such as accuracy, precision, and recall. The most suitable regression model was selected based on its overall performance and ability to generalize to new data.

The chosen regression model was then integrated into a comprehensive price prediction pipeline, which included preprocessing steps, encoding methods, and handling of various features to ensure optimal performance. The final model was deployed using Streamlit, creating an interactive and user-friendly web interface for predicting property prices. This productionalization step made the model accessible to end-users, allowing them to make informed decisions in the real estate domain.

## Building the Analytics Module
An analytics module was developed to visually represent key insights about the real estate data. Geographical maps, word clouds for amenities, scatter plots, pie charts, and box plots were employed to offer users a comprehensive understanding of the market.

## Building the Recommender System
Three distinct recommendation models were developed, each focusing on different aspects of the real estate dataset: top facilities, price details, and location advantages. The goal was to provide users with personalized recommendations tailored to their preferences and priorities. Additionally, a user-friendly recommendation interface was crafted using Streamlit, enhancing the accessibility of the recommendation systems.

## Deploying the Application on AWS
The entire application, encompassing prediction, analytics, and recommendation functionalities, was deployed on Amazon Web Services (AWS). This step ensured the scalability and accessibility of the project.

## Conclusion
This capstone project not only demonstrates proficiency in data science techniques such as feature engineering, exploratory analysis, and model building but also showcases the deployment of a real-world application, making valuable insights and recommendations accessible to end-users.

## How to Use

### Prerequisites
- Python 3.7+
- Streamlit
- Pandas
- Scikit-learn

## Repository Structure
- `data/`: Contains the raw and cleaned data.
- `notebooks/`: Jupyter notebooks for data exploration and model development.
- `models/`: Trained models and scripts for model training.
- `app.py`: Main application script for Streamlit.
- `README.md`: Project overview and instructions.

## Contact
For any questions or issues, please contact [Yogesh](mailto:yogeshdhaliyaa@gmail.com).

---

Feel free to use, modify, and share this project. Contributions are welcome!
