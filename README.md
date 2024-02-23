# R-Project: Display demographic data using plot options in R

As the old adage goes, a picture is worth a thousand words! In our increasingly data-driven world, it has become essential to understand the data being collected on a deeper level. Data visualization is the graphical representation of data. The visualization of data is an important aspect of presenting an analysis done on the data in a way that makes it easy for people from different walks of life to view the data through plots, notice trends, spot differences, etc. R is a programming language that provides several convenient options to plot data like scatterplots, boxplots, ggplots, etc.

The National Center for Health Statistics has been recording mortality rates in the United States with respect to sex, race, and year since 1900. This dataset has been chosen to demonstrate some visualization options available in R. There are 5 columns in this dataset: Year, Race, Sex, Average Life Expectancy (Years), and Age-adjusted Death Rate. The year range is from 1900 – 2018 [1]. 

A snippet of the csv file is shown here:
![Code_Snippet_01](https://github.com/maddies-codespace/R-Project/assets/141537679/62297163-da0d-4820-8e23-bbacb5923411)

Let us load and prep this data in R Studio.
![Code_Snippet_02](https://github.com/maddies-codespace/R-Project/assets/141537679/11d5100c-a2a3-4048-a652-6e59d431a03b)

We can look at column information and see

There are several parameters that can be compared and contrasted in this dataset. I have chosen the following:

# 1.	Average Life Expectancy over the years
Let us first filter the data based on gender and race. 
Relevant code:
![Code_Snippet_03](https://github.com/maddies-codespace/R-Project/assets/141537679/b4c30f22-c6d4-40df-a09e-3743fd0391ac)


There are several ways to present the same data. Finding the best way to present is always a challenge and more times than not, a matter of personal preference. For example, look at the two plots below. Fig.1 is a scatterplot and Fig.2 is a ggplot. They both present the same information - Average life expectancy (expressed in years) of black males from 1900 - 2018.  If we notice carefully, Fig.2 shows a sharp dip in life expectancy around the year, 1918. This coincides with when the flu pandemic occurred in the US [2]. I believe that Fig.2 was able to emphasize the dip much better than Fig.1 . Other than that, both plots show that the average life expectancy has steadily improved over the years, be it due to advancement in science leading the way for better medicines, dental care, vaccines, etc more available, or technology that can lead to early detection of many diseases, safer cars being available, etc. 

![Figure1](https://github.com/maddies-codespace/R-Project/assets/141537679/b91151c6-3971-4fe6-8276-3b9ea4ae0448)

Fig.1: Graphing the average life expectancy of black males by year as a scatter plot

Code to generate scatter plot:
![Code_Snippet_04](https://github.com/maddies-codespace/R-Project/assets/141537679/8fc5263a-0d3a-4449-9336-e9c284816e62)

![Figure2](https://github.com/maddies-codespace/R-Project/assets/141537679/3d1c52db-b634-4c72-956c-06e851b35529)

Fig.2: Graphing average life expectancy of black males by year as a ggplot

Code to generate ggplot:
![Code_Snippet_05](https://github.com/maddies-codespace/R-Project/assets/141537679/fc959161-c497-4fbf-b404-a00293f135e0)

As a side note, this dip can be observed in data for all males and females irrespective of race. The US lost around 675,000 lives to the flu pandemic [2].

# 2.	Average Life expectancy and gender
Let’s look at how life expectancy varied for men and women over the years. For this analysis, I chose a box plot. Fig. 3 shows a box and whisker plot while also highlighting the median of each group of data.  The median life expectancy of the male and female population was calculated to be 64.6 and 71.6 years respectively. Women live longer than men. What causes relatively earlier deaths in men - is it overall health and hygiene, eating habits, stress, smoking, drinking, risky behavior, etc. 

![Figure3](https://github.com/maddies-codespace/R-Project/assets/141537679/32ff34f8-f8f2-4d10-a812-77a16baec8db)

Fig. 3: Comparison of average life expectancy between males and females

Code to generate box plot:



# 3.	Average Life Expectancy and Race
Another aspect that can be studied with this dataset is what effect, if any does race have in the variation of the average life expectancy. I had read about ggridges [3] and wanted to explore a plot using that option. This plot has the capability to show the distribution of data. Let’s look at Fig. 4, where I compared the distributions of the life expectancy of white and black people. I have marked some peaks on the plot as A, B, C, and D. For the black population, there is an increase in mortality rate starting around age 25 and a small peak, A around age 35. The highest peak came around C, 65 years of age. For the white population, the mortality rate only starts increasing visibly after B, 40 years of age. There is a small peak around 50 and the highest peak comes around D, 75 years of age. It can also be noted that in general, black people have a greater chance of dying early and white people have a greater chance of surviving past 80 years of age. Now, there are several factors that can contribute to this phenomenon - socio-economic factors like poverty, neighborhoods, education, health, access to proper healthcare, genetic predisposition to diseases like sickle cell, diabetes, heart disease, lifestyle choices, etc. 

![Figure4](https://github.com/maddies-codespace/R-Project/assets/141537679/119c177b-f04a-4261-9145-bff959bab093)

Fig.4: Comparison of the average life expectancy of the black vs white population

Code to generate plot using ggridges:


We have to bear in mind not to draw too many conclusions from a narrow view at the data. We do not know when the deaths around A occurred - if that is well in the past or closer to 2018.

There are several more angles in which this dataset can be mined and studied. Happy exploring! Here are some links that were very helpful to me [3-8].


Hyperlinks:
1.	NCHS - Death rates and life expectancy at birth | Data | Centers for Disease Control and Prevention (cdc.gov)
2.	The 1918 Flu Pandemic: Why It Matters 100 Years Later | Blogs | CDC
3.	Introduction to ggridges (r-project.org)
4.	Data Visualization in R with ggplot2: A Beginner Tutorial (dataquest.io)
5.	How to Plot Multiple Boxplots in One Chart in R - Statology
6.	How to Calculate Conditional Mean in R (With Examples) - Statology
7.	Box Plot Explained: Interpretation, Examples, & Comparison (simplypsychology.org)
8.	How to get max of a column based on other columns in R - Stack Overflow

