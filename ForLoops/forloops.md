# For Loops in python

## range() function in for loops:
- the range() function will create an iterator object
- what arguments can be passed to the range funnction:
  ```python
  x = range(10) # this will build an iterator that iterates from 0 to 9 moving one step at a time
  y = range(5, 20) # this will build an iterator that iterates from 5 to 19 moving one step at a time
  m = range(3, 15, 3) # this iterator will move 3 steps at a time from 3 to 14

  # you can print the items in an iterator using a for loop
  for item in m:
    print(m)
- what's the best use case of an iterator that was built by range() function:
  - since iterators take the least amount of memeory (Big O notation of 1) they are best to be used instead of lists or tuples in any for loops.
- you cannot pass only a negative number to the range() function. it will do nothing.
- you can have negative steps and also iterate in a negative direction:
  ```python
  for i in range(20, 5, -5):
    print(i)
    # this will print: 20, 15, 10 and not 5 itself.
  ```



## Iterating through lists:
- using the len() function within the range() function to go through the indexes.
- using the in keyword to go through the list items directly.
  ```python
  for i in range(len(my_list)):
    print(my_list[i])
  ```
- Lists are also iterable objects which means you can loop directly in the list. You can just do:
  ```python
  for element in my_list:
    print(i)
  ```

- One other great way to loop through the index and the element of a list is using the enumerate() keyword:
   ```python
      for i, element in enumerate(lst):
          print(i, element)
  ```

  
## Iterating through tuples and strings
- works pretty much same way as lists
- all 3 steps in lists will also work for tuples and strings


## keywords inside a for loop
- break: if you wanna stop the loop as soon as sth happens:
  ```python
  lst = [3, 5, 7, 8, 4, 9, 7, 3]
  for num in lst:
    if num == 4:
      break
    print(num)
  print("done")
  ```

- continue: it will skip that iteration and every function after it.
  ```python 
  lst = [3, 5, 7, 8, 4, 9, 7, 3]
  for num in lst:
    if num == 4:
      continue
    print(num)
  print("done")   # this will print everything but 4 bc it skips that iteration
  ```

## Nested for loops 
- a for loop within another for loop:
  ```python
  for i in range(10):
    for j in range(5):
      print(i, j)
  ```

- Applications of nested for loop with a nested list:
  ```python
  lst = [[2, 3], [4. 5], [6. 7], [8, 9]]

  for i in range(len(lst)):
    interior_lst = lst[i]
    for j in range(len(interior_lst)):
      print(interior_lst[j])
  ```

## Some for loop examples:
