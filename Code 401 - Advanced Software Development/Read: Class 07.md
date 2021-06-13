# Python Scope & the LEGB Rule:

## Understanding Scope

- The scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope. Several programming languages take advantage of scope for avoiding name collisions and unpredictable behaviors.
- There is two general scopes:

Global scope: The names that you define in this scope are available to all your code.

Local scope: The names that you define in this scope are only available or visible to the code within the scope.

![](https://cdn.educba.com/academy/wp-content/uploads/2019/11/scope-in-python.png)

## Python Scope vs Namespace

- In Python, the concept of scope is closely related to the concept of the namespace. As you’ve learned so far, a Python scope determines where in your program a name is visible.

## builtins: The Built-In Scope

- The built-in scope is a special Python scope that’s implemented as a standard library module named builtins in Python 3.x. All of Python’s built-in objects live in this module. They’re automatically loaded to the built-in scope when you run the Python interpreter. Python searches builtins last in its LEGB lookup, so you get all the names it defines for free. This means that you can use them without importing any module.

## Modifying the Behavior of a Python Scope

- functions, classes, and other Python objects to certain portions of your code. You now know that you can access or reference global names from any place in your code, but they can be modified or updated from within the global Python scope.

## Using Scope Related Built-In Functions

- There are many built-in functions that are closely related to the concept of Python scope and namespaces. In previous sections, you’ve used dir() to get information on the names that exist in a given scope. Besides dir(), there are some other built-in functions that can help you out when you’re trying to get information about a Python scope or namespace. In this section, you’ll cover how to work with:

1. globals()
2. locals()
3. dir()
4. vars()

## Conclusion

- The scope of a variable or name defines its visibility throughout your code. In Python, scope is implemented as either a Local, Enclosing, Global, or Built-in scope. When you use a variable or name, Python searches these scopes sequentially to resolve it. If the name isn’t found, then you’ll get an error. This is the general mechanism that Python uses for name resolution and is known as the LEGB rule.

- You’re now able to:

1. Take advantage of Python scope to avoid or minimize bugs related to name collision
2. Make good use of global and local names across your programs to improve code maintainability
3. Use a coherent strategy to access, modify, or update names across all your Python code

---
