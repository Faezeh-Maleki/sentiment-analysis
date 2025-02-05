1) # Sentiment Analysis on Amazon Baby Reviews

This project aims to develop a sentiment analysis system to classify reviews from the Amazon Baby dataset into positive, negative, and neutral sentiments using Logistic Regression.

## Project Overview

Sentiment analysis is a subset of classification methods used to determine the sentiment expressed in a piece of text. In this project, we classify reviews based on the following criteria:
- **Positive**: Ratings of 4 or 5 stars
- **Negative**: Ratings of 1 or 2 stars
- **Neutral**: Ratings of 3 stars

## Dataset

The dataset used in this project is the `amazon_baby.csv` file, which contains reviews and ratings of baby products on Amazon.

## Steps

1. **Data Loading**: Load the dataset from a CSV file.
2. **Data Preprocessing**: Clean the text data by converting it to lowercase and removing non-alphabetic characters.
3. **Sentiment Labeling**: Define sentiment labels based on ratings.
4. **Feature Extraction**: Use `TfidfVectorizer` to convert text data into numerical features.
5. **Model Training**: Train a Logistic Regression model on the training data.
6. **Model Evaluation**: Evaluate the model using a classification report, accuracy score, and confusion matrix.
7. **Visualization**: Plot confusion matrix, distribution of sentiments, and feature importance.

## Results

- **Accuracy**: 84.8%
- **Confusion Matrix**: Shows the performance of the model in predicting different sentiment categories.
- **Sentiment Distribution**: Displays the number of reviews in each sentiment category.
- **Feature Importance**: Highlights the most influential words for positive and negative sentiments.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


2) # Q-learning with CartPole Environment

This project implements a Q-learning algorithm to train an agent to balance a pole on a cart using the CartPole-v1 environment from OpenAI Gym.

## Project Overview

Q-learning is a model-free reinforcement learning algorithm used to find the optimal action-selection policy for any given finite Markov decision process. In this project, we use Q-learning to train an agent to balance a pole on a cart.

## Environment

The environment used is `CartPole-v1` from OpenAI Gym. The goal is to keep the pole balanced by applying forces to the cart.

## Q-learning Parameters

- **Number of Episodes**: 1000
- **Maximum Steps per Episode**: 100
- **Learning Rate (Alpha)**: 0.1
- **Discount Factor (Gamma)**: 0.99
- **Exploration Rate (Epsilon)**: Starts at 1.0 and decays to 0.01
- **Epsilon Decay Rate**: 0.995

## State Space Discretization

The continuous state space is discretized into bins:
- **Cart Position**: 1 bin
- **Cart Velocity**: 1 bin
- **Pole Angle**: 6 bins
- **Pole Velocity at Tip**: 12 bins

## Q-learning Algorithm

1. **Initialize Q-table**: The Q-table is initialized to zeros.
2. **Discretize State**: Continuous states are discretized into discrete bins.
3. **Choose Action**: Actions are chosen using an epsilon-greedy policy.
4. **Update Q-value**: Q-values are updated using the Q-learning formula.
5. **Decay Epsilon**: Epsilon is decayed after each episode to reduce exploration over time.

## Results

- **Training Progress**: The total reward per episode is printed every 100 episodes.
- **Q-table Visualization**: A heatmap of the Q-table for action 0 is plotted.

  
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

