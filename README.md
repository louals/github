# Simple Calculator

A lightweight, user-friendly command-line calculator written in Python that performs basic arithmetic operations.

---

## Features

* **Basic Operations:** Addition, subtraction, multiplication, and division.
* **Error Handling:** Built-in validation for division by zero and invalid inputs.
* **Interactive Loop:** Perform multiple calculations in one session without restarting the program.

---

## Project Structure

```text
simple-calculator/
├── calculator.py
└── README.md
```

---

## Prerequisites

To run this project, you need Python installed on your system:

* **Python 3.6+**

You can check your Python version by running:

```bash
python3 --version
```

---

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/simple-calculator.git](https://github.com/your-username/simple-calculator.git)
   ```

2. **Navigate into the project directory:**
   ```bash
   cd simple-calculator
   ```

---

## Usage

Run the program directly using Python:

```bash
python3 calculator.py
```

### Example Interactive Session

```text
Select operation:
1. Add
2. Subtract
3. Multiply
4. Divide

Enter choice (1/2/3/4): 1
Enter first number: 12
Enter second number: 8

Result: 12.0 + 8.0 = 20.0

Do you want to perform another calculation? (yes/no): no
Goodbye!
```

---

## Code Example

Below is the core logic contained in `calculator.py`:

```python
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error: Division by zero!"
    return x / y

def main():
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

    choice = input("Enter choice (1/2/3/4): ")

    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(f"Result: {num1} + {num2} = {add(num1, num2)}")
        elif choice == '2':
            print(f"Result: {num1} - {num2} = {subtract(num1, num2)}")
        elif choice == '3
