### Lists and Indexing

#### Introduction to Lists
As we learning in Part 1: Variable Types, there are many different types of objects in Python outside of just integers, floats, and strings. One such object is a list! This can contain zero or more objects within it. 

To denote a list, we place square brackets around zero or more objects and separate the objects with commas. For example:

`a = [1, 'python', 3]` </br>
`b = []` </br>
`c = [[1,'cat'], 3]` </br>

... and many more combinations!

#### Introduction to Indexing
Every object within a list comes with a position. Python is zero-indexed, meaning it starts at 0 not 1. To access an object within a list, we append brackets to the variable name and call that position. 

To see this in practice, let's go ahead and consider the following list:

`a = [300, 600, 1200]` </br>

Let's say we want to access the first element of the list `a`. To do this, we can simply append brackets with the desired position (zero) like so:

`print(a[0])` </br>
`Output: 300` </br>

This practice of indexing can extend further than single elements. If we want to grab all values between two index positions, we can pass a colon into the brackets between the desired positions. For example:

`k = [240, 314, 111, 86, 350]` </br>
`print(k[1:5])` </br>
`Output: [314, 111, 86]` </br>

Now, as you likely noticed, there's a slight nuance here: Python will include the first position you included, and omit the last, in the previous example, let's say we wanted to grab everything after and including the first position. To do that, we simply would omit the second index position and retain the colon. This tells Python to grab everything remaining in the list! 

`j = ['cat', 'python', 'star']` </br>
`print(j[1:])` </br>
`Output: ['python', 'star']` </br>

Last but not least, we can also work in reverse when indexing in lists! To do this, we leverage negative numbers, with -1 representing the final object in the list.

### Summary
In this lesson, we introduced a new object lists! These are buckets of zero or more objects. Each object in a list natively has an index position, and can be accessed by appending brackets and colons!
