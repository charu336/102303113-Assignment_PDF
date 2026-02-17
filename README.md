# 102303113-Assignment_PDF
# Assignment-1: Learning Probability Density Functions

## Objective
To learn probability density functions using a roll-number-parameterized non-linear transformation on NO₂ air quality data.

## Dataset
India Air Quality Dataset (NO₂ feature used)

Dataset link:
https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data

## Transformation
Each NO₂ value (x) is transformed into z using:

z = x + a_r sin(b_r x)

where:
- a_r = 0.05 × (r mod 7)
- b_r = 0.3 × (r mod 5 + 1)
- r = University Roll Number

## Probability Density Function
The transformed variable z is modeled using:

p̂(z) = c · exp(−λ (z − μ)²)

The parameters λ, μ, and c are learned using statistical estimation.

## Files
- `assignment1.ipynb` – Complete implementation and results

## Libraries Used
- numpy
- pandas
- matplotlib

## Output
The final learned parameters (λ, μ, c) are printed in the notebook and submitted through the provided Google Form.

## Notes
- Dataset is not uploaded due to Kaggle licensing.
- Encoding issues are handled using Latin-1 encoding.
