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
