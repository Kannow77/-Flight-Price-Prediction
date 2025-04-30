# -Flight-Price-Prediction
This project uses machine learning techniques to predict flight ticket prices based on a variety of features such as airline, route, duration, stops, and journey dates. The model is trained on flight data from Indian domestic airlines.

📌 Problem Statement
Build a machine learning model that accurately predicts the price of a flight ticket using features such as departure/arrival times, duration, route, total stops, and more.

🧠 Methodology
The workflow consists of the following key steps:

🔧 Data Cleaning & Preprocessing

Handled missing values

Converted columns to appropriate data types

Extracted new datetime-based features

✨ Feature Engineering

Created new features like journey day, month, weekday, etc.

Analyzed airline market share and encoded accordingly

📏 Data Rescaling & Transformation

Applied logarithmic transformation on the target (price)

Used Box-Cox transformation for skewed features

🚫 Outlier Removal & Null Handling

Identified and removed outliers

Imputed missing values using statistical methods

🎯 Data Preparation for Modeling

One-hot encoded categorical variables

Split data into training and testing sets

📈 Model Selection & Training

Compared several regression models using cross-validation

Selected and fine-tuned the XGBoost model using RandomizedSearchCV

💾 Model Deployment

Final model saved using joblib for future inference

✅ Results
The XGBoost model achieved the best performance.

Root Mean Squared Error (RMSE): ~0.21

The model predicts flight ticket prices with good accuracy and generalization on unseen data.

📚 Dataset
Data_Train.xlsx: Training dataset

Test_set.xlsx: Test dataset

Data includes flight info such as Airline, Source, Destination, Route, Stops, Duration, and Ticket Price.
