# Difference Between Instance Variables and Class Variables

## 1.  School Example
Think of a **school** as a class,  
and **students** as objects created from that class.

- **Class Variable** → Something common to **all students**.  
  Example: `school_name = "ABC Public School"`
- **Instance Variable** → Something unique to **each student**.  
  Example: `name = "Karthik"`, `roll_no = 101`

---

## 2. Instance Variables
- Belong to a **specific object**.
- Defined **inside `__init__`** using `self`.
- Each object gets **its own copy** of instance variables.
- Changes in one object’s instance variable do **not** affect other objects.

Example:
```python
class Student:
 school_name="ABC public school"
    def __init__(self, name, roll_no):
        self.name = name        # Instance Variable
        self.roll_no = roll_no  # Instance Variable
