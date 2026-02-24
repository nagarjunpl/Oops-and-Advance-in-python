# Python `split()` Method

## What is `split()` in Python?

The `split()` method is a built-in string method in Python.\
It is used to divide a string into a list of smaller strings based on a
separator.

------------------------------------------------------------------------

## Syntax

``` python
string.split(separator, maxsplit)
```

### Parameters:

-   **separator (optional)** -- The character or substring used to split
    the string.\
    Default is whitespace (space, tab, newline).
-   **maxsplit (optional)** -- Maximum number of splits to perform.

------------------------------------------------------------------------

## 1️⃣ Split by Space (Default)

``` python
text = "Hello World Python"
result = text.split()
print(result)
```

### Output:

    ['Hello', 'World', 'Python']

------------------------------------------------------------------------

## 2️⃣ Split Using a Custom Separator

``` python
text = "apple,banana,orange"
result = text.split(",")
print(result)
```

### Output:

    ['apple', 'banana', 'orange']

------------------------------------------------------------------------

## 3️⃣ Using maxsplit

``` python
text = "one two three four"
result = text.split(" ", 2)
print(result)
```

### Output:

    ['one', 'two', 'three four']

Explanation: Only 2 splits happen.

------------------------------------------------------------------------

## 4️⃣ Split by Hyphen

``` python
text = "2026-02-24"
result = text.split("-")
print(result)
```

### Output:

    ['2026', '02', '24']

------------------------------------------------------------------------

## Important Points

-   `split()` always returns a **list**.
-   If the separator is not found, it returns a list with the original
    string.
-   Default separator is whitespace.
-   Very useful for user input and data processing.

------------------------------------------------------------------------

## Simple Example (User Input)

``` python
name = input("Enter your full name: ")
words = name.split()
print("First name:", words[0])
```

------------------------------------------------------------------------

## Summary

`split()` is used to break a string into parts and store them in a list.
It is commonly used in: - Data processing - Reading input - Parsing CSV
values - Handling text data
