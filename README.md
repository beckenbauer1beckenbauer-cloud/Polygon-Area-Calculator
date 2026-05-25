# Polygon Area Calculator

A Python-based geometric calculator that demonstrates the power of Object-Oriented Programming (OOP), specifically class inheritance, method overriding, and state management.

## 🚀 Key Features
- **Inheritance Mastery:** The `Square` class inherits all geometric logic from the `Rectangle` class while customizing initialization and setter methods.
- **Dynamic Representation:** Custom `__str__` methods provide clear, readable debugging info.
- **Geometric Utilities:** Calculates area, perimeter, and diagonals, and provides a visual ASCII representation of the shapes.
- **Spatial Analysis:** The `get_amount_inside` method calculates tiling potential, showing how many smaller shapes fit within a larger one.

## 🛠️ Technical Stack
- **Language:** Python 3
- **Concepts:** Object-Oriented Programming (Inheritance, Method Overriding, `super()`), Geometric Algorithms

## 🧩 Logic Overview
The architecture ensures that even when a `Square` is treated as a `Rectangle`, its side-length integrity is maintained by overriding the setter methods.



```mermaid
classDiagram
    Rectangle <|-- Square
    class Rectangle {
        +int width
        +int height
        +get_area()
        +get_perimeter()
        +get_diagonal()
        +get_picture()
        +get_amount_inside(shape)
    }
    class Square {
        +__init__(side)
        +set_side(side)
        +set_width(width)
        +set_height(height)
    }
