# Lab 8 - Part B: Testing Phase

## Objective

Test the trained decision node on three new
restaurant scenarios without changing the weights.

## Final Trained Weights

- Food: 2 tokens
- Service: 1 token
- Price: 1 token

## Testing Results

| Card | Food | Service | Price | Prediction | Actual | Correct? |
|------|------|---------|-------|------------|--------|----------|
| 11 | Good | Excellent | Cheap | LIKE | LIKE | Yes |
| 12 | Bad | Bad | Expensive | DISLIKE | DISLIKE | Yes |
| 13 | Excellent | Great | Moderate | LIKE | LIKE | Yes |

## Testing Accuracy

Correct Predictions: 3
Total Testing Cards: 3

Accuracy = (3 / 3) * 100 = 100%

## Training vs Testing Comparison

| Phase | Correct | Total | Accuracy |
|-------|---------|-------|----------|
| Training | 9 | 10 | 90% |
| Testing | 3 | 3 | 100% |

## Observations

- The decision node correctly predicted all
  three new testing scenarios.
- The weights remained unchanged during testing.
- Food had the highest weight at 2 tokens.
- Training accuracy was 90%.
- Testing accuracy was 100%.
- The testing score was 10 percentage points
  higher than the training score.
- Three testing scenarios are not enough to
  prove the model will always be accurate.
- More test examples would provide a more
  reliable measure of performance.

## Conclusion

The trained decision node correctly classified
all three unseen restaurant scenarios.

The activity demonstrates how adjusting input
weights after feedback can help a decision
system make predictions on new examples.
