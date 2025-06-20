Student Grade Prediction
Project Description
This project aims to predict student final grades (G3) based on various demographic, social, and school-related features using machine learning techniques. The analysis involves data loading, preprocessing, exploratory data analysis (EDA), feature selection, and model training and evaluation.

Data Source
The dataset used in this project is a combination of two datasets: student-por.csv (Portuguese language course) and student-mat.csv (Mathematics course), available in the specified path or you can visit ucl site for this dataset.

Analysis Steps
Data Loading and Merging: The two datasets were loaded and concatenated into a single pandas DataFrame.

Data Preprocessing: Checked for missing values and duplicates.
                    Explored the data types and summary statistics.
                    
Exploratory Data Analysis (EDA): Examined the distribution of categorical features.
                                 Analyzed the relationship between various features and the final grade (G3) using visualizations (bar plots).
                                 Generated a correlation heatmap to understand the relationships between numerical features.
                                 
Feature Selection: Based on the correlation analysis and initial visualizations, a subset of relevant features was selected for model training.

Data Splitting: The selected dataset was split into training and testing sets.
Feature Scaling: Numerical features were scaled using StandardScaler.

Model Training and Evaluation:
-->A Linear Regression model was trained on the scaled training data.
-->The model's performance was evaluated using R-squared and Mean Squared Error (MSE).
-->A Decision Tree Regressor was also trained and tuned using GridSearchCV for comparison.
-->The Linear Regression model showed better performance based on the evaluation metrics.

Model Saving: The trained Linear Regression model was saved using joblib for future use.
Results
The Linear Regression model achieved an R-squared score of approximately [0.84] and a Mean Squared Error (MSE) of approximately [2.25] on the test set. The actual vs. predicted grades were visualized to show the model's performance.

Model File
The trained Linear Regression model is saved as grade_prediction.pkl.

How to Run
Clone the repository.
Make sure you have the necessary libraries installed (pandas, numpy, matplotlib, seaborn, sklearn, joblib).
Place the student-por.csv and student-mat.csv files in a folder named Grade within a datasets folder in your Google Drive, and mount your Google Drive to /content/drive.
Run the Jupyter Notebook or Python script containing the code.
