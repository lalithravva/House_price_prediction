﻿
# 🏠 House Price Prediction - California Housing Dataset

A comprehensive machine learning project comparing 9 different algorithms for predicting house prices using the California Housing dataset.

## 📊 Model Performance Comparison

| Rank | Model | R² Score | Performance |
|------|-------|----------|-------------|
| 🥇 | **Gradient Boosting** | **0.775** | Best |
| 🥈 | **Random Forest** | **0.769** | Excellent |
| 🥉 | **Neural Network (MLP)** | **0.767** | Excellent |
| 4 | Support Vector Regression | 0.719 | Very Good |
| 5 | XGBoost | 0.699 | Good |
| 6 | Linear Regression (Original) | 0.607 | Moderate |
| 6 | Ridge Regression | 0.607 | Moderate |
| 8 | Linear Regression (Sqrt Transform) | 0.581 | Moderate |
| 9 | Linear Regression (Log Transform) | 0.504 | Fair |

## 🚀 Key Features

- **9 Different ML Algorithms** implemented and compared
- **Feature Engineering** with various transformations
- **Data Preprocessing** with proper scaling
- **Comprehensive Evaluation** using R² score and MSE
- **Visual Performance Comparison** with interactive charts

## 🛠️ Technologies Used

- **Python 3.13.3**
- **Scikit-learn** - Machine Learning algorithms
- **Pandas** - Data manipulation
- **NumPy** - Numerical computing
- **Matplotlib/Seaborn** - Data visualization
- **XGBoost** - Gradient boosting framework
- **Google Colab** - Interactive development

## 📋 Algorithms Implemented

### 1. **Linear Regression Variants**
- Original features
- Log transformation
- Square root transformation

### 2. **Regularized Models**
- Ridge Regression (L2 regularization)

### 3. **Tree-Based Models**
- Random Forest
- XGBoost
- Gradient Boosting

### 4. **Advanced Models**
- Support Vector Regression (SVR) with RBF kernel
- Multi-Layer Perceptron (Neural Network)

## 🎯 Dataset Information

**California Housing Dataset:**
- **Samples:** 20,640 housing districts
- **Features:** 8 numerical features
- **Target:** Median house value
- **Source:** 1990 California census data

**Features:**
- MedInc: Median income in block group
- HouseAge: Median house age in block group
- AveRooms: Average number of rooms per household
- AveBedrms: Average number of bedrooms per household
- Population: Block group population
- AveOccup: Average number of household members
- Latitude: Block group latitude
- Longitude: Block group longitude

## 🔧 Installation & Setup

### Prerequisites
```bash
Python 3.13.3
pip or conda package manager
```

### Clone Repository
```bash
git clone https://github.com/lalithravva/House_price_prediction.git
cd House_price_prediction
```

### Install Dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost
```

### Run the Analysis
```bash
Google colab House_price_prediction.ipynb
```

## 📈 Results & Insights

### Best Performing Models:
1. **Gradient Boosting (77.5% accuracy)** - Best overall performance
2. **Random Forest (76.9% accuracy)** - Close second with good interpretability
3. **Neural Network (76.7% accuracy)** - Excellent for complex patterns

### Key Findings:
- **Ensemble methods** (Gradient Boosting, Random Forest) performed best
- **Feature scaling** was crucial for SVR and Neural Networks
- **Simple linear regression** showed limitations with complex housing data
- **Feature transformations** didn't significantly improve linear models

## 🔍 Model Details

### Gradient Boosting (Best Model)
```python
GradientBoostingRegressor(
    n_estimators=100,
    learning_rate=0.1,
    max_depth=3,
    random_state=42
)
```

### Neural Network Configuration
```python
MLPRegressor(
    hidden_layer_sizes=(100, 50),
    max_iter=500,
    random_state=42
)
```

### Support Vector Regression
```python
SVR(
    kernel='rbf',
    C=1.0,
    gamma='scale'
)
```

## 📊 Evaluation Metrics

- **R² Score:** Coefficient of determination (higher is better)
- **MSE:** Mean Squared Error (lower is better)


## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Future Improvements

- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Feature importance analysis
- [ ] Deep learning models (TensorFlow/PyTorch)
- [ ] Ensemble methods combination
- [ ] Cross-validation for all models
- [ ] Feature engineering exploration
- [ ] Model deployment with Flask/FastAPI

## 📧 Contact

**Lalith Ravva**
- GitHub: [@lalithravva](https://github.com/lalithravva)




## 🙏 Acknowledgments

- California Housing dataset from Scikit-learn
- Scikit-learn documentation and examples
- Machine Learning community for inspiration

---

⭐ **Star this repo if you found it helpful!** ⭐
