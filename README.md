# Finnish Housing Price Prediction (EUR/m²)

This project implements an AI-based regression model to predict Finnish residential housing prices as **price per square meter (EUR/m²)**.

The system is designed as a decision-support tool for buyers, sellers, agents, and investors.

---

## Data Source

Statistics Finland (StatFin) – *Prices of dwellings in housing companies*

The dataset contains historical housing transaction data aggregated at municipality level.

### MVP Features:
- Municipality
- Building type
- Year

### Target:
- Price per square meter (EUR/m²)

---

## Model

The MVP uses **Ridge Regression**, a regularized linear regression model.

Ridge was selected because:
- The dataset is relatively small (~190 samples)
- One-hot encoding increases feature dimensionality
- Regularization improves stability and generalization
- It reduces the risk of overfitting

---

## Model Evaluation

The model is evaluated using:

- 5-fold cross-validation
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

These metrics quantify prediction accuracy in meaningful units (EUR/m²).

---

## How to Run

1. Clone the repository:

   git clone https://github.com/VVeikkola/finnish-housing-price-ml.git

2. Install dependencies:

   pip install -r requirements.txt

3. Open:

   mvp_housing.ipynb

4. Run all cells.

---

## Output

The notebook outputs a predicted **price per square meter (EUR/m²)** based on the provided property inputs.

---

## Notes

This is a Minimum Viable Product (MVP) intended for academic purposes.  
The model provides estimation only and should not be considered financial or legal advice.
