# Lab 8 - Neural Network Reflection

## 1. How did your predictions improve?

During training, I correctly predicted 9 out of
10 restaurant scenarios, giving me 90% accuracy.

I made a mistake on Card 9 because I predicted
DISLIKE when the actual answer was LIKE.

After adjusting the weights, I correctly
predicted Card 10. During testing, I correctly
predicted all three new scenarios, achieving
100% testing accuracy.

## 2. How did weights help you learn?

Weights helped determine how important each
input was when making a decision.

Initially, Food, Service, and Price each had
a weight of 1 token.

After my incorrect prediction on Card 9, I
increased Food's weight from 1 to 2 tokens.

This represented giving food quality more
importance in future predictions.

## 3. What would happen with more layers or inputs?

Adding more inputs, such as atmosphere,
cleanliness, and waiting time, could help
the network consider more information.

Additional layers could allow the network
to identify more complex relationships
between restaurant features.

However, a larger network could also be
more difficult to train and require more data.

## 4. How does this reflect how real AI works?

This activity demonstrates the basic idea
of learning from feedback.

The decision node made predictions,
compared them with actual answers, and
adjusted the importance of an input
after an incorrect prediction.

Real neural networks use mathematical
calculations and algorithms to adjust
many numerical weights during training.

Our classroom activity was a simplified
representation of that learning process.

## Final Results

- Training accuracy: 90% (9/10)
- Testing accuracy: 100% (3/3)
- Final Food weight: 2
- Final Service weight: 1
- Final Price weight: 1
