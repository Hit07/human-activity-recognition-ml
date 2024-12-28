# Human Activity Classification using Body Sensor Data

## 🎯 Project Highlights
- **94% Classification Accuracy** across seven distinct human activities
- **12% Accuracy Improvement** through advanced preprocessing and optimization
- **Comprehensive ML Pipeline** implementation for time-series data
- **Robust Feature Engineering** with multiple selection techniques

##  Project Overview
This project implements an advanced machine learning pipeline for human activity classification using multi-dimensional time-series data from body-worn sensors. The system processes and analyzes data from the AReM (Activity Recognition system based on Multisensor data fusion) dataset to classify seven distinct human activities.

## 📊 Technical Architecture

### Data Engineering Pipeline
```mermaid
graph LR
    A[Raw Sensor Data] --> B[Preprocessing]
    B --> C[Feature Engineering]
    C --> D[Feature Selection]
    D --> E[Model Training]
    E --> F[Evaluation]
```

### Advanced Feature Engineering
1. **Time Series Processing**
   - Dynamic segmentation up to 20 segments per series
   - Temporal pattern extraction
   - Local characteristic analysis

2. **Statistical Feature Extraction**
   ```python
   features = {
       'statistical': ['min', 'max', 'mean', 'median'],
       'distribution': ['std', 'q1', 'q3'],
       'temporal': ['sliding_windows', 'segment_analysis']
   }
   ```

3. **Dimensionality Reduction**
   - Principal Component Analysis (PCA)
   - Recursive Feature Elimination (RFE)
   - Cross-validated feature selection

## 🛠 Technical Implementation

### Class Imbalance Solutions
- **SMOTE Implementation**
  - Synthetic sample generation
  - Balanced class distribution
  - Enhanced model robustness

### Model Optimization
1. **Regularization Techniques**
   - L1 (Lasso) for feature sparsity
   - L2 (Ridge) for overfitting prevention
   - Cross-validation for hyperparameter tuning

2. **Performance Metrics**
   ```python
   metrics = {
       'accuracy': 0.94,
       'improvement': '12%',
       'cross_validation': '5-fold',
       'evaluation': ['confusion_matrix', 'ROC_curves']
   }
   ```

## 📈 Results and Impact

### Classification Performance
- **Overall Accuracy**: 94%
- **Improvement**: 12% increase from baseline
- **Cross-Validation**: Consistent performance across folds

### Feature Importance Analysis
```python
key_features = {
    'temporal': ['segment_patterns', 'window_statistics'],
    'statistical': ['quartile_ranges', 'distribution_metrics'],
    'engineered': ['custom_indicators', 'derived_features']
}
```

## Data Processing Pipeline
1. **Raw Data Handling**
   - 88 instances × 6 time series
   - 480 consecutive values per series
   - 7 distinct activity classes

2. **Feature Engineering Framework**
   - Statistical feature extraction
   - Temporal pattern analysis
   - Dimensionality optimization

3. **Model Architecture**
   - Regularized logistic regression
   - SMOTE for class balancing
   - Cross-validated parameter tuning





---
