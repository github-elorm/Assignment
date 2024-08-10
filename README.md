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

Ensure you have Python installed. This project is compatible with Python 3.x.

## How to Use

1. **Define the smaller functions**: Make sure you have defined the following functions in your script:

    ```python
    def add_two_numbers(a, b):
        return a + b

    def subtract_two_numbers(a, b):
        return a - b

    def multiply_two_numbers(a, b):
        return a * b
    ```

2. **Use the `calculator` function**: You can use the `calculator` function as follows:

    ```python
    def calculator(a, b, operation):
        if isinstance(a, int) and isinstance(b, int):
            if operation == "add":
                return add_two_numbers(a, b)
            elif operation == "subtract":
                return subtract_two_numbers(a, b)
            elif operation == "multiply":
                return multiply_two_numbers(a, b)
            else:
                print("Please input some integer values and specify your operation as 'add', 'subtract', or 'multiply'")
        else:
            print("Both 'a' and 'b' must be integers.")
    ```

    **Example Usage:**

    ```python
    result = calculator(5, 3, "add")
    print(result)  # Output: 8
    ```

## Contributing

If you wish to contribute to this project, please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
