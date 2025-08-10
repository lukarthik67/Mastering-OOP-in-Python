# Classes & Objects in Python

## What is a Class?
A **class** is a blueprint or template for creating objects.  
It defines:
- **Attributes (variables)** → Data or properties that belong to the class/object
- **Methods (functions)** → Actions or behaviors that objects can perform

---

## What is an Object?
An **object** is an **instance** of a class — a real-world entity created from the blueprint.  
Each object has its own data but follows the structure defined by the class.

---

## Constructor (`__init__` method)
- The **constructor** is a special method named `__init__` in Python.
- It is automatically called when an object is created.
- Used to initialize the attributes of the object.
- **`self`** refers to the current instance of the class.

---

## Methods in a Class
- **Methods** are functions defined inside a class.
- They represent the behavior of the objects.
- The first parameter is always `self`, which refers to the instance.

---

## Multiple Objects
- A single class can be used to create multiple objects.
- Each object will have its own set of attributes.
- Objects created from the same class can store different data.

---

## Class Variables vs Instance Variables
- **Class Variables** → Shared by all objects of the class.
- **Instance Variables** → Unique to each object and defined inside `__init__`.

---

## Real-world Analogy
Think of a **Class** as a **Blueprint** and an **Object** as the **Actual Product** built from it.

Example analogy:
- **Class** → Car design blueprint
- **Object** → My Car (Tesla, Red, Electric)

---

## Key Points to Remember
- A **class** defines the structure (attributes) and behavior (methods).
- An **object** is an instance of a class with its own data.
- `__init__` initializes object attributes during creation.
- `self` is a reference to the current object.
- Class variables are shared, instance variables are unique.

---

## Why Use Classes & Objects?
- Organizes code into logical units.
- Increases reusability and maintainability.
- Makes complex programs easier to understand.
- Allows modeling of real-world entities in code.

---

## Summary Table

| Term                  | Meaning                                                      |
|-----------------------|--------------------------------------------------------------|
| Class                 | Blueprint/template for creating objects                      |
| Object                | Instance of a class with actual data                         |
| Constructor (`__init__`) | Special method for initializing object attributes          |
| Method                | Function inside a class that defines behavior                |
| Class Variable        | Attribute shared by all objects of the class                  |
| Instance Variable     | Attribute unique to each object                               |
| self                  | Reference to the current instance of the class                |
