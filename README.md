

# Simple Calculator

A simple calculator implemented in Python. This calculator can perform basic arithmetic operations like addition, subtraction, multiplication, and division.

## Features

- Addition
- Subtraction
- Multiplication
- Division

## Requirements

- Python 3.x


## Code Overview

The calculator script (`calculator.py`) contains functions to perform each arithmetic operation:

```python
def addition(n1, n2):
    return n1 + n2

def subtraction(n1, n2):
    return n1 - n2  

def multiplication(n1, n2):
    return n1 * n2

def division(n1, n2):
    if n2 == 0:
        return "Cannot divide by zero"
    return n1 / n2 


The operations are stored in a dictionary for easy access:

```python
operators = {
    '+': addition,
    '-': subtraction,
    '*': multiplication,
    '/': division
}


The user is prompted to input the numbers and the desired operation, and the result is then calculated and displayed:

n1 = int(input('Enter the first number: '))
for operator in operators:
    print(operator)
operation = input('Enter the operator required: ')
n2 = int(input('Enter the second number: '))

if operation in operators:
    result = operators[operation](n1, n2)
    print(f'The result of {n1} {operation} {n2} is: {result}')
else:
    print('Invalid operator')


## Example

Enter the first number: 10
+
-
*
/
Enter the operator required: +
Enter the second number: 5
The result of 10 + 5 is: 15


## Contributing

Contributions are welcome! Please create a pull request with a detailed description of your changes.


## Contact

For any questions or suggestions, please open an issue or contact me at varunbabumk@gmail.com

