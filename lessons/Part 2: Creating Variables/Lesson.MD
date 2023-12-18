### Creating Variables

#### Basics
Now that we've covered basic object types, we can get started making our own variables. Think of these like containers of data that we can call later on. In order to assign a variable, we simply have to name it and tie it to the object in question using an equals sign. For example:

  `a = 3` <br/>
  `b = 'cat'` <br/>
  `c = 4.1`
  
Now, if we ever want to call these variables again, we simply just have to call the variable name. 

#### Making new variables
As you can probably guess, manually typing a new variable each time can be highly inefficient. To circumvent this, let's start to make our own.

Starting with floats and integers, standard numeric operations are fair game. For example:

  `k = a + b` <br/>
  `j = c*2` <br/>
  `avg = (a+b)/2`
  
 Now, for strings, things are a little different. We can actually add them together, like so:
 
  `greeting = 'hello' + ' ' + 'world'` <br/>
  `response = 'hey' + ' ' + 'there!'` <br/>
  
  However,  we can't simply subtract out letters. Try subtracting two strings, and you'll likely see an error returned.
  
  As you may imagine, there are a million and one different ways we may create a new variable. As your python skills grow, so will the complexity of the data stored within your variables. For now, we'll stick with floats, integers, and strings. 
  
  #### Equivalency Tricks
  As we've discussed, assigning a variable most often happens with the equals sign. We can, however, do some clever tricks on either side of this equals sign to make our lives easier. 
  
  Let's say we want to assign mutliple variables within one step. Python will actually interpret the position we place the variables when it assigns them. To demnonstrate, try running the following:
  
  `a,b = 10,'cat'` </br>
  `print(a)` </br>
  `print(b)` </br>
