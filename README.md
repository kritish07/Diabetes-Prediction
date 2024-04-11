## Diabetes Prediction Project

This project explores the use of machine learning to predict diabetes using the Pima Indians Diabetes Dataset.

### Dependencies

This project requires the following Python libraries:

* pyspark
* matplotlib
* seaborn
* pandas
* scikit-learn

### Getting Started

1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Download the Pima Indians Diabetes Dataset ([https://archive.ics.uci.edu/dataset/34/diabetes](https://archive.ics.uci.edu/dataset/34/diabetes)) and save it as `diabetes.csv` in the same directory as this README file.

### Running the Script

1. Open a terminal or command prompt and navigate to the directory containing the project files.
2. Run the script using `python diabetes_prediction.py` (or whichever filename you are using).

### Project Overview

The script performs the following steps:

1. **Spark Session Initialization:** Creates a SparkSession to work with the data using Apache Spark.
2. **Data Loading:** Loads the `diabetes.csv` file into a Spark DataFrame.
3. **Data Exploration:** Explores the data by printing the first 10 rows, displaying descriptive statistics, and checking data types.
4. **Data Cleaning:** Handles missing values and identifies outliers using the Interquartile Range (IQR) method. Replaces outliers with the mean of the data.
5. **Data Visualization:** Creates visualizations of the data distribution using bar charts and box plots.
6. **Feature Selection:** Selects all features except the target variable (`Outcome`).
7. **Data Splitting:** Splits the data into training and testing sets using `train_test_split` from scikit-learn.
8. **Data Scaling:** Scales the training and testing data using StandardScaler.
9. **Model Training:** Trains two machine learning models:
    * Logistic Regression
    * Random Forest Classifier
10. **Model Evaluation:** Evaluates the performance of each model using accuracy score, classification report, and confusion matrix.

### Future Work

* Explore other machine learning algorithms for diabetes prediction.
* Tune hyperparameters of the models for better performance.
* Feature engineering to create new features from existing ones.
* Deploy the model as a web application.

### Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue.

### License

This project is licensed under a custom license: LICENSE that restricts commercial use, distribution, patent or trademark use of the code. You are free to use the code for private, non-commercial purposes only.
