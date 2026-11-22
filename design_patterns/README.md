
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
