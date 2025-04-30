# Shipment Cost Prediction
This project focuses on analyzing and predicting the total construction shipment cost (Total Cost (₹)) using linear regression. The dataset is sourced from Kolte Patil's combined shipment records.

📁 Dataset
The dataset used: kolte_patil_combined_shipment_data 2.xlsx
The data contains shipment records with features such as:

Location

Project Type

Item Name

Order Date

Season

Weather

Rate (₹)

Total Weight (kg)

Total Cost (₹)

📌 Objectives
Perform initial data cleaning and preprocessing.

Encode categorical features using Label Encoding.

Extract temporal features from the Order Date.

Handle outliers using Winsorization (15th to 85th percentile).

Train and evaluate a Linear Regression model to predict Total Cost (₹).

🛠️ Workflow
1. Data Cleaning
Dropped irrelevant columns: Previous Orders This Month, Duration, Project ID, Project Name, Start Date, End Date, Item ID, Sacks per Shipment, Stock Level.

Checked for null values and datatypes.

2. Statistical Overview
Calculated mean, standard deviation, and median for:

Total Weight (kg)

Rate (₹)

Total Cost (₹)

3. Label Encoding
Encoded categorical columns:

Location

Project Type

Item Name

Season

Weather

4. Date Feature Engineering
Converted Order Date to datetime format.

Extracted OrderYear, OrderMonth, and OrderDay.

5. Outlier Handling (Winsorization)
Applied to:

Rate (₹)

Total Weight (kg)

Total Cost (₹)

Capped values below 15th and above 85th percentiles.

6. Modeling
Used Linear Regression to predict Total Cost (₹).

Dataset split: 70% training and 30% testing.

7. Evaluation Metrics
Metrics used:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

Accuracy (custom % metric)

8. Visualization
Plotted Actual vs. Predicted values for test data.

📊 Results
After training the model:

Displayed accuracy, R² score, and error metrics for both training and testing datasets.

Visualization showed the prediction trend.

🔧 Requirements
Install dependencies via pip:

bash
Copy
Edit
pip install pandas scikit-learn numpy matplotlib openpyxl
📌 File Structure
css
Copy
Edit
├── kolte_patil_combined_shipment_data 2.xlsx
├── main.py (or .ipynb)
├── README.md
📍 Author
Developed by [Vedant Deore]
Third-Year Computer Engineering Student, VIIT Pune
