# TDD with Python

- Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

![](https://i.ytimg.com/vi/x5IbDPoBnb4/maxresdefault.jpg)

-The greatest advantage about TDD is to craft the software design first

-Your code will be more reliable: after a change you can run your tests and be in peace

- There are some details to pay attention. The first one is the test name. The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.

- It’s ideal to separate the tests folder from production code (the implementation) and to have something like this:

```
mymodule/
 — module.py
 — another_folder/
 — — another_module.py
tests/
 — test_module.py
 — another_folder/
 — — test_another_module.py
```

- Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.

1. Arrange: you need to organize the data needed to execute that piece of code (input);
2. Act: here you will execute the code being tested (exercise the behaviour);
3. Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

## Recursion

- The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.

- What is base condition in recursion?
  In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems.

![](https://lh3.googleusercontent.com/proxy/0Il2b18kMmH3CHD0fkoEkArZ0oHi8sSzkQvYbA317lNcLORzCcNv93H1Qc3W_WiA0KSfoYYSRDbl9Bk2Di6YoyPnK_GIq_bmyG1Ezb6kVg)

## How memory is allocated to different function calls in recursion?

- When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call.

---
