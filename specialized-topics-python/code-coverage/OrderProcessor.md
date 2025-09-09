## Order Processing System in Python

Review and verify that the following Python classes are written accurately and adhere to PEP 8 guidelines:

```python
class Order:
    def __init__(self, customer=None, items=None):
        self.customer = customer
        self.items = items if items is not None else []

class Customer:
    def __init__(self, name):
        self.name = name

class OrderItem:
    def __init__(self, product_id, quantity, price):
        self.product_id = product_id
        self.quantity = quantity
        self.price = price
```

## Refactor and Test for Code Coverage

Refactor the `OrderProcessor` class to make it easier to maintain, enhance, and test all possible branches and exceptions. Ensure the code is idiomatic Python and easy to test.

```python
class OrderProcessor:
    def process_order(self, order):
        if order is None:
            raise ValueError("order cannot be None")
        if not order.items:
            raise ValueError("Order must have at least one item.")
        for item in order.items:
            if item.quantity <= 0:
                raise ValueError("Item quantity must be greater than zero.")
            if item.product_id == 0:
                if item.price > 100:
                    print("High value item with no product ID.")
                else:
                    print("Low value item with no product ID.")
            else:
                if item.price > 100:
                    print("High value item with product ID.")
                else:
                    print("Low value item with product ID.")
        if order.customer is None:
            raise ValueError("Order must have a customer.")
        self.process_payment(order)

    def process_payment(self, order):
        print("Processing payment for order.")
```

## Write unit tests for the OrderProcessor class to cover all possible branches and exceptions.
Test cases should include:
- Valid order processing
- Order with no items
- Order with invalid item quantity
- Order with no customer
- Items with different product IDs and price
Goal:
100% code coverage for the OrderProcessor class using pytest or unittest.

Show how to measure code coverage for this class using `coverage.py`.