# PowerFullDict

`PowerFullDict` is an enhanced Python dictionary that supports deep merging and inversion of dictionaries.

## Installation

Simply copy the code into your project. Requires Python 3.6 or higher.

## Usage

### Creating an Instance

```python
from your_module import PowerFullDict

my_dict = PowerFullDict({'a': 1, 'b': 2})
```
Deep Merging

Merge two dictionaries:

```python

dict1 = PowerFullDict({'a': {'x': 1}, 'b': 2})
dict2 = PowerFullDict({'a': {'y': 2}, 'c': 3})
```
merged_dict = dict1 + dict2
# Result: {'a': {'x': 1, 'y': 2}, 'b': 2, 'c': 3}

Inverting the Dictionary

Invert keys and values:

```python

simple_dict = PowerFullDict({'a': 1, 'b': 2})
inverted_dict = simple_dict.inverted()
# Result: {1: 'a', 2: 'b'}
```
Notes

    The inverted method works only with flat dictionaries.
    Deep merging creates a new instance without modifying the original dictionaries.
