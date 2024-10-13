
# End-to-End Healthcare Analytics Using Snowflake and AWS SageMaker

## Business Overview
In this project, I leveraged machine learning to improve service delivery and patient care in a hospital, specifically by predicting the length of stay (LOS) of patients. A patient’s LOS has critical implications for patient outcomes, healthcare costs, and hospital efficiency, and by analysing anonymised patient data, healthcare providers can preemptively improve care provision and reduce operational costs.

## Objectives
- Analyse healthcare data stored in Snowflake.
- Build machine learning models to predict patient LOS.
- Deploy the models using AWS SageMaker.
- Monitor model drift and retrain as necessary using AWS infrastructure.
- Automate predictions and status reporting.

## Tech Stack
- **Tools**: AWS SageMaker, Snowflake
- **Languages**: Python, SQL
- **Libraries**:
  - Data Handling: pandas, numpy, scikit-learn
  - ML Models: xgboost, RandomForestRegressor
  - Data Connectivity: snowflake-connector-python, snowflake-sqlalchemy

## Project Workflow
1. **Data Acquisition**: 230k anonymised patients' data (19 features).
2. **Exploratory Data Analysis (EDA)**: Comprehensive data analysis in Snowflake.
3. **Feature Engineering**: Development of specific predictive features using Snowflake SQL.
4. **Model Building**: Trained multiple models including:
    - Linear Regression
    - Random Forest
    - XGBoost
5. **Model Deployment**: The best model was deployed using AWS SageMaker.
6. **Live Scoring**: Integrated the predicted results back into Snowflake.
7. **Model Retraining**: A pipeline was created to monitor data/model drift, with automated retraining.

## Files Overview
- `SQL/`: Contains the SQL queries used in Snowflake for data handling and feature engineering.
- `notebooks/`: Jupyter Notebooks for running the entire pipeline in AWS SageMaker.
- `scripts and models/`: Contains Python files for fetching data from Snowflake, preprocessing, and building machine learning models.
- `data/`: Simulation and training data files.

## Details on Healthcare Project Implementation
To further explain the project, I have also created a detailed report covering:
- **Data Preparation**: Data exploration, feature engineering, and Snowflake integration.
- **Model Building**: Description of models, performance metrics, and model selection.
- **Model Deployment and Scoring**: Integration with Snowflake for predictions.
- **Monitoring and Retraining**: Handling data and model drift using statistical tests.
- **Automation and Notifications**: Using SageMaker for scheduling and sending alerts.
