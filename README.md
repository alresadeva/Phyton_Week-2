# Python for Data Analyst 2
Second week of Python learning


## Function
Python Function is a block of statements that return the specific task. The idea is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again for different inputs, we can do the function calls to reuse code contained in it over and over again.
- In mathematics, a function is a process that relates between an input and an output.
- In Python, apart from these relationship functions, functions are also a way to organize code with the ultimate goal of code being reusable.
- Functions are defined with the def keyword followed by the function name and parameters in brackets ()
- Optionally, a docstring can be added - a documentation string that describes the context of the function


   ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/33128cda-8c51-4827-9152-4fdc5cf74b62)



- By default, Python will position according to the registration order in which it was defined, and must be called in that order.


  ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/18b26c95-5b80-410d-b298-9519ae299f81)  


### Return
The Phython Return statement is a special statement that can use inside in function or method to send the function’s result back to the caller. A Return statement consist of the return keyword followed by an optional return value. The return value of a Python function can be any Python object.


  ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/e9517f2b-3be4-41af-a1a8-81b2b755ef9f)


- The return value of a function can be stored in a variable.
- This will differentiate a function that returns a value from a function that does not return a value (often referred to as a procedure).

      ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/5b4a3c5e-d401-4bca-bf73-cb6ebd116d93)



### Pass by reference vs value
The difference between pass-by-reference and pass-by-value is that modifications made to arguments passed in by reference in the called function have effect in the calling function, whereas modifications made to arguments passed in by value in the called function can not affect the calling function.


![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/aa175aeb-d2cc-4334-8612-fef6662a0c98)


### NUMPY

**What is NumPy?**

NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, fourier transform, and matrices. NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely. NumPy stands for Numerical Python.

At the core of the NumPy package, is the ndarray object. This encapsulates n-dimensional arrays of homogeneous data types, with many operations being performed in compiled code for performance. There are several important differences between NumPy arrays and the standard Python sequences:
1. NumPy arrays have a fixed size at creation, unlike Python lists. Changing the size of an ndarray will create a new array and delete the original.
2. The elements in a NumPy array are all required to be of the same data type, and thus will be the same size in memory.

**The next step is how to apply NumPy in Python**

1. **Checking NumPy Version**

The “print(np.version)" syntax is used to determine the installed version of NumPy in Python.


> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/cc764d69-fc93-4a0f-a4e0-baa7d85e0ada)



2. **Import NumPy**
The “import numpy as np” statement is used to import the NumPy library into Python, allowing you to use its functions for numerical calculations and array manipulations.


> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/9bd4fc95-a8f9-441c-a43e-2e8c9fce0def)



3. **Creating a NumPy Array**
To create an ndarray, we can pass a list, tuple or any array-like object into the array() method, and it will be converted into an ndarray.

The syntax used to create a NumPy array from a list or tuple is the same, the only difference being the use of square brackets for a list [ ] and parentheses for a tuple ().
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/c4e877d7-95cb-484f-8785-c548467e61d6)
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/e759a79b-e90c-417c-8023-638bf96811a6)

**4. Creating an array with specific dimensions**

- 1 dimension: 1D arrays in NumPy are essentially like lists in Python. They are sequences of elements arranged in a single line.

> 

![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/175e20ce-f468-4dac-bd72-950f0309955a)



- 2 dimension: 2D arrays in NumPy are like matrices. They have rows and columns, arranged in a grid format.

> 

![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/46085bfc-4680-4901-bd97-bc3ee3dd4987)



- Creating a 3-dimensional array with two 2-dimensional arrays, both containing two arrays, can be achieved using NumPy as follows:

> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/13a84ff6-6927-4c2c-889a-a93213c408ee)



**5. Check how many dimensions the arrays have**
The "a = np.array" syntax is used to store an array variable into the NumPy library. And the "print(a.ndim)" syntax is used to provide feedback by displaying dimensional information to the user.
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/916e469c-463b-4c7f-b25f-8729a3038b34)

**6. Changing one dimension to another**
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/7a686faf-50b0-4f7f-915e-0a857417c8e6)

The syntax "ndmin=5" is used to reshape the dimension created into the fifth dimension.

**7. Get the results of the desired elements of the following array**

- Get the first element from the following array

> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/e95966ba-a2d6-4dfc-be9b-a303c8de616d)

> To retrieve the first element, you use [0] because the indexing of elements starts from 0, then 1, 2, 3, etc.

- Get the second element from the following array
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/fc18bc23-350b-46bb-aa75-b23b80ce9f83)

- Get the third and fourth element from the following array
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/f30f6be0-e21f-4026-a007-95aaa241c8c7)

> The "(arr[2] + arr[3])" syntax is used to find two elements, namely the third element and the fourth element.

**8. Accessing elements from a specified array.**
- Access the element on the first row, second column
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/bdf86f3d-f283-49bb-a68e-2cecf772ca6b)

The "arr[0, 1]" syntax is used to retrieve the element at 1st row and 2nd column.

- Access the element on the 2nd row, 5th column
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/36d19e7d-cba8-427c-996e-ee3e37cb460f)

- Access the third element of the second array of the first array
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/cdab3667-37a6-4ddc-8fbd-19b7109fef21)

The "arr[0, 1]" syntax is used to access the 2nd dimension, the 1st row, and the 3rd element.

## Pandas
Pandas is a powerful and widely used open-source Python library primarily used for data manipulation and analysis. It provides high-performance data structures and tools for working with structured data, making it an essential tool for data scientists and analysts.

> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/2230e57f-fe8d-4b0d-a07a-0944b7f00972)

Pandas has two main objects: Series and DataFrame.


## Series
The Series object is a ONE-dimensional array that can store various types of data, such as integers, floats, strings, and others. It does not have column names as it consists of only one column. Each element in a Series has a label called an index.
![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/df730949-46ee-45fe-9efa-85e582e69210)

Convert it into a Series

![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/22875b35-999b-4e4a-930b-78e69feeaf55)

Convert the Series to an array

![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/360ca8ac-70a6-4d00-9532-083265b80005)

Display the indices.

The indices are represented as a range, where the start point is inclusive, and the stop point is exclusive in the range.

- Implicit indexing: Default numerical index assigned based on positional order.
- Explicit indexing: Custom labels or values are assigned to uniquely identify rows or columns.

>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/56c04613-b76d-48a5-aa6c-84b9e7c17b8b)

When the implicit and explicit indices are the same, when we call the data, it will rely only on its explicit indices.

>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/9bbdbb68-54c4-4112-9e73-2420ac9e677b)

The result of name_2[0] is an error due to the similarity between the explicit indices and the implicit indices.

We'll now try to perform data-slicing
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/0a4f5dd5-6fb3-4df1-bac8-5cf0ac26d5e5)

But if we slice its implicit indices, only the start point will appear, because implicit indices are in the form of a range
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/78d5bf7b-800f-4ef0-9034-dcaf0314728f)

## Ioc and iloc
Example of data where some implicit and explicit indices are the same.

>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/df733de3-e31d-4c72-9ca7-fe62b11aad9e)

When we access a single index, it will display its explicit index.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/096fbb1a-c1e3-4c11-b01f-03fcf669e7ad)

When explicit and implicit indices are the same, inconsistencies occur as in the case above.
To address this inconsistency, we will use the principles of loc and iloc.
loc is used to call its explicit indices, while iloc is used to call its implicit indices.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/c0f0be6c-0235-426e-87e5-2e9199f88ab1)

*Dictionary -- Series*

### DataFrame
DataFrame is a two-dimensional tabular data structure with labeled axes (rows and columns). This allows for easy manipulation and analysis of data. Essentially, a DataFrame is a collection of series, with at least one series.

DataFrame With 2 Series : 
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/25eb39f7-8e73-4642-9303-87b69d85a1b4)
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/83c001f7-d84e-4421-9eef-2869e738b5e9)

### Load Data CSV
Load Data ‘Kelahiran_Bayi_Jakarta_2020’.csv that has been aplouded in the same folder in Python.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/90314c50-2bf4-4dfa-9826-99fbb2bc3a9a)

### Head()
Head() function to a viewing top in data by default is top five can be customized as required.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/e99a4f72-9f08-4d5b-bb6e-3afdcb35eb8f)

### Tail()
Tail()returns the last 5 rows if a number is not specified,returns a specified number of last rows.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/918144c1-6ae3-4767-877b-12e5267e20ce)

### Info()
Info()Info method prints information about the DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/bd65119e-a9ad-45e0-8d26-a28de2fe5965)

### Index
Index returns the index information of the DataFrame.

### IsNull()
isnull used to finds NULL values in DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/7be60f2d-1148-4c2b-b98c-c41ce020b1e0)

### NotNull()
notnull used to finds values that are NOT NULL.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/26967389-2ea0-4092-b461-14cc6fc07a65)

### Shape
Shape is the number of rows and columns on the index of the DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/2d139a93-4f15-4219-8c9e-dc39006e6be7)

### Columns
Column returns the label of each column in the DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/f86fcfd7-479f-4272-9be5-2840059b3e30)

### Describe
Returns a description summary for each column in the DataFrame,describe contains numeric data from managed datasets.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/01c2ac77-8532-4a50-9040-c14fdc19e7f6)

### Mean
Mean (The average value) = Return the mean of the values in the specified axis.

### Median
Returns a description summary for each column in the DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/a983e535-f042-4292-bc7b-7cffcb4fc1e6)

Median (The mid point value) = Return the median of the values in the specified axis.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/218dbb50-0e4d-4223-98b3-75de42c83c77)

### Mode
Returns a description summary for each column in the DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/0a0d1a75-992d-4fa8-966f-8da0e953c472)


- The df.unique() syntax is used to get unique values in the columns of a pandas DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/099363b9-7e4e-404a-b0e3-dd05980b2326)

- The df.nunique() is a function in Python that is used to get the unique number of values in a column or axis in a DataFrame.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/c85378f0-5d4e-4441-8bd2-3ddd537a3270)

- The df.type_value_counts() is a method on a DataFrame in pandas that is used to count the number of occurrences of each unique value in a column, while ordering them based on the number of occurrences.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/545f7ebd-9633-4233-a081-6f0b5cf8032a)

- Call a specific column is a notation for retrieving certain columns from a DataFrame df. This notation will return a new DataFrame containing only the specified columns.
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/81a094bf-9376-4013-a2d5-ecb557784119)

- Calling a Python dataset with terms and conditions means retrieving or selecting certain data from a dataset based on certain terms or conditions. This can be done using boolean operators or logical statements, such as ==, !=, <, >, <=, >=, or and, or, not.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/9696aaa5-40d2-4f22-901c-6bc998fc3aff)

- Calls several columns accompanied by a filter terms and conditions
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/997dd5f2-2188-4ca4-8ec8-f28bd9d45c42)

### DateTime 
DateTime is a module in Python that deals with real-time data and time. It provides classes and functions to manipulate and format dates and times. Here are some commonly used classes and functions in the DateTime module. 
- date : This class represents a date (year, month, and day) without time.
- datetime : This class represents a date and time (year, month, day, hour, minute, second, and microsecond).
- time : This class represents time (hour, minute, second, and microsecond) without a date.
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/97f7b0ca-a811-4c85-9b6d-712020ee66ed)

### Random Library 
The random module in Python provides various functions to generate random numbers. Here are some commonly used functions in the random library:
- random.random(): This function returns a random float number between 0.0 to 1.0.
> ![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/73dd321d-0ec0-4061-b07b-fa629c2b4b7f)


Txt File - Open - Read - Close
- Open : In Python, you can open and read a text file using the built-in open() function. The open() function in Python is used to open a file and return a file (.txt) object.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/8a3d26a8-03dc-4061-b6d6-088ce25609de) 


- Read : The read() function in Python is used to read the contents of a file object that has been opened using the open() function. 
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/928a8d22-d2d6-43f6-9c05-f5f326c74791)

- Close : The close() function in Python is used to close a file that has been opened using the open() function. This is important because it frees up system resources and ensures that any changes made to the file are saved.
>![Image](https://github.com/users/alresadeva/projects/2/assets/166176480/cfbfbd13-3f14-428d-a992-a64bcf09a086)
