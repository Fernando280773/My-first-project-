# My-first-project-

python-calculator/
│
├── src/
│   ├── __init__.py
│   ├── calculator.py        # Main calculator logic
│   └── operations.py        # Basic math operations
│
├── tests/
│   ├── __init__.py
│   └── test_calculator.py   # Unit tests
│
├── README.md               # Project documentation
├── requirements.txt        # Project dependencies
├── .gitignore             # Git ignore file
└── setup.py               # Package configuration

# Content for calculator.py:
class Calculator:
    def __init__(self):
        self.result = 0

    def add(self, a, b):
        return a + b
    
    def subtract(self, a, b):
        return a - b
    
    def multiply(self, a, b):
        return a * b
    
    def divide(self, a, b):
        if b == 0:
            raise ValueError("Cannot divide by zero")
        return a / b

# Content for README.md:
# Python Calculator

A simple calculator application written in Python.

## Features
- Basic arithmetic operations
- Error handling
- Unit tests

## Installation
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the calculator: `python src/calculator.py`

## Usage
```python
from calculator import Calculator

calc = Calculator()
result = calc.add(5, 3)  # Returns 8
```

## Testing
Run tests with: `python -m pytest tests/`
