# Hybrid Time Series Forecasting using Statistical & ML Models

A comprehensive time series forecasting project leveraging both statistical and machine learning approaches to predict future values. This project demonstrates the integration of traditional statistical methods with modern machine learning algorithms for robust forecasting capabilities.

## Project Overview

This project implements a hybrid forecasting system that combines:
- **Statistical Models**: StatsForecast for baseline predictions
- **Machine Learning Models**: Ridge Regression, Random Forest, XGBoost, and Histogram-based Gradient Boosting

The models are trained and evaluated using time-based data splitting and advanced feature engineering techniques to ensure temporal integrity and prevent data leakage.

## Features

- **Multiple Model Architecture**: Implementation of 5 different forecasting models
  - StatsForecast (Statistical baseline)
  - Ridge Regression
  - Random Forest
  - XGBoost
  - Histogram-based Gradient Boosting

- **Advanced Feature Engineering**:
  - Lag features for capturing historical patterns
  - Rolling window statistics for trend analysis
  - Time-based feature extraction

- **Proper Validation Strategy**:
  - Time-based train-test split to maintain temporal order
  - Prevents data leakage in time series forecasting

- **Comprehensive Evaluation**:
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)
  - R² Score for model comparison

## Technologies Used

- **Data Processing**: `pandas`, `numpy`
- **Visualization**: `matplotlib`
- **Statistical Models**: `statsforecast`
- **Machine Learning**: `scikit-learn`, `xgboost`
- **Development Platform**: Kaggle Notebooks

## Requirements

See `requirements.txt` for complete list of dependencies.

Key libraries:
```
pandas
numpy
matplotlib
statsforecast
scikit-learn
xgboost
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/udayprattap/time-series-forecasting.git
cd time-series-forecasting
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Model Performance

The project evaluates all models using three key metrics:
- **MSE (Mean Squared Error)**: Measures average squared difference between predictions and actual values
- **MAE (Mean Absolute Error)**: Measures average absolute difference
- **R² Score**: Indicates the proportion of variance explained by the model

## Methodology

1. **Data Preprocessing**: Clean and prepare time series data
2. **Feature Engineering**: Create lag features and rolling statistics
3. **Train-Test Split**: Time-based splitting to maintain temporal order
4. **Model Training**: Train multiple models on the same feature set
5. **Evaluation**: Compare models using MSE, MAE, and R² metrics
6. **Model Selection**: Identify the best performing model

## Project Structure

```
time-series-forecasting/
├── README.md
├── requirements.txt
├── .gitignore
└── notebooks/          # Kaggle notebooks (if added)
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is available for educational and research purposes.

## Author

**Uday Prattap**
- GitHub: [@udayprattap](https://github.com/udayprattap)

## Acknowledgments

- Developed as part of machine learning coursework
- Built on Kaggle platform for cinema audience forecasting competition
- IITM BS September 2025 term project

---

*This project demonstrates practical implementation of time series forecasting techniques suitable for internship portfolios and academic projects.*
