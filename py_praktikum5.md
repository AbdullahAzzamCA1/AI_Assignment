## Python Praktikum 5 - Artificial Intelligence

Source Code

Nomor 1 & 2
```py
# Nomor 1
print("\nPraktikum_Python_5_Nomor_1")
print("="*70)
def luas_pp(panjang,lebar):
    luas = panjang * lebar
    print("Luas Persegi  =",luas)
def luas_segitiga(alas, tinggi):
    luas = (alas * tinggi) / 2
    print("Luas Segitiga =",luas)
def luas_lingkaran(r):
    luas = 22/7 * r * r
    print("Luas Segitiga =",luas)
luas_pp(4,6)
luas_segitiga(4, 6)
luas_lingkaran(7)
```

![scn2](https://user-images.githubusercontent.com/92994688/142637171-ea9fca1a-17e1-46d6-a166-8cbe7cb266b7.png)


Nomor 3 - 8
```py
from os import system
from tabulate import tabulate
from math import factorial
system('cls')
print("\n")

# Nomor 3
print("\nPraktikum_Python_5_Nomor_3")
print("="*70)
def LuasSgt(alas,tinggi):
    luas = alas * tinggi
    return luas   
print("Luas Segitiga =",LuasSgt(5,8))

# Nomor 4
print("\nPraktikum_Python_5_Nomor_4")
print("="*70)
n_input = int(input("Masukkan Jumlah Data : "))

def program1(n):
    list_num = []
    for i in range(n):
        data_input = int(input("Masukkan Data : "))
        list_num.append(data_input)
    print("Nilai tertinggi dari list ",list_num,"=",max(list_num))
program1(n_input)

# Nomor 5
print("\nPraktikum_Python_5_Nomor_5")
print("="*70)

def program2():
    # input
    n_input = int(input("\nMasukkan Jumlah Data : "))
    # proses & display
    list_num = []
    list_x   = []
    for i in range(n_input):
        data_input = int(input("Masukkan Data : "))
        list_num.append(data_input)
        if list_num[i] % 2 == 0:
            list_x.append([i,list_num[i]])
    table = tabulate(list_x, headers=['No Index','Bilangan Genap'], tablefmt='pretty')
    print(table)
    close = input("Ulangi lagi (y/t)? : ")
    if close == 'y':
        program2()
program2()

# Nomor 6
print("\nPraktikum_Python_5_Nomor_6")
print("="*70)
n = int(input("Input nilai N : "))
def fact(n):
    print(str(n)+"! = ", end = "")
    print((" x ".join(str(i) for i in range(n, 0, -1))), "=", factorial(n))
fact(n)


# Nomor 7
print("\nPraktikum_Python_5_Nomor_7")
print("="*70)
i = [1,2,3,4,5]
j = [6,7,8,9,10]
def sumlist(a,b):
    zip_list = zip(a,b)
    sum = [x + y for (x, y) in zip_list]
    return sum
print(i,"+",j,"=",sumlist(i,j))

print("\nPraktikum_Python_5_Nomor_8")
print("="*70)
print("belum tau pak :) yang akar persamaan kuadrat")
print("="*70)
nilai_awal  = int(input("Nilai awal     : "))
banyak_suku = int(input("Banyak suku    : "))
rasio       = int(input("Rasio          : "))
def aritmatik(A,B,N):
    value   = int(A)
    for i in range(A,B+2):
        print(value, end = ' ')
        value += N
aritmatik(nilai_awal,banyak_suku,rasio)
```

Output

![output1](https://user-images.githubusercontent.com/92994688/142637138-5a6d66ec-9716-4605-89f3-01113fa5e581.png)

![output2](https://user-images.githubusercontent.com/92994688/142637155-4157b937-b8d9-4f89-a9e0-5c5f7201966f.png)

![output3](https://user-images.githubusercontent.com/92994688/142637162-9b7ad19a-f65a-4902-9a01-403fc3288dda.png)

