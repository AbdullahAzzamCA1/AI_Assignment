## Python praktikum 3 - Artificial Intelligence

Source code


Nomor 1
```py
from os import system
from tabulate import tabulate
system('cls')
print("\n")

# Nomor 1
print("\nPraktikum_Python_3_Nomor_1")
print("="*100)
input = (input("Nilai Satuan : "))
satuan = float(input)
harga = 800
tabel = []
for i in range(1, 7):
    tabel.append([float(satuan),int((satuan/0.5) * harga)])
    satuan += 0.5
table = tabulate(tabel, headers=['satuan','harga'], tablefmt='pretty')
print(table)
```

Output nomor 1

![output1](https://user-images.githubusercontent.com/92994688/142205358-8eed613f-7a98-4c7e-9afa-b37dec7148d8.png)

Nomor 2 - 8
```py
from os import system
from math import factorial
import random
system('cls')
print("\n")

# Nomor 2
print("Praktikum_Python_3_Nomor_2")
print("="*100)
nilai_awal  = int(input("Nilai awal     : "))
banyak_suku = int(input("Banyak suku    : "))
rasio       = int(input("Rasio          : "))
value       = int(nilai_awal)
for i in range(nilai_awal,banyak_suku+1):
    print(value, end = ' ')
    value += rasio

# Nomor 3
print("\n\nPraktikum_Python_3_Nomor_3")
print("="*100)
x = [int(x) for x in input("Masukkan Nilai       : ").split()]
print("Total nilai          :", sum(x))
print("Rata - rata nilai    :", sum(x)/len(x))

# Nomor 4
print("\n\nPraktikum_Python_3_Nomor_4")
print("="*100)
r = float(input("Input nilai real         : "))
b = int(input("Input bilang bulat (+)   : "))
print(r,"^",b," = ",pow(r,b))

# Nomor 5
print("\n\nPraktikum_Python_3_Nomor_5")
print("="*100)
n = int(input("Input nilai N : "))
print(str(n)+"! = ", end = "")
print((" X ".join(str(i) for i in range(n, 0, -1))), "=", factorial(n))

# Nomor 6
print("\n\nPraktikum_Python_3_Nomor_6")
print("="*100)
secret_num = random.randint(0,10)
guess_number = ""
while secret_num != guess_number:
    guess_number = int(input("Input number (0 - 10) : "))
    if guess_number > secret_num:
        print("Angka tebakan lebih besar\n")
    elif guess_number < secret_num:
        print("Angka tebakan lebih kecil\n")
print("Selamat..!! Tebakan anda benar")

# Nomor 7
print("\n\nPraktikum_Python_3_Nomor_7")
print("="*100)
x = int(input("x        = "))
y = int(input("y        = "))    
deret = [int(deret) for deret in range(x+1,y)]
print("Deret    = ", end = "")
print(' '.join(str(i) for i in deret))
print("Jumlah = ", sum(deret))

# Nomor 8
print("\n\nPraktikum_Python_3_Nomor_8")
print("="*100)

print("== A ==".center(100))
print("== B ==".center(100))
n = 5
for i in range(n):
    for j in range(i+1):
        print(n-j, end = '   ')
    print()
print("== C ==".center(100))
n = 5
for i in range(n, 0, -1):
    for j in range(1, i + 1):
        print(j, end = '   ')
    print("\r")
print("== D ==".center(100))
print("== E ==".center(100))
n = 5
for i in range(1,n+1):
    print(str(i),str(i**2).rjust(10),str(i**3).rjust(10))
```

Output nomor 2 - 8

![output2](https://user-images.githubusercontent.com/92994688/142205368-97681658-cfa6-4dd5-8a80-85263a983dac.png)
![output3](https://user-images.githubusercontent.com/92994688/142205375-d56a0966-3fbc-41e0-beca-14a0b5f4b6e8.png)
