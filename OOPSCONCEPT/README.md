# Object-Oriented Programming in Python

## 1. Complex Number Operations
Detailed implementation of complex number operations (addition, subtraction, multiplication, division) using object-oriented programming concepts.

## 2. Student Class with Instance and Class Variables
A `Student` class using instance and class variables to manage student details, marks, and the number of students.

## 3. Inheritance with Grandfather, Father, and Child Classes
Demonstrates inheritance and method overriding with a Grandfather, Father, and Child class structure.

## 4. Demonstrating Protected and Private Attributes in Python
Illustrates how protected and private attributes work in Python classes using the `User` and `Buyer` classes.

---

For full code examples and more details, check out the respective code blocks above.
**Code Summary** 
## 1.Complex Number Operations
#### Description:
###### The first part of the code implements a ComplexNumber class that supports basic arithmetic operations on complex numbers, such as addition, subtraction, multiplication, and division. The class also includes functionality for conjugating a complex number and checking for equality between two complex numbers.

#### Key Operations:
###### __init__(self, real, imag): Initializes the real and imaginary parts of the complex number.
###### __str__(self): Customizes the string representation of the complex number.
###### __add__(self, other): Adds two complex numbers.
###### __sub__(self, other): Subtracts two complex numbers.
###### __mul__(self, other): Multiplies two complex numbers.
###### __truediv__(self, other): Divides two complex numbers.
###### conjugate(self): Returns the conjugate of the complex number.
###### __eq__(self, other): Checks if two complex numbers are equal.


      +-------------------+
      | ComplexNumber      |
      +-------------------+
      | - real: float      |
      | - imag: float      |
      +-------------------+
      | + __add__(other)   |
      | + __sub__(other)   |
      | + __mul__(other)   |
      | + __truediv__(other)|
      | + conjugate()      |
      | + __eq__(other)    |
      +-------------------+
      
## 2. Student Class with Instance and Class Variables
### Description:
##### The Student class demonstrates the use of both instance variables and class variables. It includes methods to access and modify marks, authenticate changes, and track the total number of students using class variables.

#### Key Features:
##### Instance variables: name, rollno, and marks are specific to each Student object.
##### Class variables: __numberofStudents keeps track of the total number of students.
##### Private and protected attributes: __marks is private, and _field is protected.
##### Methods: Methods like getmarks(), setmarks(), and get_no_of_students() provide functionality for interacting with the student data.


      +------------------------+
      | Student                |
      +------------------------+
      | - name: string         |
      | - rollno: int          |
      | - __marks: int         |
      | - __numberofStudents: int|
      +------------------------+
      | + getmarks()           |
      | + setmarks()           |
      | + get_no_of_students() |
      | + study()              |
      | + play()               |
      +------------------------+


## 3. Inheritance in Python with Grandfather, Father, and Child Classes
### Description:
#### This code demonstrates the use of inheritance in Python. The Grandfather class is the base class, and the Father class inherits from it, extending its functionality. Both Grandfather and Father classes are extended by child classes to demonstrate method overriding.

#### Key Concepts:
###### Method Overriding: The speak() method is overridden in the Father class.
##### Inheritance: Father inherits from Grandfather, and the Child classes inherit from Father



      +------------------+
      | Grandfather      |
      +------------------+
      | - name: string   |
      | - age: int       |
      +------------------+
      | + show_details() |
      | + speak()        |
      +------------------+
             ^
             |
      +------------------+
      | Father           |
      +------------------+
      | - occupation: str|
      +------------------+
      | + show_occupation()|
      | + speak()          |
      +------------------+
## 4. Demonstrating Protected and Private Attributes in Python
#### Description:
The Buyer class demonstrates inheritance and access control. The Buyer class inherits from the User class, and both classes demonstrate how to handle protected and private attributes.

##### Key Concepts:
Protected attribute: _field can be accessed in subclasses (like Buyer).
Private attribute: __name is private to the Buyer class and cannot be accessed outside it.


      +------------------+
      | User             |
      +------------------+
      | - website: str   |
      | - _field: str    |
      | - __duration: str|
      +------------------+
      | + login()        |
      | + logout()       |
      +------------------+
             ^
             |
      +------------------+
      | Buyer            |
      +------------------+
      | - __name: string |
      +------------------+
      | + login()        |
      +------------------+


