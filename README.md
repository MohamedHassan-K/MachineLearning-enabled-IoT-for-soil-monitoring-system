# Crop Recommendation System

## Overview
This project implements a crop recommendation system using machine learning algorithms. The goal is to help farmers choose the best crop to plant based on various environmental and soil parameters. The system utilizes data from a CSV file and includes data preprocessing, exploratory data analysis, model training, and evaluation.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib
- Plotly
- CatBoost
- LightGBM
- Jupyter Notebook
- Joblib

## Data Description
The dataset used for this project is `Crop_recommendation.csv`, which includes the following features:
- `N`: Nitrogen content in the soil
- `P`: Phosphorus content in the soil
- `K`: Potassium content in the soil
- `temperature`: Temperature of the environment
- `humidity`: Humidity percentage
- `ph`: pH value of the soil
- `rainfall`: Rainfall in mm
- `label`: Recommended crop

## Exploratory Data Analysis
The exploratory data analysis includes:
- Checking for duplicates and missing values
- Descriptive statistics of the dataset
- Visualizations of the distributions and relationships between features
- Detection and removal of outliers using the Interquartile Range (IQR) method

## Modeling
Two machine learning models were implemented:
1. **CatBoostClassifier**
2. **LGBMClassifier**

Both models were trained on the processed dataset, and their performance was evaluated using accuracy and confusion matrices.

## Usage
To run the application:
1. Ensure you have all the required libraries installed.
2. Run the `app.py` script to launch the prediction application.
3. The application will prompt for the input parameters and predict the best crop to plant.

### Example Input
- Nitrogen content: `N`
- Phosphorus content: `P`
- Potassium content: `K`
- Temperature: `temperature`
- Humidity: `humidity`
- pH: `ph`
- Rainfall: `rainfall`

### Example Output
- Recommended Crop: `label`

## Files Included
- `Crop_recommendation.csv`: The dataset used for training the model.
- `notebook.ipynb`: Jupyter notebook containing data analysis, preprocessing, and model training code.
- `app.py`: Flask application to run the crop prediction service.
- `crop_app`: Saved model file using Joblib.

## License
This project is licensed under the MIT License.

