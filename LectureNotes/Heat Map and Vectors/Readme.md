### LECTURE ON HEATMAP:- 

A heatmap is a data visualization technique used to represent data in a matrix format with varying intensities of color to show magnitude.

#### Mathematical Definition

For a matrix with elements , a heatmap assigns a color to each cell based on
a colormap :
cij = C(aij )

#### Steps to Create a Heatmap

1. Normalize the data: Rescale values if needed.
2. Choose a colormap: Maps numerical values to colors.
3. Visualize the data as a grid.

#### Python Code Example

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

![Heatmap Example](./images/heatmap_example.jpg)

---

### Vectors and the Tug of War Problem

#### Vectors 

A vector is a quantity that has both magnitude and direction. It can be
represented in the Cartesian coordinate system with components along the x,
y, and z axes.

For example, a vector⃗ A in two-dimensional space can be written as:⃗
A = Axˆi + Ayˆj
where: - Ax and Ay are the components of the vector along the x and y
axes, respectively. - ˆi and ˆj are the unit vectors along the x and y axes.
![VECTOR ](VECTOR.jpg)

#### Tug of War Problem

Three people are pulling on a rope from different directions:
• Person 1 applies a force of⃗ F1 = 10ˆi + 5ˆj Newtons.

• Person 2 applies a force of⃗ F2 = −8ˆi + 7ˆj Newtons.

• Person 3 applies a force of⃗ F3 = 3ˆi − 6ˆj Newtons.

We will determine the net force on the rope by calculating the vector sum of 
F1,  F2, and F3. Additionally, we will compute the magnitude and analyze the
direction of the resultant vector.

Steps to Solve
1. Add the vectors F1, F2, and F3 :
Fnet = F1 + F2 + F3
= (10ˆi + 5ˆj) + (−8ˆi + 7ˆj) + (3ˆi − 6ˆj)
= (10 − 8 + 3)ˆi + (5 + 7 − 6)ˆj
= 5ˆi + 6ˆj.
2. Compute the magnitude of the resulting vector⃗ Fnet:
|Fnet| = p(5)2 + (6)2
= √25 + 36
= √61 ≈ 7.81 N.
3. Analyze the direction of the resultant vector:
θ = tan−1
 Vertical component
Horizontal component
= tan−1
6
5
= tan−1(1.2)
≈ 50.19◦ above the positive ˆi-axis.

#### Python Implementation

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

![Tug of War](vector%20matrix.jpg)

---

### Additional Resources 

- [Heatmap Video](https://drive.google.com/file/d/1VlTeJLOTASAtO9nbkH_QxsGp8jWv7EO0/view?usp=drive_link)
- [Tug of War Video](https://drive.google.com/file/d/1VlTeJLOTASAtO9nbkH_QxsGp8jWv7EO0/view?usp=drive_link)

---
