### Numpy

#### Package Importing
Like other languages, Python allows users to import packages that offer more than standard functions. These can be as simple as plotting packages and as complex as machine learning. Before we import our first package, numpy, let's quickly review just how to bring in a package. 

All imports start with an import statement (crazy!) followed by the package name. The Anaconda distribution comes preinstalled with many useful packages including numpy. To bring it in, we can simply execute the line of code:

`import numpy` </br>

What's more is we can actually give our packages shorthanded aliases. Most Python users will execute the following:

`import numpy as np` </br>

This just requires less typing later on. That's about it! Now you are ready to dive into numpy :) 

#### Introduction to Numpy
Numpy is a powerful, incredibly fast, arithmetic package. Most of your standard arithmetic operations can be found in numpy, as well as vector and matrix constructions. Numpy iterates through lists, offering Python users quick and efficient means to studying their data. 

To access these we'll need to deploy the use of methods. Think of the package as a house, and the methods are things you can do within the house. We can call them simply by appending a `.method_name(args)` to the package name. 

To show this in practice, let's do three steps. Importing numpy, creating a list, and calculating the sum of that list. 

`# Bringing in Numpy` </br>
`import numpy as np` </br>

`# Making a list` </br>
`a = [5673, 689, 2314]` </br>

`# Calculating the sum with method` </br>
`print(np.sum(a))` </br>
`Output: 8685` </br>

There are bunches of different methods within the numpy package, which is part of the reason it is so popular. There are methods to generate random values in a list, uniform distributions, and even fitting a basic model. To see a full list of numpy methods, see here:

https://numpy.org/doc/stable/reference/arrays.ndarray.html#
