# `self` in Python OOP — Theory

## 1. Definition
- `self` refers to the **current instance** of the class.
- It is used inside class methods to access and modify the attributes and methods of the current object.
- It works like `this` in other programming languages such as Java or C++.
- `self` is **not a Python keyword**; it is a naming convention.

---

## 2. Purpose
- Allows each object to keep its **own separate data**.
- Helps methods identify **which object's data** to work with.
- Passed **automatically** by Python when an object calls its method.

---

## 3. Key Points
- Always the **first parameter** in instance methods.
- Methods can access object attributes only through `self`.
- You do not pass `self` manually when calling methods; Python does it internally.
- It is possible to use another name instead of `self`, but it is not recommended.

---

## 4. Common Interview Questions
1. **What is `self` in Python classes?**  
   A reference to the current object, automatically passed to instance methods.
2. **Is `self` a keyword?**  
   No, it is a convention.
3. **Why is `self` required?**  
   Without it, methods cannot distinguish between the attributes of different objects.
4. **Can we call an instance method without `self` as a parameter?**  
   No, `self` must be present in the method definition.

---

## 5. Mistakes to Avoid
- Forgetting to include `self` in method definitions will cause a `TypeError`.
- Accidentally naming a variable `self` outside of its intended purpose may cause confusion.

---

**In short:**  
`self` is the link between a class’s methods and the data stored in each specific object.
