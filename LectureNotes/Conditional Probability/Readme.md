### LECTURE ON:- 
### Conditional Probability

Conditional probability is the probability of an event occurring given that
another event has already occurred. In other words, it quantifies the likelihood
of an event A happening, under the condition that event B is known to have
occurred. The conditional probability of A given B is denoted as P (A|B), and
it is calculated using the formula: 

P (A|B) = P (A ∩ B)/P (B)
where:
- P (A ∩ B) is the probability that both events A and B occur (i.e., the
intersection of A and B). - P (B) is the probability that event B occurs.

#### Dice Experiment

Let’s consider a dice experiment. We roll a standard 6-sided die and define:

- **Event A**: The die shows an even number (2, 4, or 6).
- **Event B**: The die shows a number greater than 3 (4, 5, or 6).

#### Step-by-Step Calculation

1. **Sample Space**: \(S = \{1, 2, 3, 4, 5, 6\}\)
2. **Probability of Event B**: \(P(B) = \frac{3}{6} = 0.5\)
3. **Intersection of Events A and B**: \(P(A \cap B) = \frac{2}{6} = 0.3333\)
4. **Conditional Probability Formula**:

\(P(A | B) = \frac{P(A \cap B)}{P(B)} = \frac{2/6}{3/6} = \frac{2}{3}\)

#### Python Code Example

```python
import numpy as np

# Define the sample space and events
sample_space = [1, 2, 3, 4, 5, 6]
A = [2, 4, 6]  # Even numbers
B = [4, 5, 6]  # Numbers greater than 3

# Calculate intersection
intersection_A_B = list(set(A) & set(B))

# Probabilities
P_B = len(B) / len(sample_space)
P_A_intersection_B = len(intersection_A_B) / len(sample_space)

# Conditional probability
P_A_given_B = P_A_intersection_B / P_B

print("P(A | B):", P_A_given_B)
```

**Output:**

```
P(A | B): 0.6666666666666666
```

![Conditional Probability Example](./images/conditional_probability_example.jpg)  



[Conditional Probability video 1](https://drive.google.com/file/d/1w9gS_nut-K0EZZ5SGK8UsKN_qbwcPaBN/view?usp=drive_link) 

[Conditional Probability video 2](https://drive.google.com/file/d/1J6ZlfSrlUJupLeQZTIPitkgY0OLLZeeK/view?usp=drive_link) 
