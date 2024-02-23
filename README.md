# R-Project
Display demographic data using plot options in R

As the old adage goes, a picture is worth a thousand words! In our increasingly data-driven world, it has become essential to understand the data being collected on a deeper level. Data visualization is the graphical representation of data. The visualization of data is an important aspect of presenting an analysis done on the data in a way that makes it easy for people from different walks of life to view the data through plots, notice trends, spot differences, etc. R is a programming language that provides several convenient options to plot data like scatterplots, boxplots, ggplots, etc.

The National Center for Health Statistics has been recording mortality rates in the United States with respect to sex, race, and year since 1900. This dataset has been chosen to demonstrate some visualization options available in R. There are 5 columns in this dataset: Year, Race, Sex, Average Life Expectancy (Years), and Age-adjusted Death Rate. The year range is from 1900 – 2018 [1]. 

There are several parameters that can be compared and contrasted in this dataset. I have chosen the following:

# 1.	Average Life Expectancy over the years
There are several ways to present the same data. Finding the best way to present is always a challenge and more times than not, a matter of personal preference. For example, look at the two plots below. Fig.1 is a scatterplot and Fig.2 is a ggplot. They both present the same information - Average life expectancy (expressed in years) of black males from 1900 - 2018.  If we notice carefully, Fig.2 shows a sharp dip in life expectancy around the year, 1918. This coincides with when the flu pandemic occurred in the US [2]. I believe that Fig.2 was able to emphasize the dip much better than Fig.1 . Other than that, both plots show that the average life expectancy has steadily improved over the years, be it due to advancement in science leading the way for better medicines, dental care, vaccines, etc more available, or technology that can lead to early detection of many diseases, safer cars being available, etc. 

![Figure1](https://github.com/maddies-codespace/R-Project/assets/141537679/b91151c6-3971-4fe6-8276-3b9ea4ae0448)

Fig.1: Graphing the average life expectancy of black males by year as a scatter plot

