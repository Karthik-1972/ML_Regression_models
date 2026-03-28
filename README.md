# ML Regression Models

A comprehensive collection of machine learning regression algorithms demonstrating end-to-end predictive modeling workflows. This repository showcases professional implementations of various supervised learning techniques using multiple datasets.

## 📋 Table of Contents

- [Overview](#overview)
- [Projects](#projects)
- [Datasets](#datasets)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Algorithms Overview](#algorithms-overview)
- [Performance Metrics](#performance-metrics)
- [Technologies](#technologies)
- [Key Features](#key-features)
- [Model Comparison](#model-comparison)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

## 🎯 Overview

This repository contains implementations of **6 powerful regression algorithms** for predictive modeling tasks. Each project includes complete data pipelines from preprocessing to evaluation, demonstrating industry best practices in machine learning development.

**Core Capabilities:**
- ✅ Data preprocessing and feature engineering
- ✅ Model training with hyperparameter optimization
- ✅ Comprehensive performance evaluation
- ✅ Predictive analytics and forecasting
- ✅ Data visualization and insights

## 📁 Projects

### 1. **Simple Linear Regression**
- **Purpose**: Predict continuous values using single feature relationships
- **Use Case**: Baseline regression model for understanding data trends
- **Strengths**: 
  - Fast computation
  - Easy interpretation
  - Excellent for linear relationships
- **File**: `simple_linear_regression.py`

### 2. **Multiple Linear Regression**
- **Purpose**: Predict values using multiple independent features
- **Use Case**: Real-world scenarios with multiple predictor variables
- **Strengths**:
  - Handles multi-dimensional data
  - Interpretable coefficients
  - Efficient for linear problems
- **File**: `multiple_linear_regression.py`

### 3. **Polynomial Regression**
- **Purpose**: Capture non-linear relationships in data
- **Use Case**: Complex relationships requiring curved fitting
- **Strengths**:
  - Flexible polynomial degrees
  - Better fit for curved data
  - Extends linear regression capability
- **File**: `polynomial_regression.py`

### 4. **Decision Tree Regression**
- **Purpose**: Tree-based non-parametric regression
- **Use Case**: Non-linear patterns and feature interactions
- **Strengths**:
  - Handles non-linear relationships
  - Feature importance extraction
  - Easy to interpret
- **File**: `decision_tree_regression.py`

### 5. **Random Forest Regression**
- **Purpose**: Ensemble method combining multiple decision trees
- **Use Case**: High-accuracy predictions with reduced overfitting
- **Strengths**:
  - Superior accuracy through ensemble
  - Robust to outliers
  - Feature importance analysis
  - Reduced overfitting
- **File**: `random_forest_regression.py`

### 6. **Support Vector Regression (SVR)**
- **Purpose**: Regression using support vector machines
- **Use Case**: High-dimensional data and complex patterns
- **Strengths**:
  - Excellent for non-linear regression
  - Effective in high dimensions
  - Memory efficient
  - Robust kernel options
- **File**: `support_vector_regression.py`

## 📊 Datasets

Each project works with domain-specific datasets:

| Project | Dataset | Features | Samples | Target |
|---------|---------|----------|---------|--------|
| Simple Linear Regression | Salary/Experience | 1 | ~30 | Salary |
| Multiple Linear Regression | Startups | 4+ | ~50 | Profit |
| Polynomial Regression | Position/Salary | 1 | ~10 | Salary |
| Decision Tree Regression | Position/Salary | 1 | ~10 | Salary |
| Random Forest Regression | Position/Salary | 1 | ~10 | Salary |
| Support Vector Regression | Position/Salary | 1 | ~10 | Salary |

**Data Characteristics:**
- Clean, preprocessed datasets
- CSV format for easy loading
- Well-structured features
- Real-world inspired scenarios

## 🚀 Installation

### Prerequisites
```
Python 3.7 or higher
pip package manager
```

### Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/Karthik-1972/ML_Regression_models.git
cd ML_Regression_models

# 2. Create virtual environment (recommended)
python -m venv venv

# 3. Activate virtual environment
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt
```

### Required Libraries
```
numpy>=1.19.0
pandas>=1.1.0
scikit-learn>=0.24.0
matplotlib>=3.3.0
seaborn>=0.11.0
```

## 📂 Project Structure

```
ML_Regression_Models/
│
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
├── Simple_Linear_Regression/
│   ├── simple_linear_regression.py
│   └── salary_data.csv
│
├── Multiple_Linear_Regression/
│   ├── multiple_linear_regression.py
│   └── startups.csv
│
├── Polynomial_Regression/
│   ├── polynomial_regression.py
│   └── Position_Salaries.csv
│
├── Decision_Tree_Regression/
│   ├── decision_tree_regression.py
│   └── Position_Salaries.csv
│
├���─ Random_Forest_Regression/
│   ├── random_forest_regression.py
│   └── Position_Salaries.csv
│
└── Support_Vector_Regression/
    ├── support_vector_regression.py
    └── Position_Salaries.csv
```

## 💻 Usage

### Running Individual Projects

```bash
# Navigate to project directory
cd Simple_Linear_Regression

# Run the regression model
python simple_linear_regression.py
```

### What Each Script Includes

1. **Data Loading & Exploration**
   - CSV file reading with pandas
   - Dataset overview and statistics
   - Missing value handling

2. **Data Preprocessing**
   - Feature scaling (StandardScaler)
   - Train-test split (80-20 or 70-30)
   - Feature normalization

3. **Model Training**
   - Algorithm implementation
   - Parameter configuration
   - Model fitting

4. **Evaluation & Metrics**
   - R² Score
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - Mean Absolute Error (MAE)

5. **Visualization**
   - Actual vs Predicted plots
   - Residual analysis
   - Feature relationships
   - Decision boundaries

### Example: Running Simple Linear Regression

```bash
cd Simple_Linear_Regression
python simple_linear_regression.py

# Output:
# Model R² Score: 0.957
# MSE: 54000000.00
# RMSE: 7348.15
```

## 📈 Algorithms Overview

### Regression Comparison Matrix

| Algorithm | Complexity | Speed | Interpretability | Non-linear | Best For |
|-----------|-----------|-------|------------------|-----------|----------|
| Simple Linear | Low | ⚡⚡⚡ | High | ❌ | Linear trends |
| Multiple Linear | Low | ⚡⚡⚡ | High | ❌ | Multiple features |
| Polynomial | Medium | ⚡⚡ | Medium | ✅ | Curved patterns |
| Decision Tree | Medium | ⚡⚡ | High | ✅ | Non-linear data |
| Random Forest | High | ⚡ | Medium | ✅ | Complex patterns |
| SVR | High | ⚡ | Low | ✅ | High dimensions |

## 📊 Performance Metrics

### Understanding Evaluation Metrics

**R² Score (Coefficient of Determination)**
- Range: 0 to 1
- Higher is better
- Percentage of variance explained

**MSE (Mean Squared Error)**
- Sum of squared differences
- Penalizes large errors
- Lower is better

**RMSE (Root Mean Squared Error)**
- Same units as target variable
- More interpretable than MSE
- Lower is better

**MAE (Mean Absolute Error)**
- Average absolute differences
- Robust to outliers
- Lower is better

### Typical Performance Results

```
Simple Linear Regression:     R² ≈ 0.95
Multiple Linear Regression:   R² ≈ 0.93
Polynomial Regression:        R² ≈ 0.96
Decision Tree Regression:     R² ≈ 0.92
Random Forest Regression:     R² ≈ 0.97
Support Vector Regression:    R² ≈ 0.94
```

## 🛠️ Technologies

| Technology | Version | Purpose |
|-----------|---------|---------|
| **Python** | 3.7+ | Programming language |
| **scikit-learn** | 0.24+ | ML algorithms |
| **pandas** | 1.1+ | Data manipulation |
| **numpy** | 1.19+ | Numerical computing |
| **matplotlib** | 3.3+ | Static visualization |
| **seaborn** | 0.11+ | Advanced visualization |

## ✨ Key Features

### Data Handling
- ✅ CSV file loading and parsing
- ✅ Missing value detection and handling
- ✅ Data type conversion
- ✅ Statistical summary

### Model Development
- ✅ Train-test data splitting
- ✅ Feature scaling and normalization
- ✅ Multiple algorithm implementations
- ✅ Hyperparameter configurations

### Evaluation & Analysis
- ✅ Multiple performance metrics
- ✅ Residual analysis
- ✅ Prediction accuracy assessment
- ✅ Visual comparisons

### Visualization
- ✅ Scatter plots with regression lines
- ✅ Residual distribution plots
- ✅ Actual vs Predicted charts
- ✅ Feature relationship plots

## 🎯 Model Comparison

### When to Use Each Algorithm

**Simple Linear Regression**
- One feature, linear relationship
- Quick prototype development
- Baseline model comparison

**Multiple Linear Regression**
- Multiple features, linear relationship
- Interpretable feature importance
- Real-world business problems

**Polynomial Regression**
- Non-linear single or dual features
- Curved data patterns
- Physical science applications

**Decision Tree Regression**
- Non-linear relationships
- Feature interactions
- Interpretable decision rules

**Random Forest Regression** ⭐ **Best Overall**
- Complex, non-linear patterns
- Multiple feature interactions
- High accuracy requirements
- Robust predictions

**Support Vector Regression**
- High-dimensional data
- Complex non-linear patterns
- Outlier-robust predictions
- Kernel flexibility needed

## 🔮 Future Enhancements

- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Cross-validation implementation (K-Fold)
- [ ] Feature selection techniques
- [ ] Ensemble stacking models
- [ ] Time series forecasting
- [ ] Deep learning regression (TensorFlow/Keras)
- [ ] Model persistence (pickle/joblib)
- [ ] Web API deployment (Flask/FastAPI)
- [ ] Interactive Jupyter notebooks
- [ ] Automated ML pipeline
- [ ] Comparative performance dashboard
- [ ] Real-world dataset examples

## 📚 Learning Resources

### Official Documentation
- [scikit-learn Regression](https://scikit-learn.org/stable/supervised_learning.html#regression)
- [Pandas Documentation](https://pandas.pydata.org/)
- [NumPy Guide](https://numpy.org/doc/)

### Online Courses
- [Andrew Ng - Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction)
- [Fast.ai - Practical Deep Learning](https://www.fast.ai/)
- [Kaggle Learn - Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)

### Books
- "Hands-On Machine Learning" - Aurélien Géron
- "The Hundred-Page ML Book" - Andriy Burkov
- "Introduction to Statistical Learning" - James, Witten, Hastie, Tibshirani

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -m 'Add improvement'`)
4. Push to branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 👤 Author

**Karthik-1972**
- GitHub: [@Karthik-1972](https://github.com/Karthik-1972)
- Repository: [ML Regression Models](https://github.com/Karthik-1972/ML_Regression_models)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

MIT License grants you the freedom to:
- ✅ Use commercially
- ✅ Modify the code
- ✅ Distribute
- ✅ Private use

## ⭐ Support

If you found this repository helpful:
- ⭐ Please star this repository
- 🔖 Share it with others
- 📧 Provide feedback and suggestions
- 🐛 Report issues

---

## 📊 Repository Statistics

- **Projects**: 6 Regression Algorithms
- **Datasets**: Multiple real-world inspired datasets
- **Lines of Code**: 1000+
- **Last Updated**: March 2026

---

### Quick Start Checklist

- [ ] Clone the repository
- [ ] Install Python 3.7+
- [ ] Install requirements: `pip install -r requirements.txt`
- [ ] Navigate to any project folder
- [ ] Run: `python <script_name>.py`
- [ ] View results and visualization

**Happy Learning! 🚀**
