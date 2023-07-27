
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

This project initially posed itself as a trinary classifcation problem. The reason being is that the data contained 3 potential target variables - 'functional', 'non-functional' and 'functional needs repair'.

This is what the classes looked like with nearly 60k rows in the combined datasets:

![trinary-class-barchart.png](Media/trinary-classes-population.png)


