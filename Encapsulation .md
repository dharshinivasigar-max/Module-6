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
~~~
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth
        
        print(f"Inside Constructor - Length: {self.__length}, Breadth: {self.__breadth}")

rect = Rectangle(10, 5)
~~~

## Output
Inside Constructor - Length: 10, Breadth: 5
## Result
The program demonstrates Encapsulation by defining private attributes using the double underscore prefix (__). In Python, this triggers name mangling, which makes these variables inaccessible from outside the class instance. As shown, while the class can freely access self.__length and self.__breadth within its own methods (like the constructor), an attempt to print rect.__length from the main script would result in an AttributeError.
