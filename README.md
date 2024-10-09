# Biscoff
 Integration of AI in business
Here’s a sample `README.md` file for your Git repository, which includes the key information about the program, its functionality, and how to run it. The example output can be included, but it's typically optional. If you want to provide a quick view of the program’s performance, you can include it in the "Example Output" section.

---

## Credit Risk Assessment using AI

This project integrates AI (Logistic Regression) into the finance domain by predicting the credit risk of customers. The program takes customer financial data, such as age, income, loan amount, and credit score, and predicts whether the customer is likely to default on their loan.

### Features
- **Credit Risk Prediction**: Predicts whether a customer will default on their loan using logistic regression.
- **Data Normalization**: Financial features are normalized for more accurate prediction.
- **Model Training and Evaluation**: The program splits the data into training and testing sets, evaluates the model's performance, and provides an accuracy score and classification report.
- **Customer Risk Assessment**: For new customer data, the program provides a prediction and the probability of default.

### Technologies Used
- Python
- Pandas (for data handling)
- Scikit-learn (for machine learning)
- Logistic Regression Model
- Excel file for input data

### Installation and Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/credit-risk-assessment.git
    ```
   
2. **Install required libraries**:
    You can install the necessary libraries by running:
    ```bash
    pip install pandas scikit-learn
    ```

3. **Prepare your data**:
    Ensure you have an Excel file (`customer_risk_data.xlsx`) with the following columns:
    - `Age`: Age of the customer
    - `Income`: Annual income of the customer
    - `LoanAmount`: The loan amount requested by the customer
    - `CreditScore`: The customer’s credit score
    - `Default`: (1 = Default, 0 = No Default)

4. **Run the program**:
    Run the Python program using the following command:
    ```bash
    python credit_risk_assessment.py
    ```

### How It Works
1. The program loads customer financial data from an Excel file.
2. The features (`Age`, `Income`, `LoanAmount`, `CreditScore`) are normalized using `StandardScaler`.
3. A logistic regression model is trained using the data to predict customer default.
4. The program prints the model accuracy, classification report, and makes predictions for new customer data.

### Example Output
The program outputs the accuracy and a classification report after training the model. It also predicts whether a new customer will default on their loan:

```
Model Accuracy: 0.87
Classification Report:
              precision    recall  f1-score   support

           0       0.90      0.92      0.91       150
           1       0.82      0.78      0.80        50

    accuracy                           0.87       200
   macro avg       0.86      0.85      0.85       200
weighted avg       0.87      0.87      0.87       200

Prediction: Low Risk of Default (Probability: 0.15)
```

### Customization
You can replace the new customer data for predictions by editing the `new_customer_data` array in the code:
```python
new_customer_data = [[45, 50000, 15000, 650]]  # Age, Income, LoanAmount, CreditScore
```

### Contribution
Feel free to fork this repository, submit issues, and contribute via pull requests.

