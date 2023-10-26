# midterm-programming-and-data-analysis-2023

> Midterm: Programming and Data Analysis 2023.

Define functions in `midterm.py` with given names and templates then run `test-runner.py`.

## 01. Define a function `format_date_with_padding_zero()` which formats month and day with padding zero.

```python
def format_date_with_padding_zero(yyyy: int, mm: int, dd: int) -> str:
    """
    >>> format_date_with_padding_zero(2023, 9, 9)
    '2023-09-09'
    >>> format_date_with_padding_zero(2023, 9, 10)
    '2023-09-10'
    >>> format_date_with_padding_zero(2023, 10, 9)
    '2023-10-09'
    >>> format_date_with_padding_zero(2023, 10, 10)
    '2023-10-10'
    >>> format_date_with_padding_zero(2024, 1, 1)
    '2024-01-01'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `semantic_typing()` which returns the type of input semantically.

```python
def semantic_typing(x) -> str:
    """
    >>> semantic_typing(5566)
    'The type of your input 5566 is integer.'
    >>> semantic_typing(3.1415)
    'The type of your input 3.1415 is float.'
    >>> semantic_typing(False)
    'The type of your input False is boolean.'
    >>> semantic_typing(True)
    'The type of your input True is boolean.'
    >>> semantic_typing("Python")
    'The type of your input Python is string.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a function `semantic_calculator()` which operates a few simple numeric calculations.

```python
def semantic_calculator(x: int, y: int, operator: str):
    """
    >>> semantic_calculator(55, 66, "+")
    121
    >>> semantic_calculator(55, 66, "-")
    -11
    >>> semantic_calculator(3, 5, "*")
    15
    >>> semantic_calculator(3, 5, "/")
    0.6
    >>> semantic_calculator(3, 5, "//")
    0
    >>> semantic_calculator(3, 5, "**")
    243
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a function `return_days_abbreviation()` which returns weekday/weekend abbreviations given its full name.

```python
def return_days_abbreviation(x: str) -> str:
    """
    >>> return_days_abbreviation("Sunday")
    'Sun'
    >>> return_days_abbreviation("Monday")
    'Mon'
    >>> return_days_abbreviation("Tuesday")
    'Tue'
    >>> return_days_abbreviation("Wednesday")
    'Wed'
    >>> return_days_abbreviation("Thursday")
    'Thu'
    >>> return_days_abbreviation("Friday")
    'Fri'
    >>> return_days_abbreviation("Saturday")
    'Sat'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `return_days_fullname_abbreviation_from_int()` which returns the fullname and abbreviation of weekday/weekend given its order.

```python
def return_days_fullname_abbreviation_from_int(x: int) -> tuple:
    """
    >>> return_days_fullname_abbreviation_from_int(0)
    ('Sunday', 'Sun')
    >>> return_days_fullname_abbreviation_from_int(1)
    ('Monday', 'Mon')
    >>> return_days_fullname_abbreviation_from_int(2)
    ('Tuesday', 'Tue')
    >>> return_days_fullname_abbreviation_from_int(3)
    ('Wednesday', 'Wed')
    >>> return_days_fullname_abbreviation_from_int(4)
    ('Thursday', 'Thu')
    >>> return_days_fullname_abbreviation_from_int(5)
    ('Friday', 'Fri')
    >>> return_days_fullname_abbreviation_from_int(6)
    ('Saturday', 'Sat')
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a function `square_negatives()` which returns positive args given `*args`.

```python
def square_negatives(*args) -> list:
    """
    >>> square_negatives(-3, -2, -1, 0, 1, 2, 3)
    [9, 4, 1]
    >>> square_negatives(-3, -2, -1, 0, 1, 2, 3, '4', '5')
    [9, 4, 1]
    >>> square_negatives(-3, -2, -1, False, True, 2, 3, '4', '5')
    [9, 4, 1]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `remove_duplicates_and_sort()` which removes duplicate elements for `*args` then sort with ascending order.

```python
def remove_duplicates_and_sort(*args) -> list:
    """
    >>> remove_duplicates_and_sort(2, 3, 5, 7, 11, 11, 7, 5, 3, 2)
    [2, 3, 5, 7, 11]
    >>> remove_duplicates_and_sort(13, 17, 19, 23, 29, 31, 31, 29, 23, 19, 17, 13)
    [13, 17, 19, 23, 29, 31]
    >>> remove_duplicates_and_sort(10, 9, 8, 6, 4, 1, 1, 4, 6, 8, 9, 10)
    [1, 4, 6, 8, 9, 10]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `find_idxmin_idxmax()` which finds the indices of minimum and maximum values, respectively given a `list`.

```python
def find_idxmin_idxmax(x: list) -> dict:
    """
    >>> find_idxmin_idxmax([2, 3, 5, 7, 11])
    {'idxmin': [0], 'idxmax': [4]}
    >>> find_idxmin_idxmax([2, 3, 5, 7, 11, 11, 7, 5, 3, 2])
    {'idxmin': [0, 9], 'idxmax': [4, 5]}
    >>> find_idxmin_idxmax([10, 9, 8, 6, 4, 1])
    {'idxmin': [5], 'idxmax': [0]}
    >>> find_idxmin_idxmax([10, 9, 8, 6, 4, 1, 1, 4, 6, 8, 9, 10])
    {'idxmin': [5, 6], 'idxmax': [0, 11]}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `pig_latin()` which plays the Pig Latin language game with function inputs.

- For words that begin with consonant sounds, all letters before the initial vowel are placed at the end of the word sequence. Then, "ay" is added. e.g. "pig" -> "igpay". When words begin with consonant clusters (multiple consonants that form one sound), the whole sound is added to the end. e.g. "smile" -> "ilesmay"
- For words that begin with vowel sounds, the vowel is left alone, and "yay" is added to the end. e.g. "eat" -> "eatyay"

Source: <https://en.wikipedia.org/wiki/Pig_Latin>

```python
def pig_latin(x: str) -> str:
    """
    >>> pig_latin("pig")
    'igpay'
    >>> pig_latin("smile")
    'ilesmay'
    >>> pig_latin("eat")
    'eatyay'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `fibonacci()` which returns the famous Fibonacci sequence in a `list` given `a`, `b` ($a \le b$) and `length` as parameters.

Source: <https://en.wikipedia.org/wiki/Fibonacci_sequence>

```python
def fibonacci(a: int, b: int, length: int) -> list:
    """
    >>> fibonacci(0, 1, 5)
    [0, 1, 1, 2, 3]
    >>> fibonacci(0, 1, 7)
    [0, 1, 1, 2, 3, 5, 8]
    >>> fibonacci(0, 1, 11)
    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```