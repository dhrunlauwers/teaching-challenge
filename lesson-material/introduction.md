# Introduction - Data Wrangling with Pandas

## Who am I?
<img style="float: left;" src="./images/dhrun.PNG" width="160" height="163">

    Name: Dhrun Lauwers 
    Born: Antwerp, Belgium 
    Lives: Toronto, Canada 
    Interests: Food, technology, physical movement 
    Occupation: Leading a small team of data scientists and engineers for a large retail company in Canada.


## What is data wrangling?

![](./images/wrangler.jpg)

In North America, a **wrangler** is someone who is employed to handle animals professionally, especially horses. They would round up and take care of the cattle for ranchers and cowboys to use.

**Data wrangling** is the process of accessing and transforming data so that the result can be easily summarized for analysis and other purposes. This process is typically carried out by data engineers, who prepare data for the data scientists to analyze.

Data can come in various forms and can be accessed in several different ways, but the process of cleaning and transforming data stays more or less the same.

### The data wrangling process
1. Read the data into a structured form (like Pandas data structures below)
2. Investigate the data to find missing values, outliers, and other potential problems
3. Clean the data to fix the issues identified
4. Use data for analysis or other purposes

### Why is it an important skill?

> 80% of the data analysis process is spent cleaning and preparing data

Data sources used in academics tend to be pre-processed and much cleaner than data used in the industry, so this is a very important skill to develop when you start working in the field.

Data preparation is not just a first step, but must be repeated many times over the course of analysis as new problems come to light or new data is collected.

![](./images/real-data.jpg)

## What is clean data?

> Happy families are all alike; every unhappy family is unhappy in its own way <br>
\- Leo Tolstoy

There is no easy to follow set of rules when it comes to cleaning data because it usually depends on what you intend to do with the data. However, there are some general guidelines we can learn from:
1. Data should be stored in a structured format, with labeled rows and columns
2. Each row in the dataset represents and observation (a person, an object, an event)
3. Each column describes a characteristic of the observation (a person's height or name)
4. Each type of observation is stored in a separate table (don't mix people with objects)

For more details on what clean data really means, check out the paper on Tidy Data in referenes section below.

## What is Pandas?

Pandas is the most widely used data analysis library created for Python, and it has many built-in functions that will help with data wrangling.

As with all libraries, it's important to get some practice using them and to make sure to read the documentation. See the references section for a link to the official Pandas documentation, as well as some links to practice courses.

### Data structures

Pandas is short for *panel-data*, which refers to the nature of the way data is stored in Pandas.

Pandas allows us to store our data in different data structures represented by Python objects, and to perform operations on these objects. The most common data structures include:
1. Series: A one-dimensional array of data with labels. 
2. DataFrame: A two-dimensional array of data with labelled rows and columns.

![](./images/series-and-dataframe.png)

### Common functions

Once our data is stored in one of the two data structures, pandas has many different functions we can use to manipulate and summarize data. This not only includes operations on a single data structure, like adding, removing data and summarizing data, but also includes operations on multiple data structures to combine them.

Some common operations include:
- checking for outliers in your data, and deciding what to do with them (keep or remove)
- filtering your dataset (AKA slicing) based on one or more conditions
- adding new rows or columns by combining or splitting existing rows or columns

For a complete list of all functions, see Pandas documentation in the references section below.

### Missing data

It's very common that you will get a dataset where values for certain observations are missing. A large number of missing values could affect the analysis, so they will have to either be removed or filled in with an estimate.

Some useful functions for working with missing values include:
- `isnull()`: Generates a boolean indicating missing values.
- `fillna()`: Returns a copy of the data with missing values filled in
- `dropna()`: Returns a filtered version of the data without missing values

There are many ways of estimating missing values that cannot be covered in the scope of this lesson. Please take a look at the reference section below if you are interested in learning more.

## Data wrangling with Pandas
Now to get wrangling! Open up the [Jupyter notebook associated with this lesson](./demonstration.ipynb) and lets get started.

## References

[Tidy Data - Hadley Wickham, Journal of Statistical Software](https://vita.had.co.nz/papers/tidy-data.pdf)

[Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)

[Pandas - Intro to Data Structures](https://pandas.pydata.org/pandas-docs/stable/getting_started/dsintro.html)

[Pandas Practice - w3 resource](https://www.w3resource.com/python-exercises/pandas/index.php)

[Pandas Practice](https://github.com/guipsamora/pandas_exercises)

[Missing Data](https://jakevdp.github.io/PythonDataScienceHandbook/03.04-missing-values.html)


