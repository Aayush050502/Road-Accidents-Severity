US Road Accidents Severity Prediction
Overview
This project analyzes US road accidents data from 2016-2023 using machine learning to predict accident severity. The model processes various features including weather conditions, time of day, and road characteristics to predict the severity level of accidents.
Dataset

Source: Kaggle US Accidents (2016-2023) dataset by Sobhan Moosavi
Size: ~7 million records (6,985,228 entries)
Features: 46 columns including temporal, spatial, weather, and road-related characteristics
Target Variable: Severity (1-4 scale)

Features

Temporal features (time of day, day of week, month, year)
Spatial coordinates (latitude, longitude)
Weather conditions and measurements
Road characteristics (traffic signals, junctions, etc.)
Environmental conditions (sunrise/sunset, twilight times)

Technical Implementation
Dependencies
pythonCopy- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- warnings
Project Structure

Data Loading and Preprocessing

Handles missing values
Removes irrelevant columns
Converts datatypes


Feature Engineering

Temporal feature extraction
Weather condition categorization
Boolean feature conversion
Categorical encoding


Exploratory Data Analysis (EDA)

Severity distribution visualization
Time of day analysis
Feature correlation analysis


Model Training

Data split: 75% training, 15% validation, 10% testing
Random Forest Classifier implementation
Feature importance analysis



Results
The model achieved perfect accuracy scores on the test dataset:

Test Accuracy: 1.0000
Detailed Test Accuracy: 1.0000

Data Structure
CopyData columns (46 total):
- Numerical features: 12 float64 columns
- Categorical features: 19 object columns
- Boolean features: 13 bool columns
- Datetime features: 1 datetime64[ns] column
- Target variable: Severity (int64)
Visualizations
The project includes several visualizations:

Severity distribution plots
Time of day vs. Severity analysis
Feature correlation heatmaps
Feature importance graphs

Installation and Usage

Clone the repository:

bashCopygit clone https://github.com/[username]/us-road-accidents-analysis.git

Install required packages:

bashCopypip install pandas numpy scikit-learn seaborn matplotlib

Run the analysis:

pythonCopypython main.py
Data Preprocessing Steps

Load and verify data from CSV
Handle missing values in numeric and categorical columns
Convert boolean indicators to integers
Engineer temporal and weather-related features
Encode categorical variables
Scale numerical features

Model Training Process

Split data into train/validation/test sets
Train Random Forest Classifier
Evaluate model performance
Generate feature importance analysis

Future Improvements

Implement cross-validation
Try different ML algorithms
Add more sophisticated feature engineering
Include hyperparameter tuning
Add model interpretability analysis

Contributing
Feel free to fork the repository and submit pull requests for any improvements.
License
This project is licensed under the MIT License - see the LICENSE.md file for details.
Acknowledgments

Dataset provided by Sobhan Moosavi on Kaggle
Built using scikit-learn and pandas libraries
