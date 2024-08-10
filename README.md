# Simple Calculator Function

## Overview

This project contains a simple calculator function implemented in Python. The `calculator` function can perform basic arithmetic operations such as addition, subtraction, and multiplication. It uses two smaller functions (`add_two_numbers`, `subtract_two_numbers`, and `multiply_two_numbers`) to perform these operations.

## Functionality

The `calculator` function accepts three parameters:
1. `a` (int): The first integer value.
2. `b` (int): The second integer value.
3. `operation` (str): The operation to be performed. It should be one of `"add"`, `"subtract"`, or `"multiply"`.

Based on the value of the `operation` parameter, the `calculator` function performs the following:
- **Addition**: Calls `add_two_numbers(a, b)` if `operation` is `"add"`.
- **Subtraction**: Calls `subtract_two_numbers(a, b)` if `operation` is `"subtract"`.
- **Multiplication**: Calls `multiply_two_numbers(a, b)` if `operation` is `"multiply"`.
- **Error Handling**: Prints an error message if the inputs are invalid or the operation is not recognized.

## Requirements

Ensure you have Python installed. 

