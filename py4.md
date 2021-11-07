
## Tugas Python 4 - Artificial Intelligence

Source code :

```py
from os import system
system('cls')

# For Loop
print("\n\nFor Loop")
print("="*40)
name =  "Izaya"
list = [1,2,3,4,5]
for i in name:
    print(i)
print("\n")
for i in list:
    print(i)
print("\n")
for list in range(1,6,2): #(frst,end,step)
    print(list)

# List
print("\n\nList")
print("="*40)
four_heaven_king = ["benimaru","diablo","shion","gobta"]
print(four_heaven_king)
print(four_heaven_king[0])
print(four_heaven_king[-3])
print(four_heaven_king[0:4])
for four_heaven_king in four_heaven_king:
    print(f"Nama : {four_heaven_king}")


# List Method
print("\n\nList Method")
print("="*40)
num =[10,35,44,59,24,68,88]
print(num)
num.append(77)
print(num)
num.insert(3,100)
print(num)
num.pop(3)
print(num)
num.remove(59)
print(num)
num.sort()
print(num)

# Penjumlahan list & Max Num
print("\n\nPenjumlahan list & Max Num")
print("="*40)
num = [1,2,3,4,5]
current_value = 0
for i in num:           #1
    current_value += i
print(current_value)
print(sum(num))         #2
num.sort()              #1
print(num[-1])
print(max(num))         #2
max = num[0]
for num in num:
    if num > max:
        max = num
print(max)

# Tuple Unpack
print("\n\nTuple Unpack")
print("="*40)
num = (2,4,6)           #Immutable support*count,index 
print(num, type(num))
x, y, z = num           #Unpack *Supported on list 
x, *a  = num   
print(x, y, z, a)

# Dictionary
print("\n\nDictionary")
print("="*40)
user = {
    "name"      : "Izaya Orihara",
    "age"       : 19,
    "is_admin"  : True
}
print(user.get("name"))
user["name"] = "izaya granger"
print(user.get("name"))
print(user.get("username"))
print(user.get("username", "Khun Izaya"))
```

Output :

![output1](https://user-images.githubusercontent.com/92994688/140665382-62217370-44a0-4d99-9c3a-244bf71ad9b1.png)
![output2](https://user-images.githubusercontent.com/92994688/140665386-fd34b6a7-68c1-4b48-934d-f9c19ed30a25.png)
