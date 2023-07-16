# SIGAI-Task description
Objective:
The main aim of the task is to analyze the given dataset and use different preprocessing techniques to enhance it.

The dataset used here is a heart disease statlog with no missing values(Heart_diseases_statlog.csv).
Python libraries such as pandas and NumPy are used to analyze datasets and numerical values in datasets respectively.

* **Loading the dataset**
  
Using pd.read_csv(‘Heart_diseases_statlog.csv’) the dataset is loaded/read into a variable named dataset.

* **Analysing a few rows**
  
Using describe() function, the description of the dataset is displayed. It mainly displays the standard, median, maximum, minimum, etc.
The shape of a dataset returns a tuple of array dimensions that return the number of rows and columns that exist in the dataset.
The head function returns the number of rows specified from the dataset. It returns the first five rows if the number is not mentioned.

* **Plotting Graphs**
  
Matplotlib is one of the most popular graphing and data visualization libraries for Python.
Four graphs are displayed using hist(), scatter(), bar(), plot() function a- histogram, scatter plot, bar graph, and line graph with multiple sets of data plotted respectively.

* **Null values**
  
In the given dataset, there are no null values, that is it is a clean dataset.
Using null () and sum(), the number of null values present in each column is displayed(in this case no column indicated to have null values).
The dropna() function removes the rows with null values from the dataset to achieve a cleaner dataset.

* **Standardization**
  
In statistics and machine learning, data standardization is a process of converting data to z-score values based on the mean and standard deviation of the data.

The Z-score value is given by:

For each feature, we will compute its mean and standard deviation. Then we will subtract the mean from each observation and divide it by the standard deviation to get the standardized values.

The resulting standardized value shows the number of standard deviations the raw value is away from the mean, allowing us to compare multiple features and get more relevant information since now all the data will be on the same scale.
The standardised data will have its mean value equal to zero and the values range between +3 and -3.

Python sklearn library offers us with StandardScaler() function to standardize the data values into a standard format. Further, fit_transform() is used along with the assigned object to transform and standardize the data.

* **Correlation matrix**
  
A correlation matrix is a table containing correlation coefficients between variables. Each cell in the table represents the correlation between two variables. The value lies between -1 and 1.
To create a correlation matrix, the corr() function is used on the given dataset.
