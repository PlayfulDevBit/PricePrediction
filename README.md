# Simple Linear Regression for House Price Prediction

## Project Overview
This project implements a minimal linear regression model to predict house prices in California using median income. It includes a correlation matrix to analyze feature relationships, demonstrating supervised learning and model evaluation .

## Dataset
- **Source**: California Housing Prices from scikit-learn ([link](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)).
- **Description**: Housing data from California with features like `MedInc` (median income in tens of thousands of USD), `HouseAge`, `AveRooms`, and `MedHouseVal` (median house value).
- **Feature Used**: `MedInc` as the independent variable.
- **Target**: `MedHouseVal` (scaled to USD) as the dependent variable.

## Model
- **Algorithm**: Linear Regression from scikit-learn.
- **Performance**: Achieved an R² score of approximately 0.47, indicating that 47% of the variance in house prices is explained by median income.

## Correlation Analysis
- A correlation matrix is computed and visualized as a heatmap, showing relationships between all numerical features.
- Key finding: `MedInc` has a strong positive correlation (~0.69) with `MedHouseVal`, validating its use as a predictor.

## Files
- `price_prediction.ipynb`: Jupyter notebook with code for data loading, correlation analysis, model training, evaluation, and visualization.
- `README.md`: Project documentation.

## How to Run
1. Open `price_prediction.ipynb` in Google Colab or Jupyter Notebook.
2. Ensure dependencies (`pandas`, `scikit-learn`, `matplotlib`, `seaborn`) are installed (pre-installed in Colab).
3. Run the notebook cells to view the dataset’s first rows, correlation matrix, R² score, and visualizations.

## Why This Project?
This project showcases:
- Supervised learning (regression) with minimal code.
- Feature relationship analysis via correlation matrix.
- Visualization of predictions and correlations for interpretability.

## Future Improvements
- Use additional features (e.g., `HouseAge`, `AveRooms`) for better accuracy.
- Explore advanced models like Random Forest.
- Investigate non-linear relationships using polynomial features.

## Notes
- The California Housing dataset is loaded via scikit-learn’s `fetch_california_housing`, ensuring reliable access without external downloads. It contains 20,640 rows and 8 numerical features, plus the target (`MedHouseVal`).
