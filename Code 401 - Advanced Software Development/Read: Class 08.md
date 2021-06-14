# List Comprehensions in Python

- List comprehensions provide a concise way to create lists, it consists of brackets containing an expression followed by a for clause, then
  zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.

- he list comprehension always returns a result list.

<img src="https://miro.medium.com/max/1132/1*dlRLsiPLNGhWVZvdKQJMWQ.png" width="800px" height="300px">

- If you used to do it like this:

```
new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))
```

## Syntax

- The list comprehension starts with a ‘[‘ and ‘]’, square brackets, to help you remember that the
  result is going to be a list.

1. new_list: The new list (result).

2. expression(i)
   Expression is based on the variable used for each element in the old list.

3. for i in old_list: The word for followed by the variable name to use, followed by the word in the old list.

4. if filter(i): Apply a filter with an If-statement.

 <img src="https://i.morioh.com/2020/04/29/630fa9e0ed38.jpg" width="800px" height="350px">
 
 - Examples
- Create a simple list

```
x = [i for i in range(10)]
print x

# This will give the output:
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

2.  Multiplying parts of a list
3.  Show the first letter of each word
4.  Lower/Upper case converter
5.  Print numbers only from a given string
6.  Parsing a file using list comprehension
7.  Using list comprehension in functions

- Exm:

```
def double(x):
  return x*2

# If you now just print that function with a value in it, it should look like this:
>>> print double(10)
20
```

## Debugging With PySnooper

- Debugging is a painful but necessary practice in software development. The tools that are available in Python range from the built-in debugger, to tools integrated with your coding environment, to the trusty print function. In this episode Ram Rachum describes his work on PySnooper and how it can be used to speed up your problem solving in complex or legacy applications.

---

Thanks For Reading
