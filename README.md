# Real-Time AI Traffic Management System

This project utilizes machine learning models, including **Support Vector Machine (SVM)**, **K-Nearest Neighbors (KNN)**, **Gradient Boosting Regressor (GBR)**, and **Random Forest**, to manage and optimize traffic flow in real-time. By analyzing data on vehicle count, speed, weather, and other factors, the system predicts traffic patterns and adapts traffic signals dynamically to improve traffic flow.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Architecture](#architecture)
- [Data Collection & Preprocessing](#data-collection--preprocessing)
- [Model Training](#model-training)
- [Real-Time Implementation](#real-time-implementation)
- [Results](#results)
- [Challenges and Future Work](#challenges-and-future-work)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Project Overview

Traffic congestion is a growing problem in urban areas. Traditional methods of traffic management often fail to adapt to dynamic changes in traffic patterns, leading to increased congestion and pollution. This project proposes a solution by implementing a real-time AI-based traffic management system. By utilizing machine learning models, the system can predict traffic conditions and adjust signal timings accordingly to reduce congestion.

## Features

- **Real-Time Traffic Prediction**: Predicts traffic flow based on current and historical data.
- **Adaptive Signal Control**: Adjusts traffic signal timings dynamically based on model predictions.
- **Multiple ML Models**: Utilizes SVM, KNN, GBR, and Random Forest for prediction, allowing model comparison.
- **Scalability**: Can be scaled to larger datasets and integrated with more data sources for improved accuracy.

## Architecture

1. **Data Collection**: Collects real-time data on vehicle counts, speeds, weather conditions, and special events.
2. **Data Processing**: Preprocesses data by cleaning, normalizing, and handling missing values.
3. **Model Training**: Trains four different models (SVM, KNN, GBR, and Random Forest) to predict traffic flow.
4. **Prediction & Control**: Uses the trained models to predict real-time traffic patterns and adjusts signal timings accordingly.

## Data Collection & Preprocessing

Data is gathered from traffic sensors and public sources, capturing:
- **Vehicle Count**: The number of vehicles passing through a junction.
- **Speed**: Average speed of vehicles in a particular zone.
- **Weather Conditions**: Impact of weather on traffic.
- **Special Events**: Account for increased traffic due to events, incidents, etc.

Data preprocessing steps:
- Handling missing values
- Normalizing data
- Removing outliers
- Creating additional features for model training

## Model Training

The project uses multiple machine learning models to ensure robust traffic prediction:
- **Support Vector Machine (SVM)**: Effective for high-dimensional data.
- **K-Nearest Neighbors (KNN)**: Useful for non-linear data distribution.
- **Gradient Boosting Regressor (GBR)**: Boosts weak learners to improve performance.
- **Random Forest**: Handles complex data relationships and reduces overfitting.

### Model Evaluation
The models are evaluated based on:
- Accuracy
- Prediction Speed
- Computational Efficiency
- Real-time adaptability

## Real-Time Implementation

The real-time system is integrated with traffic light controllers. It analyzes incoming data and adjusts traffic signals in real-time based on model predictions to optimize traffic flow.

## Results

- **Improved Traffic Flow**: Reduced congestion during peak hours.
- **Enhanced Travel Time**: Faster travel time due to optimized signal control.
- **Data Insights**: Useful patterns observed through time-series analysis of traffic data.

## Challenges and Future Work

### Challenges
- Data quality and missing values
- Balancing computational load with real-time requirements
- Scaling the model for larger cities with complex traffic

### Future Work
- Incorporating additional data sources such as GPS and social media.
- Testing advanced deep learning models for further accuracy.
- Deploying the system in different geographical locations.

## Technologies Used

- **Programming Languages**: Python
- **Libraries**: Pandas, NumPy, scikit-learn, Matplotlib
- **Data Visualization**: Seaborn, Matplotlib
- **Real-Time Integration**: Flask (for deployment), REST APIs for real-time data processing

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/anilsinthu114/real_time_traffic_management.git
   cd real_time_traffic_management
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python app.py
   ```

## Usage

1. **Data Collection**: Ensure traffic data is accessible through APIs or other means.
2. **Run Prediction Models**: Execute the models to generate predictions on traffic patterns.
3. **Adjust Signal Timings**: Use the output predictions to optimize traffic signals dynamically.

## License

This project is licensed under the MIT License.
