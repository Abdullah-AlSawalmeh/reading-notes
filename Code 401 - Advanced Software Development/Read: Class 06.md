# About Random Module

### how to use:

- In this post, I would like to describe the usage of the random module in Python. The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.

- When to use it? We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.

## Random functions

- The Random module contains some very useful functions.

Randint
If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number. Generate integers between 1,5. The first value should be less than the second.

#### import random

- print random.randint(0, 5)
  Random
  If you want a larger number, you can multiply it.

- example, a random number between 0 and 100:

```
import random
random.random() * 100
```

## choice

- Generate a random value from the sequence sequence.random.

```
choice( ['red', 'black', 'green'] ).
```

The choice function can often be used for choosing a random element from a list.

```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
Randrange
Generate a randomly selected element from range(start, stop, step)
```

## About Risk Analysis

- The probability of any unwanted incident is defined as Risk. In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.

- In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks.

- Now, you might think what could be the possible risks that you could encounter? Well here is a list:

1. Use of new hardware

2. Use of new technology

3. Use of new automation tool

4. The sequence of code

5. Availability of test resources for the application

## How to perform Risk Analysis?

1. Searching the risk.
2. Analyzing the impact of each individual risk.
3. Measures for the risk identified.

---
