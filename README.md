# Data Analytics And Visualization
Course Page for DS250 (Data Analytics and Visualization) being taught at [IIT Bhilai, India](https://www.iitbhilai.ac.in/index.php) in the Winter Semester of 2025.
<br> Course Instructor: [Dr. Gagan Raj Gupta ](https://www.iitbhilai.ac.in/index.php?pid=gagan)

This course's purpose is to introduce students to various algorithms and techniques for data analysis and visualization. We will emphasize activity-based learning and develop industry-relevant skills in the fields of data visualization and analysis of complex data sets, such as large network data. 

Motivation
----------
* Useful insights can be obtained from data that can help people: healthcare, industry, governments, science
* Getting data is becoming easier day by day, but is very complex and difficult for people to understand
* Data has _errors_ of various types (missing, incorrect etc.), is _incomplete_ and is _hard to clean_ (e.g. user reviews/ratings, distorted images) 
* Data usually has _complex correlations_ and i.i.d. assumptions don't always work very well (e.g. graph data, time-series data) 
* Data Visualization is critical to help us engage more diverse audience in the process of analytical thinking 

In this course, we want to learn how that is being done and solve real-life problems that interest us.

Activity Based Learning
------------------------
# UNDERSTAND DATA ---> HYPOTHESIS ---> MODELS ----> INSIGHTS
The Activities will reinforce this theme.will be done in class/lab
 * Weight distribution: study modality
 * Rolling dice: central limit theorem
 * Phone features and cost model
 * Composition: essay on "My country" -- study the vocabulary, language model, and probabilities. Can a machine compose this essay now?
 * Measure various quantities: time you sleep, time to eat, time you spend on phone, time you study, play etc. Understand these distributions...
 * Personality charts: Is there a person like me in the class whom I don't know?
 * Clusters: how many groups are there in the class, are groups equal? any outliers there? 
 * Curve-fits -- hidden points will appear after you learnt the curve
 * Guess the number game -- binary search... distribution of number easy or hard?


Course Objectives
-----------------
* Motivate and demonstrate the benefits and uses of data science  
* Impart the skills needed by a data scientist: acquire, clean, model, visualize data
* Teach fundamental algorithms for handling basic and complex datasets including __recommendation, basket analysis, streaming algorithms__
* Study techniques for creating effective visualizations based on principles from graphic design, perceptual psychology, and cognitive science
* Teach basic techniques of machine learning (unsupervised) which is important way to model relationships in data 
* Provide hands-on experience to students in analyzing datasets in diverse fields __(NLP, Image/Video, Graphs, Networks, Bio-informatics, Finance)__

Pre-requisites
--------------
* Basic knowledge of Python (most assignments will be based on Python)
* Knowledge of basic computer science principles and skills
* Math
  * Linear Algebra ( Matrix-factorization, Eigenvalues, Column and row spaces, Norms)
  * Probability theory (Conditional, Bayes Rule, Concentration Inequalities, Distributions, Gaussian, Multi-variate) 
  * Basic Data Structures, Algorithms and Asymptotic Analysis (graphs, heaps, lists, dynamic programming)
  * Calculus (Multi-variate)
* Web Technologies 
  * HTML
  * JS
  * CSS
  
If you don't meet one or more pre-requisites, be prepared to spend more time before or during the course in learning them.

Books
------
* DAV: Data Analytics and Visualization, (to be published soon)
* MML: [Mathematics of Machine Learning](https://mml-book.github.io/)
* LFD: Learning From Data, Gilbert strang
* IVB: Interactive visualization for the Web, Scott Murray
* ISL: Introduction to Statistical Learning
* PML : Probabilistic Machine Learning, Kevin P. Murphy
* DSC: Data Science from Scratch, Joel Grus
* GA: Graph Algorithms: Practical Examples in Apache Spark and Neo4J, Mark Needham, Amy Hodler

Syllabus for the course
------------------------
Introduction to Data science workflow; Data Collection and Exploratory Analysis: Automated methods for data collection, Data and Visualization Models, Data wrangling and cleaning, and Exploratory data analysis; Building Models for: Classification, Clustering, Regression; Model evaluation: statistical tests for significance of predictors; Time-series Analysis: Characteristics, Regression, Exploratory data analysis, ARIMA Models; Visualization Design: Introduction, Abstractions, Validation, Marks and Channels; Visualization of Different Data Types: Tabular Data, Multidimensional Data, Spatial Data, Graphs, Text Data; Assorted Topics: Graphical Perception, Interaction dynamics for Visual Analysis, Using Space Effectively, Stacked Graphs, Geometry & Aesthetics.

Class Materials
----------------
Google drive (for IIT Bhilai students): [GDrive](https://drive.google.com/drive/folders/11TT4hnNL50yKA7oP3damPIkM9aBF0rNF)
|#| Week   | Topics planned in this week | Text Book Reference |
| ----- | ------------| ----------- | -------- |
|1|  Dec 30  | Histogram, Dice Rolling, Central Limit Theorem, Height Weight Distribution |  |
|2|  Jan 6  | Regression, Clustering, Word Length Distribution, Vectors, Random Matrices, Linear Project, Convex Lens, Volume Calculation Using Determinants | MML Ch 4 |
|3|  Jan 13  | Linear Projections, Gradients, Noise, Multi-variate Gaussian | MML Ch 5,6 |
|4|  Jan 20  | Linear Regression, analysis, Multi-variate Calculus | MML Ch 5 |
|5|  Jan 27  | Information Theory, Decision Theory | PML Ch 5,6 |
|6|  Jan 27  | Seaborn, plotly,PCA,SVD | Lab |
|7|  Feb  3   | Classification: Statistics (MLE, MAP) | PML Ch 4 |
|8|  Feb  3   | TensorFlow | Lab |
|9|  Feb 10   | High Dimensional Data Analysis, Dimensionlity Reduction | FOD Ch1 |
|10|  Feb 10   | Lab Assignment: Individual Activity Last Lab | Lab |




Detailed Schedule
-----------------
Legend:
|#| Week| Topics planned in this week | Text Book Reference |
| --- | ------------| ----------- | -------- |
|1| Dec 30 | Introduction to Data Science, Facets of Data, Data Science Process, Data Models: Geometric view and Statistical view, Probability Distributions | |
|1| Dec 30 | Lab: Data Loading, Data Cleaning and Exploration with Python | |
|2| Jan 6 | Linear Algebra and Regression | |
|2| Jan 6 | Lab: Intro to Numpy and Pandas; Intro to Matplotlib, Seaborn, Plotly   | https://realpython.com/ggplot-python/ https://altair-viz.github.io/   |
|3| Jan 13| Optimization theory and applications, PCA ||
|3| Jan 13| Lab: Collect Data (Webscraping, API), Analyze and Make a chart in D3, Density Plots|IVB |
|3| Jan 13| Case Studies: Predicting malicious URLs, Risk in Bank Loans, Sentiment Analysis, Healthcare Dataset||
|4| Jan 20| Distance Measures, Recommendation Rules, Association Rules, ML intro, Learning by Prototypes ||
|4| Jan 20| Lab: ||
|5| Jan 27| Learning to classify data: various algorithms, Generative and Discriminative Models,  |PRML|
|5| Jan 27| Lab: Connect Python to D3 using Flask||
|6| Jan 31| Mathematics of Neural Networks, Decision Trees | PRML|
|6| Jan 31| __Project: Complete a Basic Data Classification Interactive Application__ ||
|7| Feb 7|   Networks: Basic Algorithms: Path Finding|GA Ch 4|
|7| Feb 7| Lab: Visualization of Networks and Trees in D3|IVB Ch13|
|8| Feb 14|  Networks Analysis: Random Walks, Counting Triangles|GA Ch 4 |
|8| Feb 14| Lab: Intro to Neo4J|GA Ch3|
|8| Feb 14| Case Studies: Knowledge Graphs, Product Recommendation, Graphical Models ||
|9| Feb 21|  Centrality Algorithms, Community Detection Algorithms |GA Ch5|
|9| Feb 21| Lab: Data Analysis using Neo4J| |
|10| Feb 28| Text and Graph Embedding Algorithms|GA Ch6,7|
|10| Feb 28| Lab: Word Cloud, Text Visualization, NLP libraries: NLTK    |    |
|11| Mar 7|  Graph Machine Learning |GA Ch6,7|
|11| Mar 7| __Project: Complete a graph data analysis Application__| |
|12| Mar 12-20|__Mid Sem Break__||
|12| Mar 21| __Tierce 2 Exam__||
|13| Apr 4 | Time Series Data Analysis  ||
|13| Apr 4| Lab: Interactive Dashboards|IVB Ch10|
|14| Apr 11|  Streaming Data Algorithms||
|14| Apr 11| Lab: Time Series Prediction and Clustering  ||
|14| Apr 11| Case Studies: Weather, Financial Data, Imports/Exports,  ||
|15| Apr 18|  Algorithms for Clustering Data: K-Means, K-Means++, DTW, DBSCAN ||
|15| Apr 18 | Lab: Geographical Maps  |IVB Ch14|
|15| Apr 25|  Dimensionality Reduction Algorithms | |
|16| Apr 25| Lab: Visualization of High-Dimensional Data using T-SNE ||
|17| Apr 25 |__Major Project: Complete a major data analysis course project__  ||



# Data Scientist vs. Software Developer (Engineer)
Both data-scientists and software developers are good at designing and building complex systems with many interconnected parts using different tools and frameworks. In general, software developers design systems consisting of many well-defined components, whereas data scientists work with systems wherein at least one of the components isn’t well defined prior to being built. That component is usually closely involved with data processing or analysis. Data scientists specialize in creating systems that rely on probabilistic statements about data and results. Well known examples of these are Google search engine (“These are probably the most relevant pages”), product recommendations on Amazon.com (“We think you’ll probably like these things”).

# Skills for a data scientist
We will cover the skills necessary for cleaning, modeling and visualizing data by a data-scientist. We will also learn the skills needed for developers designing interactive dashboards and applications.

# D3 ([website](https://d3js.org/))
D3.js is a JavaScript library for manipulating documents based on data. D3 helps you bring data to life using HTML, SVG, and CSS. D3’s emphasis on web standards gives you the full capabilities of modern browsers without tying yourself to a proprietary framework, combining powerful visualization components and a data-driven approach to DOM manipulation. 

To make life easy, we will be using the tutorials and notebook environment provided by [Observable](https://observablehq.com/collection/@d3/learn-d3)

Check these examples: [Sankey](https://observablehq.com/@d3/sankey), [Cholorpleth](https://observablehq.com/@d3/choropleth), [Hexbin](https://observablehq.com/@d3/hexbin-map),[Fisheye](https://bost.ocks.org/mike/fisheye/)

# Labs and Projects
The project and lab component of this course will equip students with modern software toolkit to develop their own data analysis and interactive visualization applications (web/android) to better appreciate the data science process.



