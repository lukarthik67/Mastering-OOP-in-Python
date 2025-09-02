# `__str__()` in Python OOP

## 1. What is `__str__()`?
- `__str__()` is a **special method** in Python classes.
- It defines what should be **returned as a string** when you print an object.
- Without it, printing an object shows something like `<__main__.Student object at 0x0001FABC>`.

---

## 2. Local Example — Visiting Card Analogy
Think of an **object** as a person,  
and `__str__()` as the **way they introduce themselves** when you meet them.

- If they don’t have `__str__()` → they just show a random ID you can’t understand.  
- If they have `__str__()` → they give you clear details like:  
  `"Name: Karthik, Roll No: 100"`

---

## 3. Why Use It?
- Makes objects **human-readable**.
- Useful for debugging and displaying meaningful information.
- Helps in logging and printing object details.

---

## 4. Example

```python
class Student:
    def __init__(self, name, roll_no):
        self.name = name
        self.roll_no = roll_no

    def __str__(self):
        return f"Student Name: {self.name}, Roll No: {self.roll_no}"

# Without __str__ (comment it out to test), printing shows memory address
# With __str__, printing shows friendly text

s1 = Student("Karthik", 101)
print(s1)  # Output: Student Name: Karthik, Roll No: 101
