# Tuples in python

## what is a tuple:
- a tuple is really any element inside of a paranthesis
- tuples have index like lists (exactly the same of indexing in lists)
- tuples are immutable you cannot directly modify a tuple element
- only way to change a tuple elements is to build a new one

## How to create a tuple:
- either use () and put elements inside, 
- or use the tuple() function over a list or set of items.
- or use none of the above and just separate elements by commas and assign them to a variable
  

## Similar tuple methods to list:
- len(my_tuple): will return the length of tuple (how many items)
- count(element): how many time element occured
- index(element): will print the index of the first occurance of an element within the tuple
- in operator: check if sth contains in the tuple the same way as in lists
- we can have tuples inside of tuples just as in lists
- nested tuples elements, you can access elements within elements the same way as in lists

## Some new methods for tuples:
- in python if I have only a bunch of numbers or elements separated by commas and assign them to a variable, it will automaticall will make that variable a tuple:
  ```python
  x = 1, 2, 3, 'milad', False, 6.5
  print(type(x)) # class tuple
  print(x)  # (1, 2, 3, 'milad', False, 6.5)
  ``` 

## Create tuples with only one element
- in order to do that you have to add a comma right after the only element within the paranthesis
  ```python
  x = (1)
  print(x)  # this will print just an integer which is 1
  y = (1,)
  print(y) # this one will print y as a tuple with only one element in it 
  ```