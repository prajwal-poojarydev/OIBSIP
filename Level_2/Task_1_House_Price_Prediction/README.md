# House Price Prediction Using Linear Regression

## Internship
Oasis Infobyte Data Analytics Internship — Level 2, Task 1

## Project Overview
This project uses machine learning to predict residential house sale prices using the Ames Housing dataset. It includes data exploration, preprocessing, model training, evaluation, and visualization.

## Dataset
- **Source:** [OpenML — Ames Housing](https://www.openml.org/)
- **Rows:** 1,460
- **Columns:** 81 in the original dataset
- **Target variable:** `SalePrice`

## Tools and Libraries
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Workflow
1. Explored the dataset and identified missing values.
2. Prepared numerical and categorical features.
3. Imputed missing values using median and most-frequent strategies.
4. Encoded categorical features using one-hot encoding.
5. Split the data into 80% training and 20% testing sets.
6. Trained a Linear Regression model.
7. Evaluated predictions and visualized model performance.
8. Examined regression coefficients to understand feature associations.

## Model Performance

| Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | $20,466.13 |
| Root Mean Squared Error (RMSE) | $31,294.99 |
| R² Score | 0.8723 |

The model explains approximately 87.23% of the variation in sale prices on this test split. These results are a baseline and do not guarantee the same performance on new data.

## Visualizations
- House sale price distribution
- Actual versus predicted prices
- Residual plot
- Positive regression coefficients

## Files
- `PrajwalPoojary_Level2_Task1.ipynb` — notebook containing the analysis and model
- `Ames_Housing.csv` — converted dataset
- `dataset.arff` — original dataset file
- `README.md` — project documentation

## Conclusion
The Linear Regression model provides a useful baseline for estimating house sale prices. Evaluation metrics and visualizations help identify prediction errors and areas for improvement.

**Author:** Prajwal Poojary