
# Predicting the Functionality of Water Pipelines in Tanzania using Machine Learning Classification Models
---
![tanzania-water-crisis.jpg](Media/tanzania-water-crisis.jpg)

---
## Table of Contents
1. [Business Understanding](#1.-Business-Understanding)
2. [Data Understanding](#2.-Data-Understanding)
3. [EDA/Preperation](#3.-EDA/Preperation)
4. [Preprocessing/Modeling](#4.-Preprocessing/Modeling)
5. [Final Model Further Evaluation and Tuning](#5-final-model-further-evaluation-and-tuning)
6. [Appendix]

# 1. Business Understanding

There is a country in East Africa known as Tanzania and for many years, villages across this country have struggled accessing clean and healthy water sources. In the case where villagers have access to a water well, the quality of the water will always be in question. Not to mention, people often have to travel great distances to access these water wells. To tackle this problem, I will be taking a deeper look at the data provided by Taarifa and the Tanzanian Ministry of Water, In hopes of being able to accurately predict the functionality of the water pipelines in Tanzania. I believe that by predicting how well the water pipelines function, there will then be a better understanding of which waterpoints will fail, thus focusing on how to improve and maintain clean, portable water for communities across Tanzania.

# 2. Data Understanding

The data collected for this project consists of three seperate csv files. One of the first steps I took was to concatenate these seperate dataframes in a way that makes sense. The documentation has also been recorded for each of the data columns. To view the documentation ahead of time, please click this [link](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/25/#features_list 'This will open another tab'). As for the three datasets, they are located in the repository under `Tanzanian_Datasets`, if you would like to view those seperately on your own. The column features in these data frames are all relative to how water piplines are produced and manufactured in Tanzania. The data consists of features that state- who funded the well, the year the waterpoint was constructed, how the waterpoint is managed etc.

This project initially posed itself as a trinary classifcation problem. The reason being is that the data contained 3 potential target variables - 'functional', 'non-functional' and 'functional needs repair'.

This is what the classes looked like with nearly 60k rows in the combined datasets:

![trinary-class-barchart.png](Media/trinary-classes-population.png)


So between `functional` and `non functional`, there isnt much of a class imbalance considering `functional needs repair` is only 7% of the data. 

This leaves me to make a pretty big judgement call on whether or not I am going to keep the `functional needs repair` class, as part of the dataframe and overall project.

By eliminating this class, I am only taking out 7% of the data, as well as lessening the complexity of the project. The objective and goal of the project still remains intact, and the classification project goes from ternary to binary.
In doing this, I hope to simplify the modeling process while being able to more accurately predict whether a pipeline is strictly `functional` or `non functional`.