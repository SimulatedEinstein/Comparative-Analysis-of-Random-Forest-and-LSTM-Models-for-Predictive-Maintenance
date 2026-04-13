Predictive Maintenance of Machines Using Machine Learning

A machine learning and deep learning based predictive maintenance framework for estimating the Remaining Useful Life (RUL) of industrial machines using the NASA CMAPSS turbofan engine degradation dataset.

Overview

This project predicts how many operational cycles remain before an engine fails by analyzing sensor and operational data. It compares traditional machine learning with sequence-based deep learning to evaluate which method provides better predictive performance for Remaining Useful Life estimation.

Features
Remaining Useful Life (RUL) prediction using sensor data
Random Forest based regression model
LSTM based deep learning model for temporal sequence learning
Feature importance analysis for sensor contribution
Model comparison using RMSE and R² Score
GPU-accelerated LSTM training using TensorFlow
Dataset

Source: NASA CMAPSS Turbofan Engine Dataset

The dataset contains:

Engine ID
Operational Cycles
3 Operational Settings
21 Sensor Measurements
Ground Truth RUL for Test Data
Methodology
Data Preprocessing
Assigned structured column names
Computed Remaining Useful Life (RUL)
Applied RUL clipping for stable learning
Normalized features using Min-Max Scaling
Random Forest Model
Trained baseline regression model
Generated feature importance rankings
Predicted engine-level RUL
LSTM Model
Converted data into sequential time windows
Built stacked LSTM architecture
Trained using GPU acceleration
Predicted RUL from degradation sequences
Evaluation Metrics
RMSE (Root Mean Square Error)
R² Score

Lower RMSE and higher R² indicate better predictive performance.

Results
Model	RMSE
Random Forest :  18.0106284054395
LSTM	: 16.934802526781755

Technologies Used
Python
Pandas
NumPy
Scikit-learn
TensorFlow / Keras
Matplotlib
Google Colab
Future Scope
Hyperparameter Optimization
Feature Selection / Sensor Reduction
Real-Time Deployment with IoT Sensors
Web Dashboard Integration
Conclusion

The project demonstrates that LSTM models outperform traditional Random Forest models for Remaining Useful Life estimation due to their ability to learn temporal degradation patterns from sequential sensor data.
