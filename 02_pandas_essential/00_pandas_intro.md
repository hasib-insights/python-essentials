## What is Pandas?

Pandas is a Python library used for working with data sets.

It has functions for analyzing, cleaning, exploring, and manipulating data.

The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.
## Why Use Pandas?

Pandas allows us to analyze big data and make conclusions based on statistical theories.

Pandas can clean messy data sets, and make them readable and relevant.

Relevant data is very important in data science.

## Pandas gives you answers about the data. Like:
Is there a correlation between two or more columns?
* What is average value?
* Max value?
* Min value?

## Import Pandas

```python
import pandas
```
**Pandas is usually imported under the `pd` alias.**
> alias: In Python alias are an alternate name for referring to the same thing.
```python
#Create an alias with the as keyword while importing:

import pandas as pd
```
## Checking Pandas Version
The version string is stored under `__version__` attribute.
```python
import pandas as pd

print(pd.__version__)
```
