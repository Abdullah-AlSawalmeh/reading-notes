# What Are Dunder Methods?

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores,

- example **init** or **str**.

- Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box.

- Iteration: **len**, **getitem**, **reversed**
  In order to iterate over our account object I need to add some transactions. So first, I’ll define a simple method to add transactions. I’ll keep it simple because this is just setup code to explain dunder methods, and not a production-ready accounting system:

```
def add_transaction(self, amount):
    if not isinstance(amount, int):
        raise ValueError('please use int for amount')
    self._transactions.append(amount)
```

## Callable Python Objects: **call**

- You can make an object callable like a regular function by adding the **call** dunder method. For our account class we could print a nice report of all the transactions that make up its balance:

```
class Account:
    def __call__(self):
        print('Start amount: {}'.format(self.amount))
        print('Transactions: ')
        for transaction in self:
            print(transaction)
        print('\nBalance: {}'.format(self.balance))
```

<img src="https://lh3.googleusercontent.com/proxy/kg3UPP8h_apK6bYh6S51lkCIrvzTANdJAiIwpSzVUbYuFMqBVW6bvl_eirMvF8FFTDTO9HE-TVME3wwGgfNDXKllPSmp3vmOBNhTTfFKvvAAZ4o7EKs8" width="700px" height="400px">

## Enriching a Simple Account Class

Throughout this article I will enrich a simple Python class with various dunder methods to unlock the following language features:

Initialization of new objects
Object representation
Enable iteration
Operator overloading (comparison)
Operator overloading (addition)
Method invocation
Context manager support (with statement)

## What is probability?

- At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?” An event is some outcome of interest. To calculate the chance of an event happening, we also need to consider all the other events that can occur. The quintessential representation of probability is the humble coin toss. In a coin toss the only events that can happen are:

1. Flipping a heads
2. Flipping a tails

## Three Sigma Rule

- The Three Sigma rule, also known as the empirical rule or 68-95-99.7 rule, is an expression of how many of our observations fall within a certain distance of the mean. Remember that the standard deviation (a.k.a. “sigma”) is the average distance an observation in the data set is from the mean

<img src="https://slideplayer.com/slide/5990783/20/images/8/Three+Sigma+Rule+68%25+of+the+data+95%25+of+the+data+99.7%25+of+the+data.jpg" width="600px" height="300px">

## Z-score

- The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?
- The equation below is the Z-score equation.

<img src="https://i.imgur.com/3TuDF4G.jpg" width="600px" height="300px">

---
