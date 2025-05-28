# Exp.No:4c
## EXCEPTION HANDLING


### AIM  

1. accept  number of  elements from the user eg. 45,55 and print the element 

2. get the index number "indexno" for print & add statement  eg., "10 is not accepted" instead of index error.


### ALGORITHM

Start

Try the following steps: 3. Input the number of elements, store in num_elements 4. Initialize an empty list elements 5. Repeat for num_elements times:

Input an integer and append to elements

Print the list elements

Input the index number indexno

Access and print the element at elements[indexno]

Handle Exceptions:

If an IndexError occurs (i.e., index is out of range):

Print "indexno is not accepted"

If a ValueError occurs (i.e., non-integer input is given):

Print "Invalid input! Please enter numbers only."

End

### PROGRAM
try:

    num_elements = int(input())
    
    elements = [int(input()) for _ in range(num_elements)]
    
    print(elements)  # Print the list

    indexno = int(input())

    print(elements[indexno])

except IndexError:

    print(f"{indexno} is not accepted")  # Handle out-of-range index

except ValueError:

    print("Invalid input! Please enter numbers only.")  # Handle invalid input


### OUTPUT
![image](https://github.com/user-attachments/assets/5d50f701-f8aa-4a0c-9ad7-9b43303657dd)


### RESULT
Thus, the given program was implemented in python successfully.
