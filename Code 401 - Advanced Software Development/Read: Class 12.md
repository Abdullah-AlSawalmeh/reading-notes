# About Pandas

- pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming

- Pandas library is one of the most preferred tools for data scientists to do data manipulation and analysis, next to matplotlib for data visualization and NumPy, the fundamental library for scientific computing in Python on which Pandas was built.

- The fast, flexible, and expressive Pandas data structures are designed to make real-world data analysis significantly easier, but this might not be immediately the case for those who are just getting started with it. Exactly because there is so much functionality built into this package that the options are overwhelming.

![](https://lrdatascience.com/wp-content/uploads/2019/05/2178236_88ed.jpg)

### Object creation

See the Data Structure Intro section.

Creating a Series by passing a list of values, letting pandas create a default integer index:

```
In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])

In [4]: s
Out[4]:
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64
```

- Pandas provides highly optimized performance with back-end source code is purely written in C or Python.

### Installation

To install pandas from source you need Cython in addition to the normal dependencies above. Cython can be installed from pypi:

- pip install cython
  In the pandas directory (same one where you found this file after cloning the git repo), execute:

- python setup.py install
  or for installing in development mode:

python -m pip install -e . --no-build-isolation --no-use-pep517

### Time series

pandas has simple, powerful, and efficient functionality for performing resampling operations during frequency conversion (e.g., converting secondly data into 5-minutely data). This is extremely common in, but not limited to, financial applications. See the Time Series section.

```
In [104]: rng = pd.date_range('1/1/2012', periods=100, freq='S')

In [105]: ts = pd.Series(np.random.randint(0, 500, len(rng)), index=rng)

In [106]: ts.resample('5Min').sum()
Out[106]:
2012-01-01    24182
Freq: 5T, dtype: int64
```

- Statistics Use these commands to perform various statistical tests. (These can all be applied to a series as well.)

df.describe() | Summary statistics for numerical columns

df.mean() | Returns the mean of all columns

df.corr() | Returns the correlation between columns in a DataFrame

df.count() | Returns the number of non-null values in each DataFrame column

df.max() | Returns the highest value in each column

df.min() | Returns the lowest value in each column

### Plotting

- We use the standard convention for referencing the matplotlib API:

```
In [131]: import matplotlib.pyplot as plt

In [132]: plt.close('all')
In [133]: ts = pd.Series(np.random.randn(1000),
   .....:                index=pd.date_range('1/1/2000', periods=1000))
   .....:

In [134]: ts = ts.cumsum()

In [135]: ts.plot()
Out[135]: <AxesSubplot:>
```
