# Alphabet Soup Charity Funding Predictor

This project aims to create a binary classifier using machine learning and neural networks to predict the success of funding applicants for Alphabet Soup, a non-profit foundation. The project involves preprocessing a dataset, building a neural network model, and optimizing it to achieve high accuracy.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Preprocessing](#data-preprocessing)
- [Model Compilation, Training, and Evaluation](#model-compilation-training-and-evaluation)
- [Model Optimization](#model-optimization)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The purpose of this analysis is to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. The dataset contains metadata about each organization, such as application type, affiliation, classification, use case, organization type, status, income amount, special considerations, funding amount requested, and whether the funding was successful.

## Data Preprocessing

- **Target Variable**: `IS_SUCCESSFUL`
- **Feature Variables**: All other columns except `EIN` and `NAME`
- **Columns Removed**: `EIN`, `NAME`
- **Encoding**: Categorical variables were encoded using `pd.get_dummies()`
- **Data Split**: Data was split into training and testing sets
- **Scaling**: Features were scaled using `StandardScaler()`

## Model Compilation, Training, and Evaluation

### Initial Model

- **Layers**: 3 (Input: 80 neurons, Hidden: 30 neurons, Output: 1 neuron)
- **Activation Functions**: ReLU for hidden layers, Sigmoid for output layer
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Epochs**: 50

### Evaluation

- **Model Accuracy**: 72.63%

## Model Optimization

### Optimized Model

- **Layers**: 4 (Input: 100 neurons, Hidden: 50 neurons, Hidden: 20 neurons, Output: 1 neuron)
- **Activation Functions**: ReLU for hidden layers, Sigmoid for output layer
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Epochs**: 100

### Evaluation

- **Optimized Model Accuracy**: [Insert optimized model accuracy]

## Results

The optimized model achieved a higher accuracy compared to the initial model. Future improvements could include further tuning of hyperparameters, trying different model architectures, or using other machine learning algorithms.

## Requirements

- Python 3.7+
- pandas
- scikit-learn
- tensorflow
- numpy

## Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/AlphabetSoupCharity.git
   cd AlphabetSoupCharity
