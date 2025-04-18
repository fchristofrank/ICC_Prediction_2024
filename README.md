# T20 Cricket Match Prediction

A machine learning model to predict the outcome of T20 cricket matches based on historical data.

## Overview

This project uses a neural network to predict the winner of T20 cricket matches based on the competing teams, toss winner, and host country. The model is trained on historical match data from international T20 matches.

## Dataset

The model uses the `MatchResults.csv` dataset containing historical T20 match data. The dataset includes:
- Team1 and Team2: The competing teams
- TossWinner: The team that won the toss
- Country: The host country where the match was played
- Match Winner: The team that won the match
- Series Name: The tournament or series name (used to identify World Cup matches)

## Features

The model considers:
- The two competing teams
- The toss winner
- The host country

These categorical features are one-hot encoded before being fed into the neural network.

## Model Architecture

The neural network has the following structure:
- Input layer: 74 nodes (matching the one-hot encoded features)
- Hidden layer 1: 64 nodes with ReLU activation
- Hidden layer 2: 32 nodes with ReLU activation
- Hidden layer 3: 16 nodes with ReLU activation
- Output layer: 19 nodes (for 19 possible winner teams) with softmax activation

The model is compiled with:
- Optimizer: Adam
- Loss function: Categorical cross-entropy
- Metric: Accuracy

## Installation

```
# Clone the repository
git clone https://github.com/yourusername/t20-prediction.git
cd t20-prediction

# Install dependencies
pip install -r requirements.txt
```

## Usage

```python
# Load and preprocess data
# Train the model
# Make predictions
```

## Requirements

- Python 3.7+
- TensorFlow
- Pandas
- Scikit-learn

## Future Improvements

- Include more features like player statistics, weather conditions
- Experiment with different model architectures
- Add visualization of prediction results
- Create a web interface for making predictions

## License

[Insert your chosen license here]

## Contact

[Your contact information]
