# Inheritance and OOP Code Examples

---

## 1. Basic Inheritance Example

```python
class Animal:
    def breathe(self):
        print("Animal is breathing")

class Dog(Animal):
    def bark(self):
        print("Dog is barking")

d = Dog()
d.breathe()
d.bark()
