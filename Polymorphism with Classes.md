# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
from abc import ABC, abstractmethod
class Food(ABC):
    @abstractmethod
    def get_type(self) -> str:
        pass

    @abstractmethod
    def get_color(self) -> str:
        pass
class Beans(Food):
    def get_type(self) -> str:
```
## Output
<img width="587" height="90" alt="exp1" src="https://github.com/user-attachments/assets/3a74bab6-fb35-4b92-bf7d-14c9df80dfb6" />

## Result
The program successfully creates class and returns type using polymorphism
