# Tugas Python 6 - Artificial Intelligence

Source code python :
```py
from os import system
system('cls')

# Exception & general exception
print("\n\nException & general exception")
print("="*40)

try:
    level = int(input("Input your level : "))
    level /= 0
    print(level)
# #exception
# except ZeroDivisionError:                                     
#     print("\nZeroDivisionError") 
                   
# except ValueError:
#     print("\nInput invalid, Please input number correctly")

# General exception
except:
    print("\nProgram error")

# Reading file
print("\n\nReading file")
print("="*40)
data = open("data.txt", "r") # w=clr&write, a=write, r+=read&write, r=read
# print(data.read())
arr = data.readlines()
print(arr, "\n")
index = 1
for user in arr:
    print(f"{index} - {user}")
    index += 1

# Writing file
print("\n\nWriting file")
print("="*40)
print(data.writable())
data = open("data.txt", "a") # w=clr&write, a=write, r+=read&write, r=read
data.write("Dazai - psikologi - 2020") #

data = open("data_2.txt", "w") #createnewfile
data.write("Welcome To txt files..!!")
data.close()
```

Source code txt before run program:
```txt
Izaya - Informatika - 2020
Khun - Mesin - 2020
Granger -  Industri - 2020
```

Output : 

![outputpy6](https://user-images.githubusercontent.com/92994688/140857644-331e7257-ac2f-413d-bf5e-d964a19f080e.png)


Source code txt1 after run program:
```txt
Izaya - Informatika - 2020
Khun - Mesin - 2020
Granger -  Industri - 2020
Dazai - psikologi - 2020
```


Source code new txtafter run program:
```txt
Welcome To txt new files..!!
```
