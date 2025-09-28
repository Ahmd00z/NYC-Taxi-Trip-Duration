# 🚖 NYC Taxi Trip Duration Prediction

Welcome to the **NYC Taxi Trip Duration Prediction** project! This repository implements a robust machine learning pipeline designed to predict taxi trip durations in New York City. By leveraging various data features and advanced modeling techniques, this project aims to provide accurate predictions that can assist in enhancing urban transportation systems.

---

## 📌 Overview

This repository contains a complete machine learning workflow that encompasses data preprocessing, feature engineering, model training, and evaluation. The results are persisted for reproducibility, ensuring that the model can be retrained and evaluated consistently.

### Key Highlights:

- **🚀 End-to-End ML Pipeline:**  
  From raw data ingestion to actionable predictions, this project covers every aspect of the machine learning lifecycle.

- **🧮 Feature Engineering:**  
  Utilizes a variety of features including distances, directions, datetime features, and seasonal bins to enrich the dataset and improve model accuracy.

- **🔧 Data Preprocessing:**  
  Implements log transformations, scaling, and categorical encoding to prepare the data for optimal model performance.

- **📈 Models Used:**  
  Primarily employs Ridge Regression with polynomial features, where the degree of the polynomial is auto-selected based on the training data.

- **📝 Evaluation Metrics:**  
  Evaluates model performance using Root Mean Squared Error (RMSE) and R² to ensure accuracy and reliability of predictions.

- **💾 Persistence:**  
  Trained models are stored along with their metadata using `joblib`, allowing for easy loading and reuse.

---

## 📂 Project Structure

The project is organized as follows:

NYC-Taxi-Trip-Duration/
│
├── data_sample/ # Sample data for testing
├── full_data/ # Complete dataset
├── models/ # Saved models (.pkl)
├── saving_data/ # Processed data storage
│
├── data_evaluation.py # Model evaluation scripts
├── data_preparing.py # Data preparation and feature engineering
├── data_preprocessing.py # Data cleaning and preprocessing
├── data_training.py # Model training pipeline
├── feature_fragmenting.py # Feature selection and engineering utilities
├── loading_model.py # Model loading utilities
├── loading_test.py # Model testing and validation
├── requirements.txt # Dependencies
└── README.md # Documentation

basic


---

## ⚙️ Installation

To get started with the project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/AhmedYasser06/NYC-Taxi-Trip-Duration.git
cd NYC-Taxi-Trip-Duration
pip install -r requirements.txt
🚀 Usage
1️⃣ Train the Model
To train the model, execute the following command:

bash

python data_training.py
This command trains the Ridge Regression model with polynomial features, automatically selecting the optimal degree. The trained model, along with preprocessors and metadata, will be saved in the models/ directory.

2️⃣ Evaluate on Validation / Test Sets
To evaluate the model's performance, use:

bash

python loading_test.py
This script loads the saved model, prepares the data through feature engineering and preprocessing, and evaluates the model using RMSE and R² metrics.

📊 Example Results
Upon evaluation, you can expect results similar to the following:

Train RMSE: 0.4373 | R²: 0.6972
Validation RMSE: 0.4424 | R²: 0.6942
Test RMSE: 0.4451 | R²: 0.6920
These metrics indicate the accuracy and reliability of the model in predicting taxi trip durations.

📦 Dependencies
The main libraries used in this project include:

numpy
pandas
scikit-learn
joblib
For a complete list of dependencies, please refer to the requirements.txt file.

🤝 Contributing
Contributions to enhance this project are welcome! If you have suggestions for improvements, bug fixes, or new features, please feel free to open an issue or submit a pull request.

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

Thank you for exploring the NYC Taxi Trip Duration Prediction project! Your feedback and contributions are greatly appreciated. Let's improve urban transportation together! 🚖



You can copy and paste this code directly into your `README.md` file. Let me know if you need any fur
