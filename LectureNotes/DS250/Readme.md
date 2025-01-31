# DS250 (DAV) Module
LECTURE-1 Notes
## Introduction

 Notes on Plotting Histograms and Heatmaps 
 

 

1. **HISTOGRAMS**:-


A histogram is a graphical representation of the distribution of data. It divides the entire range of values into intervals (called bins) and counts the number of data points that fall into each bin.

 
*{Mathematical Definition*:-} 

Let  be the data points. Divide the range of data into  bins, where:

The bin width  is:

w = (x) - (x)}{k}

b_i  x < b_{i+1} 

Here,  and  are the edges of the -th bin.

*Steps to Plot a Histogram:-*

1. Choose the number of bins: Use the rule of thumb or algorithms like the Sturges' formula:

k =  _2(n) + 1 

2. Plot the frequencies using bar heights.


Python Code Example:-

import matplotlib.pyplot as plt

import numpy as np

% Sample data

data = np.random.normal(0, 1, 1000)

% Plotting the histogram

plt.hist(data, bins=30, edgecolor='black', alpha=0.7)

plt.title('Histogram')

plt.xlabel('Value')

plt.ylabel('Frequency')

plt.show()


*ACTIVITY ON HISTOGRAM:- *

### Part A: Word Length Histogram
*{Objective}
Create a histogram that represents the frequency of words based on their length in any paragraph from your preferred book.

*{Steps}

     Choose a paragraph from your favorite book.
     Count the number of letters in each word.
     Group words by their lengths (e.g., words with 1 letter, 2 letters, etc.).
     Plot the histogram with:
    
         **X-axis**: Word lengths.
         **Y-axis**: Frequency of words of each length.
    
 ### Part B: Starting Letter Histogram
*{Objective}
Create a histogram to analyze the frequency of words starting with each letter of the alphabet.

*{Steps}

     Use the same paragraph as in Part A.
     Count how many words start with each letter (A-Z).
     Plot the histogram with:
    
         **X-axis**: Starting letters (A-Z).
         **Y-axis**: Frequency of words starting with each letter.
    

    
    [width=0.6 , angle=270]{word length.jpg}
    
    [width=0.7]{word_length Distribution.jpeg}
    
    

### Part C: Forecasting with Weight and Height Functions
*{Objective}
Plot histograms using functions for weight and height over time.

*{Functions}
Define the following functions:

    w(t) &= t + 2,   
    h(t) &= 3t + 5,  

where  t  represents time (from the beginning to today).

*{Steps}

     Create data points for different values of  t  (e.g.,  t = 0, 1, 2,  
     Calculate  w(t)  and  h(t)  for each  t 
     Plot the histogram using:
    
         **X-axis**: Time ( t 
         **Y-axis**: Weight ( w(t)  or Height ( h(t) 
      
    [width=0.8]{starting_letter_frequency.jpg}
    
*ANSWER THE FOLLOWING QUESTIONS*

Q1. A. PLot the histogram on the basis of word length of any Paragraph of your preferred book.

B. PLot the Starting letter of the Word.

C. Use the following function to PLot the same:- 

    Weight = w(t),
    Height = h(t)
     where :-
     
     time = t (begining, ..................., Today)

     forecast the following in Histogram Plotting.

D. Plot a histogram for the dataset [1, 2, 2, 3, 3, 3, 4, 4, 4, 4] with customizations:

Change color, labels, and title.

Add gridlines and annotate the highest frequency bin.

E. Import a real-world dataset (e.g., Iris dataset).

Plot histograms for numerical columns like petal length or sepal width.
     
2. **HEAT MAPS**

A heatmap is a data visualization technique used to represent data in a
matrix format with varying intensities of color to show magnitude.

Mathematical Definition:-

For a matrix  with elements , a heatmap assigns a color  to each cell based on a colormap :

c_{ij} = C(a_{ij})

*Steps to Create a Heatmap:-*

1. Normalize the data: Rescale values if needed.

2. Choose a colormap: Maps numerical values to colors.

3. Visualize the data as a grid.

**Python Code Example:-**

import seaborn as sns

import numpy as np

import matplotlib.pyplot as plt

%Sample data

data = np.random.rand(10, 10)

%Plotting the heatmap

sns.heatmap(data, annot=True, cmap='viridis')

plt.title('Heatmap')

Part 1: **Basics of Vector Algebra**
1.1 **Vectors**

A vector is a quantity that has both magnitude and direction. It can be represented in the Cartesian coordinate system with components along the x, y, and z axes. 

For example, a vector  in two-dimensional space can be written as:

 = A_x  + A_y 

where:
-  A_x  and  A_y  are the components of the vector along the x and y axes, respectively.
-  and  are the unit vectors along the x and y axes.


1.2 **Vector Operations**:-

*Addition of Vectors*: The sum of two vectors is obtained by adding their corresponding components.

 +  = (A_x + B_x)  + (A_y + B_y) 

*Scalar Multiplication*: When a vector is multiplied by a scalar, each component of the vector is multiplied by that scalar.

k   = k  A_x  + k  A_y 

*Dot Product*: The dot product of two vectors is a scalar quantity given by:

   = A_x  B_x + A_y  B_y

*Cross Product*: The cross product of two vectors gives a vector perpendicular to both vectors. For two 2D vectors  = A_x  + A_y  and  = B_x  + B_y  the cross product is:

   = (A_x B_y - A_y B_x) 

where  is the unit vector along the z-axis.

    
    [width=0.7]{vector matrix.jpg}
    ---

### Part 2: **Tug of War Problem**

In this problem, we will model a tug of war scenario where three people are pulling a rope from different directions. The goal is to determine the resulting force on the rope by calculating the Vector that is  sum of all the individual forces.

#### **2.1 Problem Description**

Three people are pulling on a rope from different directions:

- Person 1 applies a force of  _1 = 10  + 5   Newtons.\ 

- Person 2 applies a force of  _2 = -8  + 7   Newtons.\ 

- Person 3 applies a force of  _3 = 3  - 6   Newtons.

We will calculate the net force on the rope by adding these vectors together and analyze the direction and magnitude of the result.

2.2 *Steps to solve:-*

1. Add the vectors  _1, _2,  and  _3  

2. Compute the magnitude of the resulting vector. \ 

3. Analyze the direction of the resultant vector.

\ 
**ACTIVITY**:-

### Activity: Understanding Vectors through Tug of War
*{Objective}
The goal of this activity is to understand the concept of vectors, their operations (addition, magnitude, and direction), by modeling a tug of war scenario where three people are pulling a rope from different directions.

*{Problem Description}
Three people are pulling on a rope from different directions:

     Person 1 applies a force of  _1 = 10  + 5   Newtons.
     Person 2 applies a force of  _2 = -8  + 7   Newtons.
     Person 3 applies a force of  _3 = 3  - 6   Newtons.

We will determine the net force on the rope by calculating the vector sum of  _1, _2,  and  _3  Additionally, we will compute the magnitude and analyze the direction of the resultant vector.

*{Steps to Solve}

     Add the vectors  _1, _2,  and  _3 
    
        _ &= _1 + _2 + _3 
        &= (10  + 5 ) + (-8  + 7 ) + (3  - 6 ) 
        &= (10 - 8 + 3)  + (5 + 7 - 6)  
        &= 5  + 6 .
    

     Compute the magnitude of the resulting vector  _ 
    
        |_| &=  
        &=  
        &=   7.81  .
    
   Analyze the direction of the resultant vector:
    
         &= ^{-1} ( } ) 
        &= ^{-1} ( {5} ) 
        &= ^{-1} (1.2) 
        & 50.19^    .
    

*{Discussion Points}

     **Addition of Vectors:** Demonstrates how forces combine in two dimensions.
     **Magnitude of the Resultant Vector:** Shows how to calculate the strength of the net force.
     **Direction of the Resultant Vector:** Explains the use of trigonometry to find the orientation of the net force.

*{Extension Activity}
Challenge students to:

     Add more participants with different forces and calculate the new net force.
     Use graphical methods (parallelogram or head-to-tail) to verify the calculations.
     Explore real-world scenarios where vectors play a role, such as forces in sports or physics problems involving motion.

    
    [width=0.7]{VECTOR.jpg}
    
  ---

Part 3: *Python Implementation*

Let's implement the solution in Python using numpy to handle vector operations efficiently.

Python:-

import numpy as np

# Define the force vectors \ 

F1 = np.array([10, 5])  # Force from person 1 \ 

F2 = np.array([-8, 7])  # Force from person 2 \ 

F3 = np.array([3, -6])  # Force from person 3 \ 

Step 1: Calculate the net force (vector sum)
net_force = F1 + F2 + F3

Step 2: Calculate the magnitude of the net force
magnitude = np.linalg.norm(net_force)

Step 3: Find the direction of the net force (angle with respect to x-axis) \ 

direction = np.arctan2(net_force[1], net_force[0])  Angle in radians \ 

direction_degrees = np.degrees(direction)  # Convert to degrees \  

%Display the results
print("Net Force Vector (F_net):", net_force)

print("Magnitude of Net Force:", magnitude, "Newtons")

print("Direction of Net Force:", direction_degrees, "degrees") 
---
\ 
 \ 

**Output:**

Net Force Vector (F_net): [5 6]

Magnitude of Net Force: 7.810249675906654 Newtons

Direction of Net Force: 50.19442890773457 degrees. 


\ 

 **CONDITIONAL PROBABILITY:-**

Conditional probability is the probability of an event occurring given that another event has already occurred. In other words, it quantifies the likelihood of an event  A  happening, under the condition that event  B  is known to have occurred. The conditional probability of  A  given  B  is denoted as  P(A | B)  and it is calculated using the formula:

P(A | B) = {P(B)}

*where:*

-  P(A  B)  is the probability that both events  A  and  B  occur (i.e., the intersection of  A  and  B 
-  P(B)  is the probability that event  B  occurs.

### **Dice Experiment and Conditional Probability**

Let's consider a dice experiment. We roll a standard 6-sided die, and let’s define the following events:

- *Event A*: The die shows an even number (2, 4, or 6).

- *Event B*: The die shows a number greater than 3 (4, 5, or 6).

We want to calculate the conditional probability of event A given that event B has occurred, i.e.,  P(A | B) 

### *Step-by-Step Calculation*:-

#### Step 1: Define the Sample Space
The sample space  S  for a 6-sided die is:

S =  2, 3, 4, 5, 6

#### Step 2: Calculate the Probability of Event B,  P(B) 
Event B occurs when the die shows a number greater than 3. So,  B =  5, 6  The probability of event B is:

P(B) =  B}{ S} = {6} = 0.5

#### Step 3: Calculate the Probability of the Intersection of Events A and B,  P(A  B) 
The intersection of events A and B,  A  B  occurs when the die shows a number that is both even (from event A) and greater than 3 (from event B). The numbers that satisfy both conditions are   6 

So,  A  B =  6  and the probability of this intersection is:

P(A  B) =  A  B}{  S} = {6} = 0.3333

#### Step 4: Apply the Conditional Probability Formula
Now, we can apply the formula for conditional probability:

P(A | B) = {P(B)} = {6}}{{6}} = {3}

So, the conditional probability of event A (the die shows an even number) given that event B (the die shows a number greater than 3) has occurred is:

P(A | B) = {3}


\ 

###* Interpretation* 

Given that the die has shown a number greater than 3, the probability that it is also an even number (either 4 or 6) is  {3}  This conditional probability helps us understand how the knowledge of event B influences the likelihood of event A.

%
%
% % For nicer tables
% % For adjusting margins
%

*{Activity: Understanding Conditional Probability Using a Dice Experiment}

*{Objective}
To understand the concept of conditional probability through a simple dice-rolling experiment.

*{Materials Needed}

     A six-sided die (standard die with faces numbered 1 to 6).
     Pen and paper (or a whiteboard) for recording outcomes.

*{Instructions}

*{Step 1: Define the Experiment}

     Roll a standard six-sided die multiple times (e.g., 20 trials).
     Record the outcome of each roll.

*{Step 2: Define Events}
Let:

     **Event A**: The die roll results in an even number ( 4, 6
     **Event B**: The die roll results in a number greater than 3 ( 5, 6

*{Step 3: Conduct the Experiment}

     Roll the die and record the outcomes.
     For each roll, determine whether it satisfies Event A, Event B, or both.

*{Step 4: Analyze the Results}

     Count the number of rolls where:
          
               Event A occurs ( n(A) 
               Event B occurs ( n(B) 
               Both Event A and Event B occur ( n(A  B) 
          
     Use the frequency of these events to estimate probabilities:
          
          P(A) = ,  
          P(B) = ,  
          P(A  B) = .
          

*{Step 5: Calculate Conditional Probabilities}
Using the formula for conditional probability:

P(A  B) = {P(B)}

     Substitute the experimental values of  P(A  B)  and  P(B)  into the formula.
     Interpret the result:
          
                P(A  B)  Probability of rolling an even number, given that the number is greater than 3.
          

*{Example of Recorded Data (Sample Table)}

{cccccc}

**Trial** & **Outcome** & **Event A (Even)** & **Event B ( & **Both A and B**  

1 & 4 & Yes & Yes & Yes  
2 & 2 & Yes & No & No  
3 & 5 & No & Yes & No  
4 & 6 & Yes & Yes & Yes  
5 & 3 & No & No & No  

... & ... & ... & ... & ...  

*{Discussion Points}

     **Theoretical Probability**:
          
                P(A) = {6} = 0.5  (since there are 3 even numbers out of 6).
                P(B) = {6} = 0.5  (since there are 3 numbers greater than 3).
                P(A  B) = {6} = 0.333  (only 4 and 6 satisfy both conditions).
          
          Using these values:
          
          P(A  B) = {P(B)} = {0.5}  0.666
          
     **Connection to Real-World Applications**:
          Conditional probability is used in fields like medicine (e.g., probability of disease given a positive test result) and weather forecasting.

*{Extension Activity}

     Modify the conditions of the experiment. For example:
          
               Event A: Rolling a multiple of 3 ( 6
               Event B: Rolling an odd number ( 3, 5
          
     Explore the relationship between the events when they are independent or mutually exclusive.

***Python Code Implementation:-***

We can simulate this dice experiment and compute the conditional probability using Python:

import numpy as np

# Define the sample space for a 6-sided die

sample_space = [1, 2, 3, 4, 5, 6]

# Define the events A and B

A = [2, 4, 6]  # Even numbers

B = [4, 5, 6]  # Numbers greater than 3

# Calculate P(A ∩ B) - intersection of A and B

intersection_A_B = list(set(A) & set(B))

# Calculate P(B)

P_B = len(B) / len(sample_space)

# Calculate P(A ∩ B)

P_A_intersection_B = len(intersection_A_B) / len(sample_space)

# Calculate P(A | B) using the formula

P_A_given_B = P_A_intersection_B / P_B

# Display the result

print("P(A | B) =", P_A_given_B)

### Output:

P(A | B) = 0.6666666666666666

This Python code confirms our theoretical calculation that the conditional probability of event A given event B is  {3}  

KEEP LEARNING, KEEP GROWING :) 
