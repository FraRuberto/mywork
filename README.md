# Exploring the Palmer Penguins Dataset

![Palmer Penguins](https://tkoomar.github.io/post/tt-palmer-penguins/featured_huc6cf4a21090aa2ea134ebf239881872e_167000_720x0_resize_lanczos_2.png)


## Table of Contents

1. [Introduction](#introduction)
2. [Purpose](#purpose)
3. [Dataset Background](#dataset-background)
    - 3.1 [Main Variables](#main-variables)
4. [Contents of the Notebook](#contents-of-the-notebook)
    - 4.1 [Overview of the Dataset and Variables](#overview-of-the-dataset-and-variables)
    - 4.2 [Types of Variables](#types-of-variables)
    - 4.3 [Correlation Analysis of Two Variables in the Dataset](#correlation-analysis-of-two-variables-in-the-dataset)
5. [Technology/Library Used](#technologylibrary-used)
6. [Literature & Documentation](#literature--documentation)
7. [Conclusion](#conclusion)


## Introduction

Welcome to the world of data analysis with the Palmer Penguins dataset! This repository contains a Jupyter notebook where we will delve into the intricacies of data analysis and visualization using real-world data. The aim of this notebook is to give valuable insights into the principles of data analytics, exploring and interpreting the world famous Palmer Penguin datasets.

Click [![here](https://img.shields.io/badge/here-red?style=for-the-badge)](https://gist.githubusercontent.com/slopp/ce3b90b9168f2f921784de84fa445651/raw/4ecf3041f0ed4913e7c230758733948bc561f434/penguins.csv) for the complete Palmer Penguins dataset. 

## Purpose 

The purpose of this notebook is to provide a comprehensive analysis of the Palmer Penguins dataset, covering aspects such as data cleaning, visualization, and statistical analysis. By the end of this exploration, readers will have a clearer understanding of the dataset and the insights it holds. Additionally, this notebook serves as a learning opportunity for those interested in data analysis and visualization techniques using Python.

## Dataset background

The Palmer Penguins dataset provides valuable insights into the characteristics and behaviors of three penguin species: Adélie, Chinstrap, and Gentoo. The observations include various morphological measurements such as bill length, bill depth, flipper length, body mass, as well as categorical variables like species, island of origin, and sex.

### Main variables:

- Species: Categorical variable indicating the species of the penguin (Adélie, Chinstrap, or Gentoo).
- Island: Categorical variable indicating the island in the Palmer Archipelago where the penguin was observed.
- Bill Length (mm): Numerical variable representing the length of the penguin's bill in millimeters.
- Bill Depth (mm): Numerical variable representing the depth of the penguin's bill in millimeters.
- Flipper Length (mm): Numerical variable representing the length of the penguin's flipper in millimeters.
- Body Mass (g): Numerical variable representing the body mass of the penguin in grams.
- Sex: Categorical variable indicating the sex of the penguin (male or female).

![Palmer Penguins](https://previews.123rf.com/images/aomeditor/aomeditor1903/aomeditor190300021/122254680-illustrator-of-body-parts-of-penguin.jpg)

Click [![here](https://img.shields.io/badge/here-green?style=for-the-badge)](https://www.kaggle.com/code/pratik1120/penguin-dataset-eda-classification-and-clustering) for more information about the penguin dataset. 


## Contents of the notebook

### Overview of the Dataset and Variables

This section serves as the first part of the notebook and provides an overview of the Palmer Penguins dataset and its variables. The dataset contains information about penguins' species, island of origin, physical measurements, and sex. The Palmer Penguins dataset includes 344 entries and 7 columns. This Jupiter notebook contains a brief overview of some key variables:

#### Species
This dataset includes three species of penguins: Adelie, Chinstrap, and Gentoo.
The majority of penguins included in this dataset are of the Adelie species.

#### Island of Origin
Penguins are observed on three islands: Togersen, Biscoe, and Dream.
The distribution of penguins among the islands is not uniform.

#### Sex of Penguins
The dataset includes information about the sex of the penguins observed, divided into two categories: MALE and FEMALE.

#### Body Mass of Penguins
The body mass of penguins analyzed within this dataset ranges from 2700g to 6300g.
Summary Statistics

The table below provides summary statistics for numerical variables in the dataset:

### Dataset Overview

The dataset consists of 344 entries and 7 columns. Here's a brief overview of the key variables explored in this analysis:

| Variable           | Description                                      |
|--------------------|--------------------------------------------------|
| Species            | Three species of penguins: Adelie, Chinstrap, and Gentoo. |
| Island             | Penguins are observed on three islands: Torgersen, Biscoe, and Dream. |
| Bill Length (mm)   | Measurements of the penguins' bill length in millimeters. |
| Bill Depth (mm)    | Measurements of the penguins' bill depth in millimeters. |
| Flipper Length (mm)| Measurements of the penguins' flipper length in millimeters. |
| Body Mass (g)      | Body mass of the penguins measured in grams.    |
| Sex                | Sex of the penguins categorized as MALE or FEMALE. |

This initial section provides basic statistics, distributions, and counts for each variable, offering insights into the dataset before diving into further analysis.


The following exploratory analyses are conducted in this notebook:
- Distribution of penguin species
- Distribution of penguins among different islands
- Distribution of penguin sexes
- Body mass distribution of penguins

For a more detailed analysis, refer to the corresponding sections in the notebook.


### Types of Variables

In this second section, explored and suggested the types of variables that should be used to model the variables in the Palmer Penguin dataset in Python. Along with each variable, explained the rationale behind the choice and cite the material I used in my research. I delved into practical examples using some of the variables discussed previously. These examples aim to provide a hands-on understanding of how these variables can be effectively utilized in modeling the Palmer Penguin dataset in Python. By showcasing real-world applications, I hope to demonstrate the significance of each variable and its role in data analysis.

In this section, we will explore the variables in the Palmer Penguin dataset and suggest appropriate types for manipulation in Python.

| Variable           | Type          | Recommended Type for Manipulation |
|--------------------|---------------|------------------------------------|
| Species            | Categorical   | String                             |
| Island of Origin   | Categorical   | String                             |
| Sex of Penguins    | Categorical   | String                             |
| Body Mass          | Continuous    | Float                              |

#### Species

**Type:** Categorical  
**Recommended for Manipulation:** String  
**Rationale:** The species variable consists of discrete categories and can be represented as strings for easy manipulation.

#### Island of Origin

**Type:** Categorical  
**Recommended for Manipulation:** String  
**Rationale:** Similarly, the island of origin variable is categorical and can be represented as strings.

#### Sex of Penguins

**Type:** Categorical  
**Recommended for Manipulation:** String  
**Rationale:** The sex of penguins variable is categorical and can be represented as strings.

#### Body Mass of Penguins

**Type:** Continuous  
**Recommended for Manipulation:** Float  
**Rationale:** Body mass is a continuous numerical variable and should be represented as float for mathematical operations and analysis.

This systematic overview provides clarity on the types of variables present in the dataset and suggests appropriate types for manipulation in Python.

It's noteworthy that *integer type is not suggested for manipulation in this dataset due to the absence of variables that strictly require integer representation*. For instance, representing a categorical variable as an integer may introduce ambiguity and hinder interpretation. For further details on why integer types are not suggested, refer to the notebook. 


### Correlation Analysis of Two Variables in the Dataset

In exploring the physiological traits of penguins, understanding the relationships between various physical attributes becomes crucial. Among these attributes, body mass and flipper length are of particular interest due to their potential implications in penguin biology. In this analysis, we aim to investigate the correlation between body mass and flipper length in penguins using the Palmer Penguins dataset.

I chose 'body_mass_g' (body mass of penguins) and 'flipper_length_mm' (flipper length of penguins) for the following reasons:

- These variables represent physical characteristics of penguins that could potentially be related.
- Body mass and flipper length are both important measurements in understanding the biology and physiology of penguins.
- Exploring the relationship between body mass and flipper length can provide insights into the physical adaptations of penguins.
- I calculated the correlation coefficient, explained the result, and plotted a scatter diagram.

## Technology/Library used

- [Python](https://www.python.org/): Programming language used for data analysis and scripting.
- [Jupyter Notebook](https://jupyter.org/): Interactive development environment used for data exploration and analysis.
- [Pandas](https://pandas.pydata.org/): Python library used for data manipulation and analysis.
- [Matplotlib](https://matplotlib.org/): Python library used for data visualization.
- [NumPy](https://numpy.org/): Python library used for numerical computing.


## Litearature & Documentation

- Alabuda, A. (2022). Classification and EDA - Palmer Penguins. Kaggle. [Link here](https://www.kaggle.com/code/alabuda/)
- Analytics Vidhya. (2022, April). Data Exploration and Visualization using Palmer Penguins Dataset.  [Link here](https://www.analyticsvidhya.com/blog/2022/04/data-exploration-and-visualisation-using-palmer-penguins-dataset/)
- Banerjee, P. (2019). Descriptive Statistics with Python Project. Gist. [Link here](https://gist.github.com/pb111/512c840affb32593d28573fbb764045b)
- Canales Luna, J. (2022, February). Python Details on Correlation Tutorial. DataCamp. [Link here](https://www.datacamp.com/tutorial/tutorial-datails-on-correlation)
- Erondu, F. (2022, November 7). Visualizing the PalmerPenguins Dataset. Medium. [Link here](https://medium.com/@Fortune_/visualizing-the-palmerpenguins-dataset-d3d70bb619b4)
- Field, A. (2018). Discovering Statistics Using IBM SPSS Statistics (Fifth Edition). Sage Publications Ltd.
- Franzese, M., & Iuliano, A. (2019). Descriptive Statistics. Elsevier. [Link here](https://iris.unibas.it/retrieve/d07de51c-aa20-4def-8d07-70a96ec694e6/2019_Descriptive%20Statistics_Elsevier.pdf)
- Goldberg, D. (1991). What Every Computer Scientist Should Know About Floating-Point Arithmetic. ACM Computing Surveys, 23(1), 5-48.
- Horst, A. (2020, November 30). Introduction to palmerpenguins. GitHub [Link here](https://allisonhorst.github.io/palmerpenguins/articles/intro.html#:~:text=The%20palmerpenguins%20data%20contains%20size,Linux%20is%20named%20after%20penguins!)
- JavaTpoint. (N/A). Categorical Variable in Python. [Link here](https://www.javatpoint.comcategorical-variable-in-python#:~:text=In%20Python%2C%20a%20categorical%20variable,as%20nominal%20variables%20or%20factors.)
- Matplotlib Development Team. (n.d.). Histograms. Matplotlib  [Link here](https://matplotlib.org/stable/gallery/statistics/hist.html)
- Matplotlib Development Team. (n.d.). matplotlib.pyplot.hist. Matplotlib. [Link here](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html)
- Matplotlib. (Year unavailable). matplotlib.pyplot.bar Documentation.[Link here](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html)
- Matplotlib. (Year unavailable). Matplotlib.pyplot.scatter Documentation. [Link here](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html)
- McKinney, W. (2017). Python for Data Analysis. O'Reilly Media.
- Mazzaroli, C.M. (Year unavailable). Exploratory Data Analysis to Predictive analysis: Palmer Penguins. [Link here](https://deepnote.com/app/mazzaroli/Exploratory-Data-Analysis-to-Predictive-analysis-Palmer-Penguins-e6bd8932-9ca1-4363-b78a-79f4f4dc818f)
- NumPy Contributors. (n.d.). Array manipulation routines — NumPy v1.21 Manual. [Link here](https://numpy.org/doc/stable/reference/routines.array-manipulation.html)
- NumPy Contributors. (n.d.). [Link here](https://numpy.org/doc/stable/reference/routines.array-manipulation.html)
- Pandey, P. (2020). Five Ways to Use value_counts. Kaggle. [Link here](https://www.kaggle.com/code/parulpandey/five-ways-to-use-value-counts)
- Real Python. (n.d.). Python Variables: Defining, Assigning, and Using Variables in Python. [Link here](https://realpython.com/python-variables/)
- Schober, P., Boer, C., & Schwarte, L. A. (Year unavailable). Correlation Coefficients: Appropriate Use and Interpretation.
- Simplilearn. (n.d.). Python Float: Examples and Basic Guide. [Link here](https://www.simplilearn.com/tutorials/python-tutorial/float-in-python#:~:text=Float%20is%20an%20important%20mathematical,values%20and%20not%20on%20characters.&text=The%20inbuilt%20function%2C%20float(),%E2%80%9D%2C%20%E2%80%9Cand%20infinity%E2%80%9D.)
- Solomon, B. (2018, February 28). Python Plotting With Matplotlib (Guide). [Link here](https://realpython.com/python-matplotlib-guide/)
- Statistics Canada. (n.d.). Introduction to probability - Variables. [Link here](https://www150.statcan.gc.ca/n1/edu/power-pouvoir/ch8/5214817-eng.htm)
- Stojiljković, M. (2019, December 16). Python Statistics Fundamentals: How to Describe Your Data. Real Python.[Link here](https://realpython.com/python-matplotlib-guide/)
- Stojiljković, M. (2019, December 23). NumPy, SciPy, and pandas: Correlation With Python. Real Python. [Link here](https://realpython.com/numpy-scipy-pandas-correlation-python/)
- Twomey, M. (2022, July 12). Exploring Palmer Penguins. [Link here](https://rpubs.com/michelle10128/923430)
- VanderPlas, J. (2016). Python Data Science Handbook. O'Reilly Media. [Link here](https://jakevdp.github.io/PythonDataScienceHandbook/)
- W3Resource. (n.d.). NumPy: Array manipulation - numpy.unique(). [Link here](https://www.w3resource.com/numpy/manipulation/unique.php)
- Yale University Department of Statistics. (1997-98). Categorical Data. [Link here](http://www.stat.yale.edu/Courses/1997-98/101/catdat.htm)


## Conclusion

In this project, we embarked on an insightful journey into the world of penguin biology through an exploratory analysis of the Palmer Penguin dataset. Our investigation revolved around key variables such as species, island of origin, sex of penguins, body mass, and flipper length, each offering unique insights into the characteristics and behaviors of these fascinating creatures.

Through data visualization techniques and correlation analysis, we investigated intriguing patterns and relationships within the dataset. Furthermore, we delved into the intricate relationship between body mass and flipper length, attempting to grasp how these physical attributes may be linked to the evolutionary adaptations of penguins. 

As we wrap up our exploration of the Palmer Penguin dataset, it's clear that our analysis represents just a small contribution to the broader effort of understanding the natural world. While our findings may not be groundbreaking, they highlight the value of using data to gain insights into biological patterns. This project underscores the importance of curiosity-driven exploration and reminds us of the fascinating intricacies of life on Earth.

## End 