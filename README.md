# Bank Telemarketing Prediction  

This repository contains a machine learning project aimed at predicting whether a client will subscribe to a term deposit based on data from direct marketing campaigns of a banking institution. The project is based on a Kaggle competition dataset, and the marketing campaigns were conducted via phone calls.  

---

## Table of Contents  
- [Project Overview](#project-overview)  
- [Dataset Description](#dataset-description)  
- [Approach](#approach)  
- [Results](#results)  
- [Usage](#usage)  
- [File Structure](#file-structure)  
- [Acknowledgments](#acknowledgments)  

---

## Project Overview  
Banking institutions often rely on direct marketing campaigns to promote products like term deposits. These campaigns can be expensive, and predicting customer behavior helps optimize efforts and resources. This project applies machine learning techniques to analyze client data and predict whether they will subscribe to a term deposit.  

The target variable for this prediction is:  
`target`: Whether the client subscribed to a term deposit (`yes` or `no`).  

---

## Dataset Description  
The dataset contains information collected from previous marketing campaigns. It is divided into training and test sets:  

- **`train.csv`**: Training dataset used to build the predictive model.  
- **`test.csv`**: Test dataset used for evaluation.  
- **`sample_submission.csv`**: Sample output file format for predictions.  

### Input Variables  
The dataset includes the following features:  

1. **`last_contact_date`**: Date of the last contact during the campaign.  
2. **`age`**: Age of the client (numeric).  
3. **`job`**: Type of job (categorical).  
4. **`marital`**: Marital status (categorical: "married", "divorced", "single").  
5. **`education`**: Education level (categorical: "unknown", "secondary", "primary", "tertiary").  
6. **`default`**: Has credit in default? (binary: "yes", "no").  
7. **`balance`**: Average yearly balance in euros (numeric).  
8. **`housing`**: Has a housing loan? (binary: "yes", "no").  
9. **`loan`**: Has a personal loan? (binary: "yes", "no").  
10. **`contact`**: Contact communication type (categorical: "unknown", "telephone", "cellular").  
11. **`duration`**: Last contact duration in seconds (numeric).  
12. **`campaign`**: Number of contacts performed during this campaign (numeric).  
13. **`pdays`**: Days since the client was last contacted (-1 if not previously contacted).  
14. **`previous`**: Number of contacts before this campaign (numeric).  
15. **`poutcome`**: Outcome of the previous marketing campaign (categorical: "unknown", "other", "failure", "success").  

### Target Variable  
- **`target`**: Whether the client subscribed to a term deposit (`yes` or `no`).  

---

## Approach  
The project follows these key steps:  

1. **Data Cleaning and Preprocessing**:  
   - Handling missing values.  
   - Encoding categorical variables.  
   - Feature scaling and transformation.  

2. **Exploratory Data Analysis (EDA)**:  
   - Visualization of feature distributions and relationships.  
   - Insights into factors influencing customer subscription.  

3. **Modeling**:  
   - Tried multiple classification algorithms (e.g., Logistic Regression, Random Forest, Gradient Boosting).  
   - Optimized hyperparameters using grid search.  

4. **Evaluation**:  
   - Measured performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.  

---

## Results  
- Best-performing model achieved **[accuracy/performance metric]** on the test set.  
- Insights: Features like `duration`, `campaign`, and `poutcome` were significant predictors.  

---

## File Structure

- train.csv: Training dataset.
- test.csv: Test dataset.
- sample_submission.csv: Sample output format.
- notebooks/: Jupyter notebooks for EDA and model development.
- scripts/: Python scripts for preprocessing, training, and evaluation.
- README.md: Project documentation.

## Acknowledgments

- Dataset: Kaggle Bank Marketing Dataset.
- Inspired by the need to optimize banking resources for targeted marketing.

Feel free to contribute, raise issues, or suggest improvements. Happy coding!
