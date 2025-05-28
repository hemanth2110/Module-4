# Exp.No:4.e
## SEB - Write a Python class named Rectangle constructed by a length and width, has 2 methods.

---

### AIM  
To write a Python class named Rectangle constructed by a length and width, has 2 methods.
 1. setvalues - to set the values of length and breadth

2. a method which will compute the area of a rectangle.

### ALGORITHM

Start

Define a class rectangle with two methods:

setvalues(self, a, b) to assign values to the rectangle’s length and breadth

area(self) to compute and print the area as a × b

Input the length a of the rectangle

Input the breadth b of the rectangle

Create an object obj of the class rectangle

Call obj.setvalues(a, b) to assign the input values to the object

Call obj.area() to calculate and print the area

End

### PROGRAM
class rectangle:

    def setvalues(self,a,b):
        self.a=a
        self.b=b
    def area(self):
        print(self.a * self.b)
a=int(input())

b=int(input())

obj=rectangle()

obj.setvalues(a,b)

obj.area()
        
### OUTPUT
![image](https://github.com/user-attachments/assets/07f0ccdb-7912-4d64-99d8-88b5c8e6b3cc)

### RESULT
Thus, Python class named Rectangle constructed by a length and width, has 2 methods was implemented successfully.
