# Exp.No:4.d
## FILES - FREQUENCY OF CHARACTERS IN A FILE


### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.


### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM
from collections import defaultdict

def create_file(file_path, content):

    with open(file_path, 'w') as file:
        file.write(content)

def char_frequency(file_path):

    freq_dict=defaultdict(int)
    with open(file_path,'r')as file:
        content=file.read()
        for char in content:
            freq_dict[char]+=1
    return freq_dict


### OUTPUT
![image](https://github.com/user-attachments/assets/99084e19-1539-4588-81de-d5db8a53fdb7) ![image](https://github.com/user-attachments/assets/157cfd8e-ef1e-4296-a24c-72b3bb9c2d9f) ![image](https://github.com/user-attachments/assets/635f3e0e-58d6-4f13-9bd3-01781947c4dd)

### RESULT
Thus,  Python program that reads a file and counts the frequency of each character was successfully implemented.
