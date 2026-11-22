
# Introduction to Design Patterns with Python

This project explores reusable object-oriented design patterns in Python.

## Learning Objectives

- Understand creational, behavioral, and structural design patterns.
- Apply the Open/Closed Principle.
- Extend existing systems without modifying their core logic.
- Understand composition over inheritance.

## Task 0: Factory — Extending a Registry

**File:** `0-factory.py`

This task demonstrates the Factory pattern using a vehicle registry.

The `VehicleFactory` supports Bus, Train, and Bike by default.

A Scooter is added dynamically using:

```python
factory.register_kind("scooter", Scooter)
```

The factory's `create()` method remains unchanged.

### Expected Output

```text
road
rails
lane
scooter_lane
```

### Run

```bash
python3 0-factory.py
```

## Requirements

- Python 3.10 or later
- PEP 8 coding style
- No external dependencies

## Task 2: Decorator - Adding a New Wrapper

File: 2-decorator.py

This task demonstrates the Decorator structural design pattern.

Coffee is the base beverage, costing 50 cents.

Decorators:
- MilkDecorator adds 10 cents.
- SugarDecorator adds 5 cents.
- CaramelDecorator adds 15 cents.

Decorators can be combined without modifying existing classes.

Example:

    cup3 = CaramelDecorator(MilkDecorator(SugarDecorator(Coffee())))

Expected output:

    Coffee + milk 60
    Coffee + sugar + milk 65
    Coffee + sugar + milk + caramel 80

Run:

    python3 2-decorator.py
