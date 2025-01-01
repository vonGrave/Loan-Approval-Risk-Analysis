# German Credit Risk Analysis

## Project Overview
This project implements a logistic regression model to predict credit risk for bank loan applications. The model helps banks make informed decisions about loan approvals by analyzing various demographic and socio-economic factors of applicants.

## Dataset Description
The dataset (German_Credit.csv) contains information about bank customers and their credit risk status, including:
- Age (numeric)
- Sex (male/female)
- Job (skill levels)
- Housing status (own/rent/free)
- Saving accounts (little/moderate/quite rich/rich)
- Checking account (little/moderate/rich)
- Credit amount (in Deutsche Mark)
- Duration (loan duration in months)
- Purpose (car/furniture/radio/TV/etc.)
- Risk (0=good credit, 1=bad credit)

## Technical Details
### Libraries Used
pandas
numpy
matplotlib
seaborn
statsmodels
sklearn

### Model Performance
Three threshold variations were tested:
1. Default threshold:
- High precision, lower recall
- Best for minimizing resource expenditure
2. 0.27 threshold:
- High recall (76%), lower precision
- Best for identifying potential customers
3. 0.36 threshold:
- Balanced precision and recall
- Recommended for optimal resource allocation

## Key Findings
1. Duration is a significant predictor of default risk
2. Male customers show lower default probability
3. Customers with low/moderate savings are higher risk
4. Housing status (rent/free) correlates with default risk
5. Younger customers show slightly higher default rates

## Recommendations
1. Implement stricter policies for high-risk categories
2. Adjust interest rates based on risk factors
3. Enhanced documentation for non-homeowners
4. Modified policies for younger applicants
5. Focus on balanced threshold model for optimal results

## Running the Analysis
1. Ensure all required libraries are installed
2. Place the German_Credit.csv file in the working directory
3. Run the Jupyter notebook Logistric_Regression_German_Credit.ipynb

## Requirements
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- StatsModels

## Future Improvements
- Implementation of additional machine learning models
- Feature engineering
- Cross-validation
- Hyperparameter optimization
- Cost-sensitive learning implementation

Duration (Numeric: Duration for which the credit is given in months)

Purpose (Categories: car, furniture/equipment,radio/TV, domestic appliances, repairs, education, business, vacation/others)

Risk (0 - Person is not at risk, 1 - Person is at risk(defaulter))
