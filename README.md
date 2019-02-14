# Exploratory Data Analysis with Python Project

This is an exploratory data analysis project. In this project, I explore the `Absenteeism time in hours` dataset.

It is categorized into various sections which are listed in table of contents as follows:-


## Table of contents:-

1.	Introduction to Exploratory Data Analysis

2.	Types of a variable

3.	Distribution of a variable

4.	Types of exploratory data analysis

5.	Exploratory data analysis techniques

6.	Objectives of exploratory data analysis

7.	Exploratory data analysis – prerequisites

8.	Import the required Python libraries

9.	The dataset description

10.	Import the dataset

11.	Overview of the dataset

12.	Check for anomalies in the dataset

13.	Univariate analysis

14.	Multivariate analysis

15.	References


=================================================================================



## 1. Introduction to Exploratory Data Analysis

Several questions come to mind when we come across a new dataset.  The below list shed light on some of these questions:-


•	What is the distribution of the dataset?

•	Are there any missing numerical values, outliers or anomalies in the dataset?

•	What are the underlying assumptions in the dataset?

•	Whether there exists relationships between variables in the dataset?

•	How to be sure that our dataset is ready for input in a machine learning algorithm?

•	How to select the most suitable algorithm for a given dataset?

So, how do we get answer to the above questions? 

The answer is **Exploratory Data Analysis**. It enable us to answer all of the above questions.

**Exploratory Data Analysis** or **EDA** is a critical first step in analyzing a new dataset. The primary objective of EDA is to analyze the data for distribution, outliers and anomalies in the dataset. It enable us to direct specific testing of the hypothesis. It includes analysing the data to find the distribution of data, its main characteristics, identifying patterns and visualizations.  It also provides tools for hypothesis generation by visualizing and understanding the data through graphical representation. 

According to Howard Seltman (Carnegie Mellon University), **"loosely speaking, any method of looking at data that does not include formal statistical modeling and inference falls under the term exploratory data analysis"**. 


=================================================================================


## 2. Types of a variable

Generally, there are two types of variables in the dataset.  These are **Categorical variables** and **Quantitative variables**.  
There are other types of variables in the dataset. For example - confounding variables, control variables, measurement variables, 
random variables or ranked variables. But these are less common type. So, I will limit the discussion to **Categorical** and **Quantitative** variables, as these are the most common types of variables. 


## Categorical variable

Categorical variables are variables which describe a particular category. The examples of categorical variables are hair color, gender, marital status, smoking status, disability, home owner etc. Usually, they take on one of a number of fixed variables in the dataset. 
For example:

•	The category “hair color” could contain the categorical variables “black,” “brown,” “blonde,” and “red.”

•	The category “gender” could contain the categorical variables “Male” or “Female”.


We can divide categorical data into four types. These are:-

**nominal data**, 

**ordinal data**, 

**interval data**, and 

**ratio data**. 


These terms were developed by Stanley Smith Stevens, an American psychologist.  His work was published in 1946 and these terms came 
into effect. These four types of data variable – nominal, ordinal, interval and ratio data are best understood with the help of examples.


**Nominal variable**

A categorical variable is also called a **nominal** variable when it has two or more categories. There is no ordering involved with 
this type of variable. For example, hair colour is a categorical variable having a number of categories - black, blonde, brown, brunette, red, etc. and there is no agreed way to order these from highest to lowest. 
 
 
**Ordinal variable**

In ordinal variables, there is a ordering involved. The order of the values is important and significant. We classify data into three categories. The categories may be low, medium and high. So, the categories express an order of measurement. If these categories were equally spaced, then that variable would be an interval variable.


**Interval variable**

An interval variable is similar to an ordinal variable where the values of the interval variable are equally spaced. So, the 
difference between two interval variables is measurable and constant. The example of an interval scale is Celsius temperature 
because the difference between each value is the same.  For example, the difference between 60 and 50 degrees is a measurable 10 degrees, as is the difference between 80 and 70 degrees. 


**Ratio variable**

A ratio variable, has all the properties of an interval variable, and also has a clear definition of 0.0. When the variable equals 0.0, there is none of that variable. Variables like height, weight, enzyme activity are ratio variables. Temperature, expressed in F or C, 
is not a ratio variable. 



## Quantitative variable

The second category of variables are **Quantitative variables**. They contain numerical data. They can be further classified into two categories:-


**Discrete variable**

Discrete variables are numeric variables that have a finite number of countable values between any two values. A discrete variable is always numeric. For example, the number of customer complaints or the number of flaws or defects.


**Continuous variable**

Continuous variables are numeric variables that have an infinite number of values between any two values. A continuous variable can be numeric or date/time. The examples of continuous variables are income, temperature, height, weight, and distance. 


=================================================================================

## 3. Distribution of a variable

Now, I will discuss the types of distribution of a variable. There are three types of distribution of a variable. They are **Univariate**, **Bivariate** and **Multivariate** distribution. Variables mean the number of objects that are under consideration 
as a sample in an experiment. 


**Univariate distribution**


In univariate distribution, there is only one variable under consideration. It is the simplest form of analysis because only one quantity changes. It does not deal with causes or relationships. The main purpose of the analysis is to describe the data and find patterns that exist within it. The example of a univariate data can be height of a single person.


We can describe patterns found in univariate data using central tendency (mean, median and mode) and dispersion (range, variance, standard deviation, maximum and minimum values and interquartile range).


We can visualize the univariate data using various types of charts and graphs. These are frequency distribution tables, histograms, bar charts, pie charts and frequency polygons.


**Bivariate distribution**

This type of data distribution involves two different variables. The analysis of this type of data deals with causes and relationships and the analysis is done to find out the relationship among the two variables. A very common example of bivariate distribution is height and weight of a single person.


Bivariate analysis means the analysis of bivariate data. It is one of the simplest forms of statistical analysis, used to find out if there is a relationship between two sets of values. Thus bivariate data analysis involves comparisons, exploring relationships, finding causes and explanations. These variables are often plotted on X and Y axis on the graph for better understanding of data and one of these variables is independent while the other is dependent.


Common types of bivariate analysis include drawing scatter plot, regression analysis and finding correlation coefficients. A scatter plot is used to find out if there exists any relationship between two variables. Regression analysis is a statistical method for estimating the relationships between variables. Correlation coefficient analysis measures the strength and direction of a linear relationship between two variables on a scatter plot.


**Multivariate distribution**

When the dataset involves three or more variables, it is categorized under multivariate distribution.  Multivariate analysis is used to study more complex sets of data. It is usually unsuitable for small sets of data.

There are wide variety of analysis techniques to perform multivariate analysis. The choice of analysis techniques depends on the dataset and our goals to be achieved. Some examples of multivariate analysis techniques are additive tree, cluster analysis, correspondence analysis, factor analysis, MANOVA (multivariate analysis of variance), multidimensional scaling, multiple regression analysis, principal component analysis and redundancy analysis.


=================================================================================



## 4. Types of exploratory data analysis (EDA)


EDA is generally cross-classified in two ways. First, each method is either non-graphical or graphical. Second, each method is either univariate or multivariate (usually bivariate).  The non-graphical methods provide insight into the characteristics and the distribution of the variable(s) of interest. So, non-graphical methods involve calculation of summary statistics while graphical methods include summarizing the data diagrammatically.


There are four types of exploratory data analysis (EDA) based on the above cross-classification methods.  These are as follows:-


i.	**Univariate non-graphical EDA**

ii.	**Multivariate non-graphical EDA**

iii.	**Univariate graphical EDA**

iv.	**Multivariate graphical EDA**


Each of these types of EDA are described below:-


### i. Univariate non-graphical EDA


The objective of the univariate non-graphical EDA is to understand the sample distribution and also to make some initial conclusions about population distributions. Outlier detection is also a part of this analysis.


**Categorical data**


A simple tabulation of the frequency of each category is the best univariate non-graphical EDA for categorical data. So, a simple univariate non-graphical EDA method for categorical variables is to build a table containing the count and the fraction (or frequency) of data of each category.


**Quantitative data**

Univariate non-graphical EDA for a quantitative variable is a way to make preliminary assessments about the population distribution of the variable. The characteristics of the population distribution of a quantitative variable are its center, spread, modality (number of peaks in the pdf), shape and outliers. So, we plot characteristics of quantitative data which are **central tendency**, **spread**, and **shape of the distribution (skewness and kurtosis)**.


The most common measure of central tendency is the **mean**. For skewed distribution or when there is concern about outliers, 
the **median** may be preferred.


The **variance** and **standard deviation** are two useful measures of spread. The **variance** is the mean of the squares of the individual deviations. The **standard deviation** is the square root of the variance. For Normally distributed data, approximately 95% of the values lie within 2 sd of the mean.


The **IQR** is calculated using the boundaries of data situated between the 1st and the 3rd quartiles. In the same way that the median is more robust than the mean, the IQR is a more robust measure of spread than variance and standard deviation and should therefore be preferred for small or asymmetrical distributions. 


The **interquartile range (IQR)** can be calculated as follows:-


**IQR = Q3 – Q1**


**Skewness** is a measure of a distribution’s asymmetry. **Kurtosis** is a summary statistic communicating information about the tails (the smallest and largest values) of the distribution. Both quantities can be used as a means to communicate information about the distribution of the data when graphical methods cannot be used.



### ii. Multivariate non-graphical EDA


Multivariate non-graphical EDA techniques show the relationship between two or more variables in the form of either cross-tabulation or statistics.


**Cross-Tabulation**


**Cross-tabulation** is the basic bivariate non-graphical EDA technique. Cross-tabulation is an extension of tabulation method that works for categorical and quantitative data with only a few variables. For two variables, we build a two-way table with column headings that match the levels of one variable and row headings match the levels of the other variable. Then, we fill in the counts of all subjects that share a pair of levels. The two variables may be either exposure or outcome variables or one of each.


**Covariance and Correlation**


There are two other statistics that can be calculated for two categorical variables. It is their **Covariance and Correlation**.  Covariance and correlation measures the degree of the relationship between two random variables and examines how much they change together. 


A positive covariance means the variables are positively related (they move together in the same direction), while a negative covariance means the variables are negatively related (they move in negative direction). A problem with covariance is that its value depends on the scale of the values of the random variables. The larger the values of x and y, the larger the covariance. It makes it impossible for example to compare covariances from data sets with different scales. This issue can be fixed by dividing the covariance by the product of the standard deviation of each random variable, which gives Pearson’s correlation coefficient. Correlation is therefore a scaled version of covariance, used to assess the linear relationship between two variables. 


### iii. Univariate graphical EDA


In addition to finding the various sample statistics of univariate distribution (discussed above), we also look graphically at the distribution of the sample.  The non-graphical methods are quantitative and objective. They do not give full picture of the data. 
Hence, we need graphical methods, which are more qualitative in nature and presents an overview of the data. 
There are several univariate graphical EDA techniques which can be used to explore the data. These are as follows:-


**Histograms**


Histograms are among the most useful EDA techniques. It allows us to gain insight into our data, including distribution, central tendency, spread, modality and outliers. Histograms are bar plots of counts versus subgroups of an exposure variable. Each bar represents the frequency (count) or proportion (count divided by total count) of cases for a range of values. The range of data 
for each bar is called a bin. Histograms give an immediate impression of the shape of the distribution (symmetrical, skewed, 
outliers).


**Stem plots**


Stem and leaf plots (also called stem plots) are a simple substitution for histograms. They show all data values and the shape of the distribution.


**Boxplots**


Boxplots are interesting for representing information about the central tendency, symmetry, skewness and outliers. Boxplots show robust measures of location and spread as well as providing information about symmetry and outliers. But they can hide some aspects of the data such as multimodality. Boxplots are an excellent EDA technique because they rely on robust statistics like median and IQR.


**2-D line plots**


2D line plots represent graphically the values of an array on the y-axis, at regular intervals on the x-axis. 


**Probability plots** (Quantile-Normal Plot/QN Plot, Quantile-Quantile Plot/QQ Plot)


Probability plots are a graphical test for assessing if data follows a particular distribution. Quantile-Normal plots allow detection 
of non-normality and diagnosis of skewness and kurtosis. They are most often used for testing the normality of a data set, as many statistical tests have the assumption that the exposure variables are approximately normally distributed. These plots are also used to examine residuals in models that rely on the assumption of normality of the residuals (ANOVA or regression analysis for example).



### iv. Multivariate graphical EDA**


There are several useful multivariate graphical EDA techniques, which are used to look at the distribution of multivariate data. 
These are as follows:-


**Side-by-Side Boxplots**


Side-by-side boxplots are the best graphical EDA technique for examining the relationship between a categorical variable and a quantitative variable. Representing several boxplots side by side allows easy comparison of the characteristics of several groups of data. They allow us to check the distribution of the quantitative variable at each level of the categorical variable.


**Scatterplots**


For two quantitative variables, the basic graphical EDA technique is the scatterplot which has one variable on the x-axis, one on the y-axis and a point for each case in the dataset. If one variable is explanatory and the other is outcome, it is a strong convention to put the outcome on the y (vertical) axis.


**Curve Fitting**


Curve fitting is one way to quantify the relationship between two variables or the change in values over time. The most common method for curve fitting relies on minimizing the sum of squared errors (SSE) between the data and the fitted function.


**Heat Maps** and **3-D Surface Plots**


Heat maps are simply a 2D grid built from a 2D array, whose color depends on the value of each cell. The data set must correspond to a 2D array whose cells contain the values of the outcome variable. This technique is useful when we want to represent the change of an outcome variable as a function of two other variables.


The color mapping can be customized (e.g. rainbow or grayscale). The 3D equivalent is mesh plots or surface plots.


**Summary**

So, we should always perform appropriate EDA before further analysis of the data. We should perform the necessary steps to become more familiar with the data. We should check for mistakes, outliers and anomalies in the data. We should learn about variable distributions and relationships between variables.


I have summarized the above discussion in the following table.


=================================================================================



## 5. Exploratory data analysis (EDA) techniques


EDA techniques depend on the type of data and the objectives of the analysis.


The following table summarizes the useful EDA techniques based on the type of data:-


| Type of data              | EDA techniques         |
|---------------------------|------------------------|
| Categorical               | Descriptive statistics |
| Univariate discrete       | Barplot                |
| Univariate continuous     | Line plot, Histogram   |
| Bivariate continuous      | 2-D scatter plot       |
| 2-D arrays                | Heatmap                |
| Multivariate distribution | 3-D scatter plot       |
| Multiple groups           | Boxplot                |



The following table summarizes the useful EDA techniques depending on the objective:-


| Objective                                 | EDA techniques                                  |
|-------------------------------------------|-------------------------------------------------|
| Check the distribution of a variable     | Histogram                                       |
| Find outliers                             | Histogram, scatterplot, 
                                              box-and-whisker plot   
| Quantify relationship  between variables  | 2-D scatter plot,  
                                              covariance and correlation   
| Visualize relationship  between variables | Heatmap                                         |
| Visualize  high-dimensional data          | Principal component analysis,  3-D scatter plot |


=================================================================================


## 6. Objectives of exploratory data analysis


Before proceeding, we need to summarize the objectives of the EDA. The objectives of the EDA are as follows:-


i.	To get an overview of the distribution of the dataset.


ii.	Check for missing numerical values, outliers or other anomalies in the dataset.


iii.	Discover patterns and relationships between variables in the dataset.


iv.	Check the underlying assumptions in the dataset.


=================================================================================


## 7. Exploratory data analysis - prerequisites


We need two Python libraries for exploratory data analysis – NumPy and Pandas.


•	**NumPy** – NumPy is the fundamental Python library for scientific computing. It adds support for large and multi-dimensional 
arrays and matrices. It also supports large collection of high-level mathematical functions to operate on these arrays.


•	**Pandas** - Pandas is a software library for Python programming language which provide tools for data manipulation and analysis tasks. It will enable us to manipulate numerical tables and time series using data structures and operations.


We need two more libraries for data visualization purpose. These are Seaborn and Matplotlib.


•	**Seaborn** - Seaborn is a Python data visualization library based on Matplotlib. It provides a high level interface for drawing attractive and informative statistical graphics.


•	**Matplotlib** - Matplotlib is the core data visualization library of Python programming language. It provides an object-oriented 
API for embedding plots into applications.


=================================================================================


## 8. Import the required Python libraries


We have seen that we need two Python libraries – NumPy and Pandas for the exploratory data analysis process. Also, we need two more libraries – Seaborn and Matplotlib for data visualization purposes. We need to import these libraries before we actually start using them. We can import them with their usual shorthand notation as follows:-


`import numpy as np`


`import pandas as pd`


`import seaborn as sns`


`import matplotlib.pyplot as plt`


`%matplotlib inline`


=================================================================================


## 9. Dataset description

For this project, I have used the Absenteeism at work dataset. This dataset can be found at the following url-

https://archive.ics.uci.edu/ml/datasets/Absenteeism+at+work

The dataset consists of records of absenteeism at work from July 2007 to July 2010 at a courier company in Brazil. 
The dataset contains 740 number of instances and 21 number of attributes.


It was created by Andrea Martiniano, Ricardo Pinto Ferreira and Renato Jose Sassi.


Attribute information in the dataset is as follows:-

1.	ID – represents individual identification ID


2.	Reason for absence (ICD) – 


Absences attested by the International Code of Diseases (ICD) stratified into 21 categories (I to XXI) as follows: 


I Certain infectious and parasitic diseases 


II Neoplasms 


III Diseases of the blood and blood-forming organs and certain disorders involving the immune mechanism 


IV Endocrine, nutritional and metabolic diseases 


V Mental and behavioural disorders


VI Diseases of the nervous system 


VII Diseases of the eye and adnexa 


VIII Diseases of the ear and mastoid process


IX Diseases of the circulatory system 


X Diseases of the respiratory system


XI Diseases of the digestive system


XII Diseases of the skin and subcutaneous tissue


XIII Diseases of the musculoskeletal system and connective tissue 


XIV Diseases of the genitourinary system


XV Pregnancy, childbirth and the puerperium


XVI Certain conditions originating in the perinatal period 


XVII Congenital malformations, deformations and chromosomal abnormalities 


XVIII Symptoms, signs and abnormal clinical and laboratory findings, not elsewhere classified 


XIX Injury, poisoning and certain other consequences of external causes


XX External causes of morbidity and mortality 


XXI Factors influencing health status and contact with health services. 


And 7 categories without (CID) patient follow-up (22), medical consultation (23), blood donation (24), laboratory examination (25), unjustified absence (26), physiotherapy (27), dental consultation (28).


3.	Month of absence 


4. Day of the week (Monday (2), Tuesday (3), Wednesday (4), Thursday (5), Friday (6)) 


5. Seasons (summer (1), autumn (2), winter (3), spring (4))


6. Transportation expense 


7. Distance from Residence to Work (kilometers)


8. Service time 


9. Age 


10. Work load Average/day 


11. Hit target 


12. Disciplinary failure (yes=1; no=0) 


13. Education (high school (1), graduate (2), postgraduate (3), master and doctor (4)) 


14. Son (number of children) 


15. Social drinker (yes=1; no=0)


16. Social smoker (yes=1; no=0)


17. Pet (number of pet) 


18. Weight 


19. Height 


20. Body mass index


21. Absenteeism time in hours (target) 


=================================================================================


## 10. Import the dataset


We can import the dataset using the usual **read_csv()** function as follows:-


data = "C:/eda/Absenteeism_at_work.csv"


df = pd.read_csv(data, sep=";")


Generally, in the csv file the values are separated by a comma. So, there is no need to use the sep parameter which describes how the values are separated. In this case, the values are separated by semicolon (;). So, I used the sep = ";" parameter to denote that the values are separated by semicolon.


=================================================================================


## 11. Overview of the dataset


Now, we should get to know our data. We should know its dimensions, structure and column data types. 

We can proceed as follows:-


### df.shape attribute


The first thing that I do is to check the dimensions of the dataset. We can check the dimensions of the data with **df.shape** attribute as follows:-


`print(df.shape)`


The dataset has 740 rows and 21 columns.


### df.columns attribute


I can view the column names in the dataset with **df.columns** attribute.


### df.head() and df.tail() methods


Now, it is time to get an overview of the dataset. We can view the top five and bottom five rows of the dataset with **df.head()** 
and **df.tail()** methods respectively.


### df.info() method
We can get a concise summary of the dataset with **df.info()** method. This method prints information about a dataframe including the index, column names and data types, non-null values and memory usage.


### drop redundant columns


There are two columns `ID` and `Pet` which have no correlation with the target variable `Absenteeism time in hours`. So, we should drop these columns. We can do it as follows:-


`df.drop(['ID','Pet'], axis = 1, inplace=True)`


### df.describe() method


We can view the summary statistics of numerical columns with **df.describe()** method. It enable us to detect outliers in the data which require further investigation.


=================================================================================


## 12. Check for anomalies in the dataset


Now, we should check for any discrepancy in the dataset. 


### Check for missing numerical values


The first step is to check for any missing numerical values in the dataset. There are several commands that help us to check for 
any missing numerical values in the dataset. These are as follows:-


**df.isnull()**


The above command checks whether each cell in a dataframe contains missing values or not. If the cell contains missing value, 
it returns true otherwise it returns false. 


**df.isnull.sum()**


The above command returns the total number of missing values in each column in the dataset.


**isna()** and **notna()** functions to detect ‘NA’ values


Pandas provides isna() and notna() functions to detect ‘NA’ values. These are also methods on Series and DataFrame objects.



### Examples of **isna()** and **notna()** commands


**detect ‘NA’ values in the dataframe**	


`df.isna()`


**detect ‘NA’ values in a particular column in the dataframe**


`pd.isna(df[‘col_name’])`


`df[‘col_name’].notna()`


### Encode missing numerical values


Missing values are encoded in different ways. They can appear as ‘NaN’, ‘NA’, ‘?’, zero ‘0’, ‘xx’, minus one ‘-1’ or a blank space “ ”. We need to use various pandas methods to deal with missing values. But, pandas always recognize missing values as ‘NaN’.  So, it is essential that we should first convert all the ‘?’, zeros ‘0’, ‘xx’, minus ones ‘-1’ or blank spaces “ ” to ‘NaN’. If the missing values isn’t identified as ‘NaN’, then we have to first convert or replace such non ‘NaN’ entry with a ‘NaN’.


**Convert '?' to 'NaN'**


`df[df == '?'] = np.nan`


I have discussed several methods to deal with missing numerical values:-


### Drop missing values with dropna() method


This is the easiest method to handle missing values. In this method, we drop labels or columns from a data set which refer to missing values. 


**drop labels or rows from a data set containing missing values**

`df.dropna (axis = 0)`


 **drop columns from a data set containing missing values**

`df.dropna(axis = 1)`


This is the Pandas dataframe **dropna()** method. An equivalent **dropna()** method is available for Series with same functionality.


To drop a specific column from the dataframe, we can use drop() method of Pandas dataframe.


**drop col_name column from Pandas dataframe**

`df.drop(‘col_name’, axis = 1)`



**A note about axis parameter** 

Axis value may contain (0 or ‘index’) or (1 or ‘columns’). Its default value is 0.

We set axis = 0 or ‘index’ to drop rows which contain missing values.

We set axis = 1 or ‘columns’ to drop columns which contain missing values.


After dropping the missing values, we can again check for missing values and the dimensions of the dataframe.


**again check the missing values in each column**


`df.isnull.sum()`


**again check the dimensions of the dataset**


`df.shape`


But, this method has one disadvantage. It involves the risk of losing useful information. Suppose there are lots of missing values 
in our dataset. If drop them, we may end up throwing away valuable information along with the missing data. It is a very grave 
mistake as it involves losing key information. So, it is only advised when there are only few missing values in our dataset.
So, it's better to develop an imputation strategy so that we can impute missing values with the mean or the median of the row or 
column containing the missing values.



### Fill missing values with a test statistic


In this method, we fill the missing values with a test statistic like mean, median or mode of the particular feature the missing 
value belongs to. One can also specify a forward-fill or back-fill to propagate the next values backward or previous value forward.


**Filling missing values with a test statistic like mean**


`mean = df['col_name'].mean()`


`df['col_name'].fillna(value = mean, inplace = True )`


**We can also use replace() in place of fillna()**


`df[‘col_name’].replace(to_replace = NaN, value = mean, inplace = True)`


### Check with ASSERT statement

We should check for missing values programmatically. If we drop or fill missing values, we expect no missing values. We can write an assert statement to verify this. So, we can use an assert statement to programmatically check that no missing or unexpected ‘0’ value is present. This gives confidence that our code is running properly.


Assert statement will return nothing if the value being tested is true and will throw an AssertionError if the value is false.


Asserts


•	assert 1 == 1   (return Nothing if the value is True)


•	assert 1 == 2   (return AssertionError if the value is False)


**assert that there are no missing values in the dataframe**


`assert pd.notnull(df).all().all()`


**assert that there are no missing values for a particular column in dataframe**


`assert df.column_name.notnull().all()`


**assert all values are greater than or equal to 0**


`assert (df >=0).all().all()`



**assert no entry in a column is equal to 0**
`assert (df['column_name']!=0).all().all()`


=================================================================================


## 13. Univariate analysis


### Measures of central tendency and dispersion


**Central tendency** means a central value which describe a probability distribution. It may also be called a center or location 
of the distribution. The most common measures of central tendency are the **arithmetic mean**, the **median** and the **mode**. 
The most common measure of central tendency is the **mean**. For skewed distribution or when there is concern about outliers, 
the **median** may be preferred. So, **median** is more robust measure than the mean.


**Dispersion** is an indicator of how far away from the center, we can find the data values. The most common measures of dispersion are **variance**, **standard deviation** and **interquartile range (IQR)**. **Variance** is the standard measure of spread. The **standard deviation** is the square root of the variance. The **variance** and **standard deviation** are two useful measures of spread. 


A third measure of spread is the **interquartile range (IQR)**. The IQR is calculated using the boundaries of data situated between the 1st and the 3rd quartiles. So, IQR can be calculated as **IQR = Q3 - Q1**. It is a robust measure of spread.


### Measures of shape


Now, we will take a look at measures of shape of distribution. There are two statistical measures that can tell us about the shape of the distribution. These measures are **skewness** and **kurtosis**. These measures can be used to convey information about the shape of the distribution of the dataset.


### Skewness


**Skewness** is a measure of a distribution's symmetry or more precisely lack of symmetry. It is used to mean the absence of symmetry from the mean of the dataset. It is a characteristic of the deviation from the mean. It is used to indicate the shape of the distribution of data.


### Negative skewness


Negative values for skewness indicate negative skewness. In this case, the data are skewed or tail to left. By skewed left, we mean that the left tail is long relative to the right tail. The data values may extend further to the left but concentrated in the right. So, there is a long tail and distortion is caused by extremely small values which pull the mean downward so that it is less than the median. Hence, in this case


**Mean < Median < Mode**


### Zero skewness


Zero skewness means skewness value of zero. It means the dataset is symmetrical. A data set is symmetrical if it looks the same to the left and right to the center point. The dataset looks bell shaped or symmetrical. A perfectly symmetrical data set will have a skewness of zero. So, the normal distribution which is perfectly symmetrical has a skewness of 0. So, in this case


**Mean = Median = Mode**


### Positive skewness


Positive values for skewness indicate positive skewness. The dataset are skewed or tail to right. By skewed right, we mean that the right tail is long relative to the left tail. The data values are concentrated in the right. So, there is a long tail to the right 
that is caused by extremely large values which pull the mean upward so that it is greater than the median. So, we have


**Mean > Median > Mode**


### Reference range on skewness values


The rule of thumb for skewness values are:


•	If the skewness is between -0.5 and 0.5, the data are fairly symmetrical.


•	If the skewness is between -1 and – 0.5 or between 0.5 and 1, the data are moderately skewed.


•	If the skewness is less than -1 or greater than 1, the data are highly skewed.


We have looked at the measures of central tendency of the data (mean and median) and spread of the data (standard deviation (std), interquartile range (IQR), minimum (min) and maximum (max) values. These quantities can only be used for quantitative variables not 
for categorical variables.


### Kurtosis


Kurtosis is the degree of peakedness of a distribution.


Data sets with high kurtosis tend to have a distinct peak near the mean, decline rather rapidly and have heavy tails.


Data sets with low kurtosis tend to have a flat top near the mean rather than a sharp peak. 


### Reference range for kurtosis


The reference standard is a normal distribution, which has a kurtosis of 3. Often, **excess kurtosis** is presented instead of kurtosis, where **excess kurtosis** is simply **kurtosis - 3**. 


**Mesokurtic curve**


A normal distribution has kurtosis exactly 3 (**excess kurtosis** exactly 0). Any distribution with kurtosis ≈3 (excess ≈ 0) is 
called **mesokurtic**.


**Platykurtic curve**


A distribution with kurtosis < 3 (**excess kurtosis** < 0) is called **platykurtic**. As compared to a normal distribution, its 
central peak is lower and broader, and its tails are shorter and thinner.


**Leptokurtic curve**


A distribution with kurtosis > 3 (**excess kurtosis** > 0) is called **leptokurtic**. As compared to a normal distribution, 
its central peak is higher and sharper, and its tails are longer and fatter.


### Distribution of target variable


Now, we should plot the distribution of target variable. We can use Seaborn's **distplot()** function to plot the distribution.


First, I will draw the plot using **distplot()** function. This function plot a univariate distribution of observations. 


This function combines the matplotlib **hist()** function with the seaborn **kdeplot()** function.


### Findings of univariate analysis


Findings of univariate analysis are as follows:-


•	The target variable `Absenteeism time in hours` is highly positively skewed.

•	Its distribution curve is a **Leptokurtic curve**. Its central peak is higher and sharper and its tails are longer and fatter.

•	The `Absenteeism time in hours` data values follow the lognormal distribution relatively closely as compared to normal distribution.


=================================================================================


## 14. Multivariate analysis


### Examine relationship between target variable and categorical attributes


In the dataset, we have several categorical attributes like `Seasons`, `Education`, `Social drinker` and `Social smoker`. 
In this section, I will explore the relationship between these categorical attributes and target variable.


### Frequency distribution and visualization of categorical attributes


`Seasons` is a categorical attribute. We can find out what categories exist and how many values belong to each category using the `value_counts ()` method.


Similarly, `Education`, `Social drinker` and `Social smoker` are also categorical attributes. We can visualize their frequency distribution using the value_counts() method and visualize them.


### Findings of multivariate analysis


Findings of multivariate analysis are as follows:-


•	The spring season contains highest number of `Absenteeism time in hours`.


•	The high school category consists of highest number of `Absenteeism time in hours`.


•	The `Social drinker` category have higher number of `Absenteeism time in hours`.


•	The `Social smoker` category have lesser number of `Absenteeism time in hours`.


### Estimating correlation coefficients


Our dataset is very small. So, we can compute the standard correlation coefficient (also called Pearson's r) between every pair of attributes. We can compute it using the `df.corr()` method.


Our target variable is `Absenteeism time in hours`. So, we should check how each attribute correlates with the `Absenteeism time in hours` variable.


**Interpretation of correlation coefficient**


The correlation coefficient ranges from -1 to +1. 


When it is close to +1, this signifies that there is a strong positive correlation. So, we can see that there is a small positive correlation between `Absenteeism time in hours` and `Height`. 


When it is clsoe to -1, it means that there is a strong negative correlation. So, there is a small negative correlation between `Absenteeism time in hours` and `Reason for absence`.


When it is close to 0, it means that there is no correlation. So, there is no correlation between `Absenteeism time in hours` and `Seasons`.


### Discover patterns and relationships 


An important step in EDA is to discover patterns and relationships between variables in the dataset. We will use the following graphs and plots to explore the patterns and relationships in the dataset.


•	Correlation Heat Map


•	Pair Plot


•	Scatter Plot


•	Box Plot


### Findings of multivariate analysis


Findings of multivariate analysis are as follows:-


•	`Month of absence` and `Seasons` are positively correlated (correlation coefficient = 0.41).


•	`Body mass index` and `Service time` are positively correlated (correlation coefficient = 0.50).


•	Smilarly, `Body mass index` and `Age` are positively correlated (correlation coefficient = 0.47).


•	Also, `Body mass index` and `Weight` are highly positively correlated (correlation coefficient = 0.90).


•	The pair plot confirms that there is strong positive correlation between `Service time` and `Age`.


•	Similarly, `Distance from Residence to Work` and `Transportation expense` are positively correlated.


•	There is a mildly positive correlation between `Absenteeism time in hours` and `Height`. Majority of data values lie below the fitted regression line.


•	There is a weak correlation between `Absenteeism time in hours` and `Son`.


•	There is a strong positive correlation between `Body mass index` and `Service time`. Approximately, half of the data values lie below the fitted regression line and half of the values lie above it.


•	The people aged 34 or 58 have highest number of `Absenteeism time in hours`.


•	The people who have 2 sons have highest number of `Absenteeism time in hours`.


=================================================================================


## 15. References


The ideas and concepts in this project are taken from the following books and websites:-


https://en.wikipedia.org/wiki/Exploratory_data_analysis


https://www.statisticshowto.datasciencecentral.com/probability-and-statistics/types-of-variables/


https://medium.com/@InDataLabs/why-start-a-data-science-project-with-exploratory-data-analysis-f90c0efcbe49


https://www.datacamp.com/community/tutorials/exploratory-data-analysis-python


https://www.kaggle.com/ekami66/detailed-exploratory-data-analysis-with-python


Think Stats – Exploratory Data Analysis in Python by Allen B. Downey








