<h1 align="center"> Learn Python for Data Analysis </h1>

I am building this repository for study purposes. I am on the journey to become a Data Analyst, and I want to share what I have learned along the way.

## Prerequisites
1. Python 3.x version
2. Git is installed and you know basics of [git commands.](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)
3. Have access and know [how to use terminal/command line.](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands)

## About the Content

The content of this repository is organized by levels. First, we start with basic programming concepts using Python. Next, we delve into the world of data analysis and its theories. Finally, we bring everything together and start exploring Python for data analysis. For each section, we will complete at least one project.

Note 1: All of this content is written in the form of "notes" by me. I encourage you to take some time and read the official documentation for the Python language and its libraries. I will always provide these references and others at the end of each topic.

Note 2: At the time of viewing this, I may still be in the process of developing the content and updating this repository. As a result, you may encounter some unclickable topics. The updates to these topics do not follow a specific order and are based on my needs and study progress. Follow me to stay updated on new upgrades.

### Python Introduction Level

1. Why you should learn programming?
2. Why Python?
3. Installing Python and setting up the environment.
4. Baby steps with Python. 
5. What is Logic programming and Pseudocode?
6. Variables, Types and Data Structures.
7. Loops, Condititionals, Methods and Functions.
8. Modules, Packages, Built-in Functions and File handling. 

### Python Basic Level

1. Oriented Object Programming.
2. Math and Numpy.
3. Data handling with Pandas.
4. Data Visualization with Matplotlib and Seaborn.

### Python Intermediary Level

1. Data Analysis with Statsmodel.
2. Temporal series Analysis.
3. Machine Learning with Scikit-Learn.
4. Deep Learning with TensorFlow.
5. Reinforcement Learning.

### Data Analysis

1. What are Data? Why should we care about it?
2. What is Data Analysis?
3. What are the key points that this area helps business?
4. Data Analysis Life Cycle.
5. Data Types.
6. Data Analysis types.
7. Cleaning Data Strategies.
8. Handling with missing values.
9. Transforming and Enconding Variables.
10. Math and Statistics for Descriptive Analysis.
11. Web Scraping and Data Analysis.
12. Attribute Engineering.
13. Data Prepocessing.
14. Data Visualization Design.

### Libraries

Note: The purpose of this section is not to cover all Python libraries - this is not even possible. The main goal of this repository section is to delve deeper into libraries that I may be using during my studies and popular ones that I may use in the future.

#### 1. Pandas

About:

- Pandas is a Python library used for data analysis and manipulation. Provides high level data structures for efficiently storing large datasets and tools for working with them. [Official documentation.](https://pandas.pydata.org/docs/index.html)

Simple Example using Pandas to create a DataFrame and perfom some basic operations:

```Python

import pandas as pd

# Creating a DataFrame from a dictionary

data = {'Name': ['John', 'Jane', 'Jim', 'Joan'],
        'Age': [29, 31, 27, 35],
        'Country': ['USA', 'UK', 'Canada', 'Australia']}
df = pd.DataFrame(data)

# Display the DataFrame
print(df)

# Selecting rows based on condition
df = df[df['Age'] > 30]

# Sorting the DataFrame
df = df.sort_values(by='Age', ascending=False)

# Display the DataFrame after sorting
print(df)

```

Code Anatomy:

- `import pandas as pd`: Imports the Pandas library and renames it as "pd".
- `data = {'Name': ['John', 'Jane', 'Jim', 'Joan'],'Age': [29, 31, 27, 35], 'Country': ['USA', 'UK', 'Canada', 'Australia']}`: Creates a dictionary of data with three columns - Name, Age, and Country.
- `df = pd.DataFrame(data)`: Creates a Pandas DataFrame from the dictionary.
- `print(df)`: Prints the DataFrame.
- `df = df[df['Age'] > 30]`: Selects rows from the DataFrame where the age is greater than 30.
- `df = df.sort_values(by='Age', ascending=False)`: Sorts the DataFrame in descending order of age.
- `print(df)`: Prints the DataFrame after sorting.

#### 2. Matplotlib

About:

- Matplotlib is a Python library used for data visualization. Its help you to create a various types of static, animated and interactive visualizations. [Official documentation.]( https://matplotlib.org/ )

Example using Matplotlib to create a line plot:
impor
```python
 
import matplotlib.pyplot as plt

# Data to plot
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

# Creating the plot
plt.plot(x, y)

# Adding labels to the plot
plt.xlabel('X axis')
plt.ylabel('Y axis')

# Adding title to the plot
plt.title('Line Plot Example')

# Showing the plot
plt.show()
```

Code Anatomy:

- `import matplotlib.pyplot as plt`: Imports the Matplotlib library and renames it as "plt" for ease of use.
- `x = [1, 2, 3, 4, 5]`: Creates a list of values for the x-axis.
- `y = [2, 4, 6, 8, 10]`: Creates a list of values for the y-axis.
- `plt.plot(x, y)`: Creates a line plot using the x and y values.
- `plt.xlabel('X axis')`: Adds a label to the x-axis.
- `plt.ylabel('Y axis')`: Adds a label to the y-axis.
- `plt.title('Line Plot Example')`: Adds a title to the plot.
- `plt.show()`: Displays the plot.

#### 3. NumPy

About: 

- NumPy is a library in Python used for numerical computing and data manipulation. It provides a high-perfomance multidimensional array object and tools for working with these arrays. [Official documentation.]( https://numpy.org/ )

Example with NumPy to create arrays:

```python

import numpy as np

# Creating a 1D array
a = np.array([1, 2, 3, 4, 5])

# Creating a 2D array
b = np.array([[1, 2, 3], [4, 5, 6]])

# Finding the shape of an array
print(a.shape)
print(b.shape)

# Reshaping an array
b = b.reshape(3, 2)

# Finding the shape of the reshaped array
print(b.shape)

# Finding the sum of all elements in an array
print(a.sum())

# Finding the mean of all elements in an array
print(a.mean())

```

Code Anatomy:

- `import numpy as np`: Imports the NumPy library and renames it as "np" for ease of use.
- `import numpy as np`import numpy as np: Creates a one-dimensional NumPy array with values [1, 2, 3, 4, 5].
- `b = np.array([[1, 2, 3], [4, 5, 6]])`: Creates a two-dimensional NumPy array with values [[1, 2, 3], [4, 5, 6]].
- `print(a.shape)`: Prints the shape of the a array, which is (5,).
- `print(b.shape)`: Prints the shape of the b array, which is (2, 3).
- `b = b.reshape(3, 2)`: Reshapes the b array from shape (2, 3) to shape (3, 2).
- `print(b.shape)`: Prints the shape of the reshaped b array, which is (3, 2).
- `print(a.sum())`: Prints the sum of all elements in the a array, which is 15.
- `print(a.mean())`: Prints the mean of all elements in the a array, which is 3.

#### 4. Seaborn

About: 

- Seaborn is a Python library used for statistical data visualization. It provides a high-level interface for creating beautiful and informative statistical graphics. Seaborn is built on top of Matplotlib and provides a more convenient and simple way to create plots. [Official documentation.]( https://seaborn.pydata.org/ )

Example using Seaborn to create a bar plot:

```python

import seaborn as sns
import matplotlib.pyplot as plt

# Creating a sample data set
data = {"A": [1, 2, 3, 4, 5], "B": [2, 4, 6, 8, 10]}

# Creating a bar plot using Searbon
sns.barplot(data=data, x="A", y="B")

# Adding labels to the plot
plt.xlabel('X axis')
plt.ylabel('Y axis')

# Adding title to the plot
plt.title('Bar Plot Example')

# Showing the plot
plt.show()

```

Code Anatomy:

- `import seaborn as sns`: Imports the Seaborn library and renames it as "sns" for ease of use.
- `import matplotlib.pyplot as plt`: Imports the Matplotlib library and renames it as "plt" for ease of use.
- `data = {"A": [1, 2, 3, 4, 5], "B": [2, 4, 6, 8, 10]}`: Creates a sample data set with two columns "A" and "B".
- `sns.barplot(data=data, x="A", y="B")`: Creates a bar plot using the Seaborn library. The data argument specifies the data set to use, and the x and y arguments specify the columns to use for the x-axis and y-axis, respectively.
- `plt.xlabel('X axis')`: Adds a label to the x-axis.
- `plt.ylabel('Y axis')`: Adds a label to the y-axis.
- `plt.title('Bar Plot Example')`: Adds a title to the plot.
- `plt.show()`: Displays the plot.

#### 5. BeautifulSoup

About: 

- BeautifulSoup is a Python Library used for web scraping and parsing HTML and XML documents. It provides a simple way to extract data from HTML and XML documents and navigate through the tree-like structure of the documents.

Example using BeautifulSoup to scrape the title of the top news articles from the BBC News website:

```python

import requests
from bs4 import BeautifulSoup

# Sending a GET request to the webpage
url = 'https://www.bbc.com/news'
response = requests.get(url)

# Checking if the request was successful
if response.status_code == 200;
       # Parsing the HTML content of the page
       soup = BeautifulSoup(response.text, 'html.parser')
       
       # Finding all the article tags
       article_tags = soup.find_all('h3', {'class': 'gs-c-promo-heading__title'})
       
       # Extracting the text from each article tag
       articles = [article_tag.text.strip() for article_tag in article_tags]
       
       # Printing the titles of the articles
       print(articles)
else:
       print('Failed to retrieve the page')

```

Code Anatomy:

- `import requests`: Imports the requests library, which is used to send HTTP requests.
- `from bs4 import BeautifulSoup`: Imports the Beautiful Soup library.
- `url = 'https://www.bbc.com/news'`: Specifies the URL of the BBC News homepage.
- `response = requests.get(url)`: Sends a GET request to the specified URL and stores the response in the "response" variable.
- `if response.status_code == 200:`: Checks if the request was successful by checking the status code of the response. A status code of 200 means that the request was successful.
- `soup = BeautifulSoup(response.text, 'html.parser')`: Parses the HTML content of the page and creates a Beautiful Soup object. The response.text argument specifies the HTML content to parse, and the 'html.parser' argument specifies the HTML parser to use.
- `article_tags = soup.find_all('h3', {'class': 'gs-c-promo-heading__title'})`: Searches for all the "h3" tags with the class gs-c-promo-heading__title, which correspond to the titles of the articles.
- `articles = [article_tag.text.strip() for article_tag in article_tags]`: Extracts the text from each article tag and creates a list of article titles. The strip() method is used to remove any leading or trailing whitespace from the text.
- `print(articles)`: Prints the list of article titles.
- `else:`: Executed if the request was not successful.
- `print('Failed to retrieve the page')`: Prints an error message.

#### 6. Scikit-Learn

under development.

#### 7. TensorFlow

under development.

#### 8. Selenium

under development.

#### 9. StatsModels

under development.

#### 10. SciPy

under development.

#### 11. PyTorch

under development.

#### 12. Keras

under development.


## Contact me 🔗 👇 

<a href="https://github.com/soareseric/" target="blank"><img align="center" src="https://img.shields.io/github/followers/soareseric?label=Follow&style=social&link=https://github.com/soareseric/" alt="EricSoares" height="20" width="90" /></a>
<a href="https://www.linkedin.com/in/eric-soares-maciel" target="blank"><img align="center" src="https://img.shields.io/badge/-EricSoares-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/eric-soares-maciel/" alt="EricSoares" height="20" width="100" /></a>
