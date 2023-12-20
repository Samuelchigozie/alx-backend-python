# Variable (Type) Annotations

This repository consists of tasks aimed at learning and applying variable and type annotations in Python 3.

## Tasks Overview

### 0. Basic annotations - add

[**0-add.py**](0-add.py) contains a type-annotated function `add` that takes two float arguments `a` and `b` and returns their sum as a float.

### 1. Basic annotations - concat

[**1-concat.py**](1-concat.py) contains a type-annotated function `concat` that takes two string arguments `str1` and `str2` and returns their concatenated string.

### 2. Basic annotations - floor

[**2-floor.py**](2-floor.py) contains a type-annotated function `floor` that takes a float argument `n` and returns its floor as an int.

### 3. Basic annotations - to string

[**3-to_str.py**](3-to_str.py) contains a type-annotated function `to_str` that takes a float argument `n` and returns its string representation.

### 4. Define variables

[**4-define_variables.py**](4-define_variables.py) is a script that defines and annotates several variables with specified values, including integer, float, boolean, and string types.

### 5. Complex types - list of floats

[**5-sum_list.py**](5-sum_list.py) contains a type-annotated function `sum_list` that takes a list of floats (`input_list`) as an argument and returns their sum as a float.

### 6. Complex types - mixed list

[**6-sum_mixed_list.py**](6-sum_mixed_list.py) contains a type-annotated function `sum_mixed_list` that takes a list (`mxd_lst`) of integers and floats and returns their sum as a float.

### 7. Complex types - string and int/float to tuple

[**7-to_kv.py**](7-to_kv.py) contains a type-annotated function `to_kv` that takes a string `k` and an int or float `v` as arguments and returns a tuple. The first element of the tuple is the string `k`, and the second element is the square of the int/float `v` (annotated as float).

### 8. Complex types - functions

[**8-make_multiplier.py**](8-make_multiplier.py) contains a type-annotated function `make_multiplier` that takes a float `multiplier` as an argument and returns a function that multiplies a float by `multiplier`.

### 9. Let's duck type an iterable object

[**9-element_length.py**](9-element_length.py) contains a type-annotated version of a function `element_length` that takes a list (`lst`) and returns a list of tuples containing elements and their lengths.

### 10. Duck typing - first element of a sequence

[**100-safe_first_element.py**](100-safe_first_element.py) contains a type-annotated version of a function `safe_first_element` that returns the first element of a sequence (`lst`) if it exists.

### 11. More involved type annotations

[**101-safely_get_value.py**](101-safely_get_value.py) contains a script with a function `safely_get_value` and includes type annotations for the parameters and return values.

### 12. Type Checking

[**102-type_checking.py**](102-type_checking.py) contains a script using `mypy` to validate and apply necessary changes for the given code that includes a function `zoom_array`.

## Concept

[Advanced Concept](https://intranet.alxswe.com/concepts/554)

## Resources

- [Python 3 Typing Documentation](https://intranet.alxswe.com/rltoken/5j0OtdWh36_HVAHKJX2gaA)
- [MyPy Cheat code](https://intranet.alxswe.com/rltoken/Eud-nrUG7x3iT6JD2Sas-g)