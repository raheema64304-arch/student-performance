# student-performance
AI-powered Student Performance Analytics and Prediction dashboard built with React, TensorFlow.js, and Recharts. Analyze student academic data, visualize performance trends, train a neural-network regression model, and predict final scores directly in the browser.
# Student Performance Analytics & Prediction

A modern Student Performance Analytics and Machine Learning Prediction web application built with React, TensorFlow.js, Vite, Tailwind CSS, and Recharts.

The application analyzes student academic and lifestyle factors, visualizes performance patterns, trains a neural-network regression model directly in the browser, and predicts a student's expected final score.

> 100% client-side ML application — no backend, database, or external API is required.

## Features

### Interactive Dashboard

* Total number of students
* Average final score
* Average attendance
* Average study hours
* Highest score
* Lowest score
* Final-score distribution
* Study hours vs. final score
* Attendance vs. final score
* Previous marks vs. final score

### Student Performance Analysis

Explore relationships between academic and lifestyle factors and final performance:

* Assignment score vs. final score
* Midterm score vs. final score
* Sleep hours vs. final score
* Participation vs. final score
* Average study hours
* Average attendance
* Average previous marks
* Average assignment score
* Average midterm score
* Average final score

Interactive charts are powered by Recharts.

### Machine Learning Prediction

The application trains a neural-network regression model using TensorFlow.js.

Users can enter:

* Study hours
* Attendance
* Previous marks
* Assignment score
* Midterm score
* Participation
* Sleep hours
* Internet access
* Extracurricular activity

The trained model predicts the student's expected final score.

### Model Performance

The application evaluates the trained model using:

* MAE
* MSE
* RMSE
* R² Score

It also provides an Actual vs. Predicted visualization and allows the model performance report to be downloaded.

## Technologies Used

* React
* Vite
* Tailwind CSS
* TensorFlow.js
* Recharts
* PapaParse
* JavaScript

## Machine Learning Approach

The project uses a feed-forward neural network for regression.

### Model Architecture

```text
Input Layer
    |
    | 9 Features
    |
Dense Layer
16 neurons
ReLU activation
    |
Dense Layer
8 neurons
ReLU activation
    |
Output Layer
1 neuron
Linear activation
    |
Predicted Final Score
```

### Training Configuration

* Algorithm: Neural Network Regression
* Framework: TensorFlow.js
* Optimizer: Adam
* Learning Rate: 0.01
* Loss Function: Mean Squared Error
* Epochs: 50
* Batch Size: 16
* Training/Test Split: 80% / 20%

## Dataset

The project includes a synthetic student dataset located at:

```text
public/data/students.csv
```

The dataset contains 300 student records and the following columns:

```text
study_hours
attendance
previous_marks
assignment_score
midterm_score
participation
sleep_hours
internet_access
extracurricular
final_score
```

## Project Structure

```text
student-performance/
|
├── public/
│   └── data/
│       └── students.csv
|
├── src/
│   ├── components/
│   ├── ml/
│   ├── pages/
│   ├── services/
│   ├── utils/
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
|
├── index.html
├── package.json
├── package-lock.json
├── postcss.config.js
├── tailwind.config.js
├── vite.config.js
└── README.md
```

## Installation

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/student-performance.git
cd student-performance
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
npm run dev
```

Open the local URL provided by Vite, usually:

```text
http://localhost:5173
```

## Production Build

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## How It Works

```text
CSV Dataset
     |
Data Validation
     |
Data Preprocessing
     |
Train/Test Split
     |
Feature Normalization
     |
TensorFlow.js Neural Network
     |
Model Training
     |
Model Evaluation
     |
Data Visualization
     |
Student Performance Prediction
```

## Privacy

The application processes the dataset and performs machine learning operations directly in the browser.

No application backend or external machine learning API is required.

For real-world student information, appropriate privacy and data-protection practices should still be followed.

## Disclaimer

This project is intended for educational, demonstration, and portfolio purposes.

The included dataset is synthetic and should not be considered representative of real student populations.

Predicted scores should not be treated as definitive measurements of a student's academic ability or future performance.

## Future Improvements

* CSV upload through the user interface
* Individual student profiles
* Feature importance analysis
* Multiple machine learning algorithm comparison
* Database integration
* Authentication
* PDF report generation
* Cloud deployment
* Model hyperparameter tuning
* Cross-validation
* Training and validation loss visualization
