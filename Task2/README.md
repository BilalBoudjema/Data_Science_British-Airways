# British Airways Customer Booking Prediction

## 📋 Project Overview

This project implements a machine learning model to predict customer booking completion behavior for British Airways. The analysis uses a Random Forest classifier to identify key factors that influence whether customers complete their bookings.

## 🎯 Objectives

1. **Explore and prepare the dataset** - Understand customer booking patterns and prepare data for modeling
2. **Train a machine learning model** - Build an interpretable Random Forest classifier
3. **Evaluate model performance** - Use cross-validation and comprehensive metrics
4. **Visualize insights** - Create interactive visualizations and professional presentation

## 📊 Features Used

### Numeric Features
- `num_passengers` - Number of passengers traveling
- `purchase_lead` - Days between booking and travel date
- `length_of_stay` - Days spent at destination
- `flight_hour` - Hour of flight departure
- `flight_day` - Day of week (1=Monday, 7=Sunday)
- `flight_duration` - Total flight duration in hours
- `is_weekend` - Derived feature (Saturday/Sunday = 1, else = 0)

### Categorical Features
- `sales_channel` - Booking channel
- `trip_type` - Round Trip, One Way, or Circle Trip
- `route` - Origin → Destination
- `booking_origin` - Country of booking
- `wants_extra_baggage` - Extra baggage preference
- `wants_preferred_seat` - Seat preference
- `wants_in_flight_meals` - Meal preference

### Target Variable
- `booking_complete` - Whether the booking was completed (1) or not (0)

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn python-pptx
```

**Optional (for high-quality image export):**
```bash
pip install kaleido
```

### Running the Analysis

1. Open `Getting Started.ipynb` in Jupyter
2. Run all cells sequentially from top to bottom
3. Interactive visualizations will appear inline
4. Final PowerPoint presentation will be generated in `outputs/` folder

## 📈 Model Performance

The Random Forest classifier is evaluated using:
- **5-Fold Cross-Validation** with stratified splitting
- **Metrics**: ROC AUC, Accuracy, Precision, Recall, F1 Score
- **Test Set Evaluation** with comprehensive classification report

## 📦 Output Files

All outputs are saved in the `outputs/` directory:

- **`BA_Customer_Booking_Analysis.pptx`** - Professional presentation with:
  - Cross-validation metrics with standard deviations
  - Test set performance
  - Model configuration details
  - Top 20 feature importances
  - ROC curve (if kaleido available)
  
- **`feature_importance.png`** - High-resolution feature importance chart
- **`roc_curve.png`** - ROC curve visualization (if kaleido available)

## 🎨 Visualizations

The notebook includes interactive Plotly visualizations:

1. **Target Distribution** - Pie chart of booking completion rates
2. **Sales Channel Analysis** - Bookings by channel
3. **Feature Distributions** - Histograms of numeric features
4. **Purchase Lead Analysis** - Box plots by booking status
5. **Flight Duration Analysis** - Violin plots by booking status
6. **Correlation Heatmap** - Feature correlations
7. **ROC Curve** - Model performance visualization
8. **Confusion Matrix** - Prediction accuracy breakdown
9. **Feature Importances** - Top contributing features

## 🔧 Technical Details

### Model Configuration
- **Algorithm**: Random Forest Classifier
- **Number of Trees**: 300
- **Max Depth**: None (trees grow until pure)
- **Min Samples Split**: 2
- **Min Samples Leaf**: 1
- **Random State**: 42 (reproducible results)

### Data Processing
- **Encoding**: OneHotEncoder for categorical variables
- **Feature Engineering**: Created `is_weekend` derived feature
- **Split**: 80% training, 20% test set (stratified)
- **Cross-Validation**: 5-fold stratified K-fold

## 📝 Notes

- The notebook uses fallback mechanisms for image export if `kaleido` is not installed
- All visualizations are interactive when viewed in Jupyter
- The PowerPoint presentation is optimized for professional presentation
- Random seed is set for reproducibility

## 🎓 Learning Outcomes

This project demonstrates:
- End-to-end machine learning workflow
- Feature engineering and data preprocessing
- Model training and evaluation best practices
- Interactive data visualization with Plotly
- Professional presentation creation with python-pptx
- Robust error handling and fallback mechanisms

## 📧 Contact

For questions or feedback about this analysis, please refer to the project repository.

---

**Generated**: October 2025  
**Framework**: scikit-learn  
**Visualization**: Plotly, Matplotlib, Seaborn  
**Presentation**: python-pptx

