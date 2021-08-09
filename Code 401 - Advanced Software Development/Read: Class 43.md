What Are Dunder Methods?
In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example **init** or **str**.

As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”

These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them. You should treat these methods like a normal language feature.

Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

Understanding iterators is a milestone for any serious Pythonista. With this step-by-step tutorial you’ll understanding class-based iterators in Python, completely from scratch.

Python Iterators Tutorial
I love how beautiful and clear Python’s syntax is compared to many other programming languages.

Let’s take the humble for-in loop, for example. It speaks for Python’s beauty that you can read a Pythonic loop like this as if it was an English sentence:

numbers = [1, 2, 3]
for n in numbers:
print(n)
But how do Python’s elegant loop constructs work behind the scenes? How does the loop fetch individual elements from the object it is looping over? And how can you support the same programming style in your own Python objects?

You’ll find the answer to these questions in Python’s iterator protocol:

Objects that support the **iter** and **next** dunder methods automatically work with for-in loops.

But let’s take things step by step. Just like decorators, iterators and their related techniques can appear quite arcane and complicated on first glance. So we’ll ease into it.
