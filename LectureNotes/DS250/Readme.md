Lecture-1 Notes
---

## Introduction

### Notes on Plotting Histograms and Heatmaps

---

### 1. Histograms

A histogram is a graphical representation of the distribution of data. It divides the entire range of values into intervals (called bins) and counts the number of data points that fall into each bin.

#### Mathematical Definition

Let \(x_1, x_2, \dots, x_n\) be the data points. Divide the range of data into \(k\) bins, where:

The bin width \(w\) is:

\(w = \frac{\text{max}(x) - \text{min}(x)}{k}\)

For each bin \(i\):

\(b_i < x < b_{i+1}\)

Here, \(b_i\) and \(b_{i+1}\) are the edges of the \(i\)-th bin.

#### Steps to Plot a Histogram

1. Choose the number of bins: Use the rule of thumb or algorithms like Sturges' formula:

   \(k = [log_2(n) + 1 ]

2. Plot the frequencies using bar heights.

#### Python Code Example

[View Histogram Code Example](https://gist.github.com/your-link-here)

```python
import matplotlib.pyplot as plt
import numpy as np

# Sample data
data = np.random.normal(0, 1, 1000)

# Plotting the histogram
plt.hist(data, bins=30, edgecolor='black', alpha=0.7)
plt.title('Histogram')
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.show()
```

---

#### Activity on Histograms

**Part A: Word Length Histogram**

**Objective:** Create a histogram that represents the frequency of words based on their length in any paragraph from your preferred book.

**Steps:**

1. Choose a paragraph from your favorite book.
2. Count the number of letters in each word.
3. Group words by their lengths (e.g., words with 1 letter, 2 letters, etc.).
4. Plot the histogram:
   - **X-axis:** Word lengths.
   - **Y-axis:** Frequency of words of each length.

**Part B: Starting Letter Histogram**

**Objective:** Create a histogram to analyze the frequency of words starting with each letter of the alphabet.

**Steps:**

1. Use the same paragraph as in Part A.
2. Count how many words start with each letter (A-Z).
3. Plot the histogram:
   - **X-axis:** Starting letters (A-Z).
   - **Y-axis:** Frequency of words starting with each letter.
![Word Length Distribution](./word_length.jpg)
![Starting Letter Distribution](./starting_letter_frequency.jpg)

**Part C: Forecasting with Weight and Height Functions**

**Objective:** Plot histograms using functions for weight and height over time.

**Functions:**

\(w(t) = t + 2, \ h(t) = 3t + 5\)

Where (t\) represents time (from the beginning to today).

---

### 2. Heatmaps

A heatmap is a data visualization technique used to represent data in a matrix format with varying intensities of color to show magnitude.

#### Mathematical Definition

For a matrix \(A\) with elements \(a_{ij}\), a heatmap assigns a color \(c_{ij}\) to each cell based on a colormap \(C\):

\(c_{ij} = C(a_{ij})\)

#### Steps to Create a Heatmap

1. Normalize the data: Rescale values if needed.
2. Choose a colormap: Maps numerical values to colors.
3. Visualize the data as a grid.

#### Python Code Example

[View Heatmap Code Example](https://gist.github.com/your-link-here)

```python
import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt

# Sample data
data = np.random.rand(10, 10)

# Plotting the heatmap
sns.heatmap(data, annot=True, cmap='viridis')
plt.title('Heatmap')
plt.show()
```

---

### 3. Vectors and the Tug of War Problem

#### Vectors

A vector is a quantity that has both magnitude and direction. For example, a vector \(\vec{A}\) in 2D space:

\(\vec{A} = A_x \hat{i} + A_y \hat{j}\)

#### Tug of War Problem

Three people pull a rope with forces:

- \(\vec{F}_1 = 10 \hat{i} + 5 \hat{j}\) Newtons.
- \(\vec{F}_2 = -8 \hat{i} + 7 \hat{j}\) Newtons.
- \(\vec{F}_3 = 3 \hat{i} - 6 \hat{j}\) Newtons.

**Net Force:**

\(\vec{F}_{\text{net}} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3\)

**Magnitude:**

\(|\vec{F}_{\text{net}}| = \sqrt{(5)^2 + (6)^2}\)

**Direction:**

\(\theta = \tan^{-1} \left( \frac{6}{5} \right)\)

#### Python Implementation

[View Tug of War Code Example](https://gist.github.com/your-link-here)

```python
import numpy as np

# Forces
F1 = np.array([10, 5])
F2 = np.array([-8, 7])
F3 = np.array([3, -6])

# Net force
net_force = F1 + F2 + F3

# Magnitude and direction
magnitude = np.linalg.norm(net_force)
direction = np.degrees(np.arctan2(net_force[1], net_force[0]))

print("Net Force:", net_force)
print("Magnitude:", magnitude)
print("Direction:", direction)
```

---

### Additional Resources

- [Histogram Video](https://drive.google.com/file/d/1g_NWFWEwnrwKtEe_6Ub3wr88oSFAZrdw/view?usp=drive_link)
- [Heatmap Video](https://drive.google.com/file/d/1VlTeJLOTASAtO9nbkH_QxsGp8jWv7EO0/view?usp=drive_link)
- [Tug of War Video](https://drive.google.com/file/d/1Rbj_JCdAgs84ctgMNpFsYSufM_-e7lto/view?usp=drive_link)

---

### Conditional Probability

Conditional probability is the probability of an event \(A\) occurring given that another event \(B\) has occurred:

\(P(A | B) = \frac{P(A \cap B)}{P(B)}\)

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

![Conditional Probability](./conditional_probability.jpg)

---

