# Employee Absenteeism Prediction System

A machine learning project that predicts employee absenteeism using logistic regression with 85% accuracy. The system includes data preprocessing, feature engineering, and a production-ready deployment module.

##  Project Overview

This project analyzes employee data to predict absenteeism patterns, helping HR departments make data-driven decisions. The model identifies key factors contributing to employee absence and provides probability predictions for new employee data.

##  Features

- **Predictive Modeling**: Logistic regression model with 85% accuracy
- **Custom Data Pipeline**: Automated preprocessing with feature engineering
- **Production Ready**: Modular Python class for easy deployment
- **Statistical Analysis**: Comprehensive data analysis and insights
- **Scalable Architecture**: Easy to retrain and update with new data

## 🛠 Technologies Used

- **Python 3.x**
- **scikit-learn** - Machine learning algorithms
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **pickle** - Model serialization
- **Jupyter Notebook** - Development and analysis

## 📊 Dataset Features

The model uses the following features to predict absenteeism:
- Reason for absence (categorized into 4 types)
- Transportation expense
- Distance to work
- Age
- Body mass index
- Education level
- Number of children
- Pet ownership
- Month and day patterns

## 🔧 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/employee-absenteeism-prediction.git
cd employee-absenteeism-prediction
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook for analysis:
```bash
jupyter notebook Employee_Absenteeism_Analysis.ipynb
```

## 💻 Usage

### For Predictions:
```python
from absenteeism_module import absenteeism_model

# Initialize the model
model = absenteeism_model('model', 'scaler')

# Load and preprocess new data
model.load_and_clean_data('new_data.csv')

# Get predictions
predictions = model.predicted_outputs()
print(predictions)
```

### For Training:
Run the Jupyter notebook `Employee_Absenteeism_Analysis.ipynb` to:
- Explore the dataset
- Perform feature engineering
- Train the model
- Evaluate performance

## 📁 Project Structure

```
employee-absenteeism-prediction/
│
├── data/
│   ├── raw/
│   │   └── absenteeism_data.csv
│   └── processed/
│       └── cleaned_data.csv
│
├── notebooks/
│   └── Employee_Absenteeism_Analysis.ipynb
│
├── src/
│   └── absenteeism_module.py
│
├── models/
│   ├── model
│   └── scaler
│
├── requirements.txt
├── README.md
└── .gitignore
```

## 📈 Model Performance

- **Accuracy**: 85%
- **Precision**: 0.82
- **Recall**: 0.79
- **F1-Score**: 0.80

## 🔍 Key Insights

1. **Medical reasons** are the strongest predictors of absenteeism
2. **Transportation costs** significantly impact absence patterns
3. **Seasonal trends** show higher absenteeism in winter months
4. **Distance to work** correlates with absence frequency

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

##  Author

**Vedika Kute**
- LinkedIn: [vedika-kute-602b22282](https://linkedin.com/in/vedika-kute-602b22282)
- Email: vedikakute06@gmail.com

##  Acknowledgments

- Inspiration from real-world HR analytics challenges
- Thanks to the data science community for best practices
