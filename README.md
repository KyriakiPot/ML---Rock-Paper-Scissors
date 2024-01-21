# ML---Rock-Paper-Scissors Agent

# Project Overview
The goal of this project is to develop an intelligent agent capable of playing the Rock-Scissors-Paper game. The agent will be trained using a dataset containing images for each movement: Rock, Scissors, and Paper. The objective is for the agent to learn and make optimal choices based on the images it observes.

# Dataset
The project utilizes the Rock-Scissors-Paper dataset, available at Kaggle (https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors). This dataset comprises 700+ images for each movement.

# Agent Rules
The agent will bet €1 against a Random Agent for a total of N rounds.
If the agent wins, it receives a €2 refund; in a tie, it receives €1; otherwise, it loses €1.
The Random Agent applies various transformations to the images with probabilities p1 and p2, making the game more challenging.

# Random Agent Transformations
Vertical Flip with probability p1 = 0.5.
Horizontal Flip with probability p2 = 0.5.
Addition of random noise (white noise) to each pixel with mean value 0 and standard deviation 5% of the maximum pixel value.

# Project Steps

1. Data Preparation:
Assign moves (Rock, Scissors, Paper) to numerical labels (0, 1, 2).
Divide the dataset into train-test sets, allocating a percentage for testing seperating equally the labels.

2. Image Processing:
Randomly select an image from the dataset.

3. Apply preprocessing steps:
Vertical Flip with probability p1.
Horizontal Flip with probability p2.
Add noise with specified parameters.
Implement any other image processing methods to increase the game's difficulty.

4. Agent Action:
Send the preprocessed image to the agent.
The agent reads the image and chooses the optimal action.

5. Game Profit Maximization:
The goal is to maximize profit.
Track the total profit in each round and plot it at the end of the game.

6. Testing Accuracy:
Evaluate the accuracy of the agent/model on images outside the dataset.
Rescale external images to the same size for testing.
Dimensionality Reduction:

7. Resize images to a smaller size.
Convert images to black and white to reduce total pixels.
Normalize images to a 0-1 scale.

8. Environment:
Build a simple environment with loops and functions to create the game interface.

9. Supervised Learning:
Train a machine learning model (e.g., Logistic Regression, Random Forest, Convolutional Neural Network) to recognize images.
After recognizing the image, use a rule-based approach to choose the best action.
After training different ML models, the model that was used is Ensemble CNN.

# Running the Project
To run the project, follow these steps:

Download the Rock-Scissors-Paper dataset from Kaggle.
Implement the necessary image processing and agent logic.
Train the machine learning model.
Build the game environment.
Execute the game and observe the agent's performance.
Note: Adjust parameters, such as the percentage of the test set, probabilities of flips, and image processing methods, based on experimentation and desired difficulty levels.

Feel free to experiment with different machine learning models and image processing techniques to enhance the agent's capabilities.
