# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math
class Shape(ABC):

    @abstractmethod
    def calculate_area(self):
        pass
class Rectangle(Shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height

    def calculate_area(self):
        return self.width * self.height
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def calculate_area(self):
        return math.pi * (self.radius ** 2)
rect = Rectangle(5, 3)
print("Rectangle area:", rect.calculate_area())

circle = Circle(4)
print("Circle area:", circle.calculate_area())
```
## Output
<img width="403" height="67" alt="exp1" src="https://github.com/user-attachments/assets/8b69d849-da4e-4661-b586-67d19ee8a677" />

## Result
The program successfully calculates area of shapes using abstarct method and classes
# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
# Encapsulation Example in Python

class Rectangle:
    # Constructor to initialize private variables
    def __init__(self, length, breadth):
        self.__length = length      # Private attribute
        self.__breadth = breadth    # Private attribute

    # Method to display private values
    def display(self):
        print("Length:", self.__length)
        print("Breadth:", self.__breadth)

# Create an object of the Rectangle class
rect = Rectangle(10, 5)

# Display private members using class method
rect.display()
```
## Output
<img width="382" height="112" alt="exp1" src="https://github.com/user-attachments/assets/7fca0216-7a85-499d-9bb1-7907ad0b9c07" />

## Result
The program successfully demonstrates Encapsulation in Python by defining a class with private data members (__length and __breadth). The private variables are accessed only through class methods, ensuring data protection and controlled access.
