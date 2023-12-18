### Pandas

#### Introduction to Pandas
As you might have guessed, we can't always manually type up lists and arrays for numpy to perform operations on. Eventually, we'll need to bring in and manipulate our data. To do this, many Python users choose to leverage pandas. 

Pandas stores data in intuitive tables, and has several features that make accessing and manipulating data a breeze. These tables are often referred to as "dataframes". The index, or the 0th axis, goes down the table and refers to the rows. Columns, on the other hand, are the 1st axis. 

#### Importing data
One very pandas method is `.read_excel()`. This method takes a user defined filepath, and sheet number, and pulls in the excel sheet. To see this in practice:

`import pandas as pd` </br>
`dataframe = pd.read_excel(r"filepath.xlsx", 1)` </br>

The above code:
1. Imported the pandas package
2. Created a variable dataframe
3. Assigned the 2nd sheet (remember, Python is zero indexed) of the excel workbook "filepath.xlsx) to the variable dataframe

However, to learn how to use pandas, let's just go ahead and artificially make a dataset. If you copy and paste the below code in your notebook, you should see a dataframe populate. 

`import pandas as pd` </br>
`import numpy as np` </br>
`df = pd.DataFrame(data = np.random.rand(10,2), columns = ['x', 'y'])` </br>

And that's it! Now when you call df, you should see a dataframe output into your notebook. 

#### Indexing a dataframe
We can apply many of the principles we previously learned in indexing to a dataframe. As a reminder, a dateframe's index refers to the row identifiers. If we wanted to grab the first row of data, we'd append the `.iloc[0]` method onto our dataframe. 

Similarly to our indexing lesson, we can work backwards, grab several different rows using the `.iloc[]` method on our dataframe. 

However, one important note is that dataframe indexes don't just have to be numeric. These can also be strings, dates, or anything similar. 

If we'd like to access a categorical index, we use the `.loc[]` method instead. For instance, let's say our dataframe has a date based index and we wanted to access the data for September 1st, 2020. To do that, we'd execute:

`sept_1 = df.loc['2020-09-01']` </br>

Now, there are a million and one different ways to index a dataframe, but the above general rule of `.iloc[]` for `.loc[]` will be a good starting point. 

#### Dataframe Columns
Accessing columns in pandas is very straight forward. To call one, we simple append brackets containing the name to the dataframe name. For example, if we wanted just the x column in the above example, we'd execute `df['x']`. It's that easy! Note for more than one column, we'd simply make the argument inside the brackets a list of all the columns we want. 

What's great about pandas is how easily we can make a new column. Let's say we wanted to create a new column, `z`, that's equivalent to `x+y`. This is easy as creating a new variable with the name we want, and telling python how to make it. Visually:

`df['z'] = df['x'] + df['y']` </br>

#### Other possibilities
Pandas can truly satisfy many basic analysis needs, such as cleaning NaN rows, visualizing columns, and many more. Further documentation can be found here: 

https://pandas.pydata.org/docs/
