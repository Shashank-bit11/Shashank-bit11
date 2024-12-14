
class Calculator:
    def __init__(self, a, b, operation):
        self.a = a
        self.b = b
        self.operation = operation

    def add(self):
        return self.a + self.b

    def subtract(self):
        return self.a - self.b

    def multiply(self):
        return self.a * self.b

    def divide(self):
        if self.b != 0:
            return self.a / self.b
        else:
            return "Error: Division by zero is not allowed"

    def calculate(self):
        operations = {
            'addition': self.add,
            'subtraction': self.subtract,
            'multiplication': self.multiply,
            'division': self.divide
        }

        if self.operation.lower() in operations:
            return operations[self.operation.lower()]()
        else:
            return "Error: Invalid operation"
Output: Error: Division by zero is not
```
