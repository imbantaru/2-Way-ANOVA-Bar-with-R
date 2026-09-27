# <p>  <b>2-WAY ANOVA + Graph </b> </p>
**Introduction to ANOVA**

A two-way ANOVA (two-way analysis of variance) is a statistical test used to find out how two categorical independent variables affect one continuous dependent variable
Or simpled as you want to test 2 categorical independent variables
e.g. variable A & variable B effect both and individually to dependent variable.

This was used in one of my research to determine how significant treatments to dependent variable -> mine was height, diameter, etc.
For the Script check for the **script** file. Below [here](README.md/#Breakdown) will explain for each code

# </b> Breakdown </p>
R uses packages to run a task, and to load a package type `library()` in the terminal

### 1st - Data Preparation
To load your .xlsx / excel file use `readxl` package
~~~
library(readxl)
~~~

`dplyr` used for data manipulation, e.g grouping, arranging, filtering
~~~
library(dplyr)
~~~

**(Optional)** mine was used for agricultural research so package `agricolae` really helpful for the tests
~~~
library(agricolae)
~~~

We're going to set our .xlsx file as the environment with
~~~
(environment name) <- (your excel file)
~~~
Feel free to use any name you like. But keep in mind that **R is highly sensitive** to typo, uppercase/lowercase, so choose wisely.

After this, we will set our independent variable as the factor R recognize by
~~~
(environment name)$(your 1st factor) <- as.factor(environment name$your 1st factor)
(environment name)$(your 2nd factor) <- as.factor(environment name$your 2nd factor)
~~~

