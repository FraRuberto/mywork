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
    - 4.3 [Correlation Analysis](#correlation-analysis)
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