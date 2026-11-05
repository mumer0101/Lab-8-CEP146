# Lab 8 - Part A: Training Phase

## Objective
Train a decision node to predict whether customers
LIKE or DISLIKE a restaurant based on Food,
Service, and Price.

## Initial Weights
- Food: 1 token
- Service: 1 token
- Price: 1 token

## Training Results

| Card | Food | Service | Price | Prediction | Actual | Correct? |
|------|------|---------|-------|------------|--------|----------|
| 1 | Great | Poor | Cheap | LIKE | LIKE | Yes |
| 2 | Bad | Great | Expensive | DISLIKE | DISLIKE | Yes |
| 3 | Good | Okay | Moderate | LIKE | LIKE | Yes |
| 4 | Poor | Poor | Cheap | DISLIKE | DISLIKE | Yes |
| 5 | Excellent | Excellent | Expensive | LIKE | LIKE | Yes |
| 6 | Okay | Bad | Moderate | DISLIKE | DISLIKE | Yes |
| 7 | Great | Okay | Cheap | LIKE | LIKE | Yes |
| 8 | Poor | Excellent | Expensive | DISLIKE | DISLIKE | Yes |
| 9 | Excellent | Poor | Moderate | DISLIKE | LIKE | No |
| 10 | Okay | Okay | Expensive | DISLIKE | DISLIKE | Yes |

## Weight Adjustment Tracker

| Stage | Food | Service | Price | Adjustment |
|-------|------|---------|-------|------------|
| Initial | 1 | 1 | 1 | Starting weights |
| Cards 1-8 | 1 | 1 | 1 | All correct; no changes |
| After Card 9 | 2 | 1 | 1 | Increased Food by 1 token |
| After Card 10 | 2 | 1 | 1 | Correct; no changes |

## Training Accuracy

Correct Predictions: 9
Total Training Cards: 10

Accuracy = (9 / 10) * 100 = 90%

## Learning Observations

- The first eight predictions were correct.
- Card 9 was incorrectly predicted as DISLIKE.
- The actual result for Card 9 was LIKE because
  excellent food outweighed poor service.
- Food's weight was increased from 1 to 2 tokens.
- Card 10 was correctly predicted as DISLIKE.
- Final weights: Food 2, Service 1, Price 1.
- Training accuracy was 90%.
- This activity demonstrates how feedback can
  guide changes to the importance of inputs.
