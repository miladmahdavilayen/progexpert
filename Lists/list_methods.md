# Lists in Python

## General Notes on List

- Data within a list are ordered. Each data is assigned an index.
- Does not matter what data type you add to a list. Can contain several data type within the same list.
- An index is the position of an element within a list
- We always start counting at zero
## Some of the usefull methods for lists:

```python
1. my_list.append() # adds a new element to the end of your list
2. len(my_list) # this is a dunder method that will return the lenght of your list
3. my_list.pop() # it will remove the last element in your list and returns it
4. my_list.count(element) # it will count how many times an element occures inside your list. True in a list will also be considered as one.
5. my_list.index(element) # it will return index of the first time that an element occurs in your list.
6. my_list.remove(element) # it removes the first occurance of an element you pass to the method.
7. contains = element in my_list # will check if an element exists inside your list. 
```

## Negative indexing in lists:
```python
x = [1, 2, 3, 'milad', 6, True]

x[-1] # this will return the last element in the list which is True
x[-2] # this will return 6 which is the second last element in the list
```


## Combining two lists together

- Using the addition operator:
```python
x = [1, 2, 3]
y = [4, 5]
combined = x + y # the combined list will contain all elements from both lists.
```

- Using the extend() method:

```python
x.extend(y)  # will add the items from y to the end of x
```

## Nested lists:
- you can access the elements in an interior list within a list:
  ```python
  lst = [[3, 5], [6, [7, 5]], ['milad', 'javad']]
  lst[-2][1][0] # this will retunr 7
  ```



