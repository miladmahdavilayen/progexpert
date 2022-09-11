# Strings in python

## recap on strings
- we can index strings:
  - ```python
    s = "hello"
    s[0] # will return the first char which is h
    ```

- the len method works on strings the same as lists as well:
  - ```python 
    len(s) # this will return the length of the string
    ```

## string methods:
- count(): it will count the number of times a char has occured in your string
- find("char"): it will return the index of the character that is passed to it in your string.
  ```python
  s = "hello"
  index = s.find('l')
  print(index)  # this will print 2 which the index of first occurance of l
  ```
- .uppper and .lower:
  ```python
  upper = s.upper()
  lower = s.lower()
  print(upper, lower) # this will print "HELLO, hello"
  ```

- capitalize():
  ```python
  name = "milad"
  capitlaized = name.capitalize()
  print(capitalized) # will capitalize the first letter only and prints Milad
  ```

- Check if sth is in a list with in operator the same way as in lists:
  ```python
  s = "mahdavilayen"
  check = h in s
  print(check) # this will print True
  ```

- isdigit() method:
  ```python
  s = 'milad54js'
  ss = '5465'
  sss = '54.67'
  s.isdigit()
  ss.isdigit()
  sss.isdigit()
  # first is False and second is True and last if False
  # only works on integer numbers
  ```

- split('separator') method:
  ```python
  s = "hello my name is milad"
  words = s.split(' ')
  print(words) # will print ['hello', 'my', 'name', 'is', 'milad']
  ```
- replace("old_char", "new_char") method:
  ```python
  s.replace('l', 'B') # this will replace all of the ls in the string given with a capital B
  ```
- f.strings:
  ```python
  name = "milad"
  print(f'hi {name}, you are a nice guy!')
  ```

## string multiplication
```python
name = 'milad'
print(name * 5) # will repeat the string number of times that you multiplied it by
```

## multiline strings
```python
string = """hello my name is milad
and this is a multiline string
you are getting confused!!
"""  # this is also a multiline comment if not assigned to a variable
``` 

## Escape characters:

```python
name = 'milad'
string = f'hey {name} your god\'s best creature'
# the single backslash is escaping the ' character such that it won't interfere with the format method
```

## join('joiner_char') method:
- it allows you to build a string from a collection of a strings within a list.
```python
lst = ['m', 'i', 'l', 'a', 'd']
my_name = lst.join()
print(my_name) # this will print 'milad'
```

