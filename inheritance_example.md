# Inheritance: Beginner to Advanced

## 1. What is Inheritance?
![Inheritance Diagram](images/inheritance_diagram.png)  

Inheritance means **one class takes or “inherits” properties and behaviors from another class**.

Imagine a parent and child relationship:  
- The **parent** has some qualities.  
- The **child** gets all those qualities automatically but can also have its own unique things.

---

## 2. Why Use Inheritance?

- To **reuse code** — no need to write the same things again.  
- To **organize** your code better.  
- To create **hierarchies** like Animal → Dog → Puppy.

---

## 3. Basic Syntax
class ParentClass:  
    # Parent class code here  
    pass  

class ChildClass(ParentClass):  
    # Child class code here  
    pass  
- **Parent class** (also called base or super class) has common stuff.  
- **Child class** (also called derived or subclass) inherits from parent.  

---

## 4. Simple Example  


---

## 1. Basic Inheritance Example  


# Parent class  
class Animal:  
    def breathe(self):  
        print("Animal is breathing")  

# Child class inherits Animal  
class Dog(Animal):  
    def bark(self):  
        print("Dog is barking")  

# Use  
d = Dog()  
d.breathe()   
d.bark()      

A parent class like Animal has some behaviors.  
A child class like Dog inherits those behaviors and can add its own. 

---

## 5. How Child Class Inherits?

The child class automatically gets all methods and properties of the parent, so you don’t write them again.

---

## 6. Adding Child-specific Features

You can add new methods or variables in the child that don’t exist in the parent.

---

## 7. Overriding Parent Methods
class Animal:
    def sound(self):
        print("Animal sound")

class Dog(Animal):
    def sound(self):
        print("Bark")

d = Dog()
d.sound()


You can **replace** the parent method in the child to change behavior.

---

## 8. Calling Parent’s Method from Child
class Animal:
    def sound(self):
        print("Animal sound")

class Dog(Animal):
    def sound(self):
        print("Dog starts:")
        super().sound()

d = Dog()
d.sound()


Sometimes you want to override but still use the parent’s method inside the child by explicitly calling the parent’s method.

---

## 9. Constructor Inheritance
 class Animal:
    def __init__(self, name):
        self.name = name

class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name)
        self.breed = breed

d = Dog("Buddy", "Labrador")
print(d.name)
print(d.breed)


- Parent class usually has a constructor (initializer).  
- Child class can call parent’s constructor to reuse initialization.

---

## 10. Multilevel Inheritance (Chain of Inheritance)
class Animal:
    def breathe(self):
        print("Breathing")

class Dog(Animal):
    def bark(self):
        print("Barking")

class Puppy(Dog):
    def weep(self):
        print("Weeping")

p = Puppy()
p.breathe()
p.bark()
p.weep()


One child can become a parent for another child, forming a chain. For example, Puppy inherits from Dog, which inherits from Animal.

---

## 11. Multiple Inheritance

class Flyer:
    def fly(self):
        print("Flying")

class Swimmer:
    def swim(self):
        print("Swimming")

class Duck(Flyer, Swimmer):
    pass

d = Duck()
d.fly()
d.swim()



A class can inherit from multiple parents simultaneously (supported in some languages like Python).

---

## 12. Is-A Relationship

Inheritance models an “is-a” relationship:  
- A Dog **is an** Animal.  
- A Puppy **is a** Dog.

---

## 13. When NOT to use Inheritance

- Avoid inheritance if classes don’t have a clear “is-a” relationship.  
- Prefer **composition** (has-a relationship) instead, which is more flexible.

---

## Summary Chain

- Inheritance means child class takes parent’s features.  
- Child can add or override features.  
- You can call parent methods and constructors inside child.  
- Supports multi-level and multiple inheritance.  
- Models "is-a" relationships.

---

