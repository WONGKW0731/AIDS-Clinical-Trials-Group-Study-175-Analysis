# AIDS Clinical Trials Group Study 175 Analysis

This project analyzes data from the AIDS Clinical Trials Group Study 175 to predict patient outcomes. The primary goal is to develop an accurate predictive model to determine the most effective AIDS treatment, ultimately helping to prolong patient lifetimes. This repository contains the complete data science project, from data exploration to model deployment.

This project was completed by students of the Bachelor of Computer Science (Honors) in Data Science program at Tunku Abdul Rahman University of Management and Technology (TAR UMT) for the BACS3013 Data Science course.

## Methodology

The project followed a structured data science lifecycle:

1.  **Business Understanding:** Defining the project's objective to predict patient outcomes to identify the most effective AIDS treatment.
2.  **Data Understanding:** Collecting, describing, and exploring the dataset to identify initial patterns and assess data quality.
3.  **Data Preparation:** Cleaning the data, handling outliers and zero values, selecting relevant features using ANOVA and Chi-Squared tests, and normalizing the data.
4.  **Modeling:** Developing and training three different machine learning models (Logistic Regression, Random Forest, and Artificial Neural Network) to predict the target variable. The dataset was resampled to handle class imbalance.
5.  **Evaluation:** Comparing the models based on key performance metrics like accuracy, precision, recall, and F1-score to identify the best-performing model.
6.  **Deployment:** Creating a user interface to allow for predictions based on new input data using the best model.

## Dataset

The dataset used for this project is the **AIDS Clinical Trials Group Study 175** from the UC Irvine Machine Learning Repository.

* **Instances:** 2139
* **Features:** 25 (including patient demographics, medical history, and lab results)
* **Target Variable (`cid`):** A binary indicator where `1` represents patient death (failure) and `0` represents censoring.

## Modeling and Results

Three classification models were developed and evaluated. After hyperparameter tuning and training on a balanced dataset, the models achieved the following accuracies:

* **Logistic Regression:** 86%
* **Artificial Neural Network (ANN):** 88%
* **Random Forest:** 89%

The **Random Forest** model was selected as the best-performing model due to its superior accuracy and balanced performance across other metrics.

## Usage

To run this project, you will need Python and the libraries listed in the `requirements.txt` file.

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    ```
2.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the analysis:**
    The main analysis, including data preprocessing, model training, and evaluation, is contained in the `final (1).ipynb` Jupyter Notebook.

## File Structure

