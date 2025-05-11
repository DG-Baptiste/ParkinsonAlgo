# Parkinson's Disease Detection using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-1.5%2B-orange)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-green)

A machine learning model to detect Parkinson's disease from voice measurement data using XGBoost classifier.

## Table of Contents
- [About](#about)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## About
This project implements a machine learning pipeline to predict Parkinson's disease based on voice signal features. The model achieves **94.87% accuracy** using XGBoost classifier with feature scaling.

## Dataset
The dataset contains biomedical voice measurements from:
- 147 subjects with Parkinson's disease (positive cases)
- 48 healthy subjects (negative cases)

Dataset source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Parkinsons)

## Features
The model uses 22 voice measurement features including:
- Fundamental frequency (Fo, Fhi, Flo)
- Jitter and shimmer measurements
- Nonlinear dynamical complexity measures
- Signal fractal scaling exponent

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/parkinsons-detection.git
cd parkinsons-detection
```

2. Create and Activate Virtual Environment
python -m venv parkinson_env
source parkinson_env/bin/activate  # Linux/Mac
.\parkinson_env\Scripts\activate   # Windows

3. Install depedencies
pip install -r requirements.txt

Run the Model:
jupyter notebook parkinson_model_training.ipynb
