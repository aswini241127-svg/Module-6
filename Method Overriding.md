# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```
class Fish:
    def type(self):
        return "I am a fish."
class Shark(Fish):
    def type(self):
        return "I am a shark, a type of fish."
fish = Fish()
print(fish.type())  # Output: I am a fish.

shark = Shark()
print(shark.type())  # Output: I am a shark, a type
```
## OUTPUT
<img width="386" height="84" alt="exp1" src="https://github.com/user-attachments/assets/058f9cfa-f5b9-4c19-a6ee-58bb776a4b8e" />

## RESULT
The program successfully creates class inheritance
