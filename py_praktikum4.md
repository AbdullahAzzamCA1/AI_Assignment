## Python Praktikum 4 - Artificial Intelligence

Source Code
```py
from os import system
from tabulate import tabulate
system('cls')
print("\n")

# Nomor 1
print("\nPraktikum_Python_4_Nomor_1")
print("="*100)
tabel_nama    = []
tabel_nilai   = []
tabel_output  = []

for i  in range(1,6):
    nama  = input("Masukkan nama        : ")
    nilai = int(input("Masukkan nilai       : "))
    print()
    tabel_nama.append(nama)
    tabel_nilai.append(nilai)
    tabel_output.append([i,tabel_nama[i-1],tabel_nilai[i-1]])

table = tabulate(tabel_output, headers=['No','Nama','Nilai'], tablefmt='pretty')
print(table)
print("Jumlah Mahasiswa =",len(tabel_nama))
print("Rata - rata      =",sum(tabel_nilai)/len(tabel_nilai))

# Nomor 2
print("\nPraktikum_Python_4_Nomor_2")
print("="*100)
tabel_nama    = []
tabel_nilai   = []
tabel_output  = []
tabel_ket     = []

for i  in range(1,6):
    nama  = input("Masukkan nama        : ")
    nilai = int(input("Masukkan nilai       : "))
    print()
    tabel_nama.append(nama)
    tabel_nilai.append(nilai)
    if tabel_nilai[i-1] >= 60:
        ket = "Lulus"
    else:
        ket = "Tidak Lulus"
    tabel_ket.append(ket)

    tabel_output.append([i,tabel_nama[i-1],tabel_nilai[i-1],tabel_ket[i-1]])

table = tabulate(tabel_output, headers=['No','Nama','Nilai','Keterangan'], tablefmt='pretty')
print(table)
print("Jumlah Mahasiswa =",len(tabel_nama))
print("Rata - rata      =",sum(tabel_nilai)/len(tabel_nilai))
max        = max(tabel_nilai)
min        = min(tabel_nilai)
max_index  = tabel_nilai.index(max)
min_index  = tabel_nilai.index(min)
jmlh_lulus = tabel_ket.count("Lulus")
jmlh_gagal = tabel_ket.count("Tidak Lulus")
print(f"Nilai tertinggi  = {max} Oleh {tabel_nama[max_index]}")
print(f"Nilai terendah   = {min} Oleh {tabel_nama[min_index]}")
print(f"Jumlah Lulus     = {jmlh_lulus}")
print(f"Jumlah Gagal     = {jmlh_gagal}")

# Nomor 3
print("\nPraktikum_Python_4_Nomor_3")
print("="*100)
tabel_nama    = []
tabel_tugas   = []
tabel_uts     = []
tabel_uas     = []
tabel_na      = []
tabel_output  = []

jumlah_mahasiswa = int(input("Masukkan Jumlah Mahasiswa : "))
for i  in range(1,jumlah_mahasiswa+1):
    nama        = input("\nMasukkan nama          : ")
    nilai_tugas = int(input("Masukkan nilai tugas   : "))
    nilai_uts   = int(input("Masukkan nilai uts     : "))
    nilai_uas   = int(input("Masukkan nilai_uas     : "))
    na          = (30/10*nilai_tugas) + (30/100*nilai_uts) + (40/100*nilai_uas)
    tabel_nama.append(nama)
    tabel_tugas.append(nilai_tugas)
    tabel_uts.append(nilai_uts)
    tabel_uas.append(nilai_uas)
    tabel_na.append(na)
    tabel_output.append([i,tabel_nama[i-1],tabel_tugas[i-1],tabel_uts[i-1],tabel_uas[i-1],tabel_na[i-1]])

table = tabulate(tabel_output, headers=['No','Nama','Tugas','UTS','UAS','NA'], tablefmt='pretty')
print("\n",table)
avg_tugas = sum(tabel_tugas)/len(tabel_tugas)
avg_uts   = sum(tabel_uts)/len(tabel_uts)
avg_uas   = sum(tabel_uas)/len(tabel_uas)
avg_na    = sum(tabel_na)/len(tabel_na)
print(f"Rata - rata           {avg_tugas} {avg_uts} {avg_uas}  {avg_na}")

# Nomor 4
print("\nPraktikum_Python_4_Nomor_4")
print("="*100)
x = [int(x) for x in input("Masukkan nilai       : ").split()]
even_x = [even for even in x if even % 2 == 0]
print("Bernilai genap       :",' '.join(str(y) for y in even_x))

# Nomor 5
print("\nPraktikum_Python_4_Nomor_5")
print("="*100)
data = [10,99,98,22,11,8,7,66]
max  = max(data)
print(f"Bilangan terbesar dari list {data} = {max}")

# Nomor 6
print("\nPraktikum_Python_4_Nomor_6")
print("="*100)
x = [int(x) for x in input("Masukkan nilai       : ").split()]
# A
value = []
for a in range(len(x)):
    if a % 2 == 0:
        z = x[a]
        value.append(z)
print("berindeks genap      ="," ".join(map(str, value)))
# B - D
x_positif = [num for num in x if num > 0]
print("Bernilai positif     =",' '.join(str(y) for y in x_positif))
x_m3odd = [num for num in x if num % 3 == 0 and num % 2 == 1 ]
print("Ganjil x3            =",' '.join(str(y) for y in x_m3odd))
x_mod3 = [num for num in x if num % 3 != 0]
print("Tidak habis / 3      =",' '.join(str(y) for y in x_mod3))

# Nomor 7
print("\nPraktikum_Python_4_Nomor_7")
print("="*100)
x = [int(x) for x in input("Masukkan nilai       : ").split()]
x_mod5 = [num for num in x if num % 5 == 0]
print("Jumlah Kelipatan 5   =",len(x_mod5))

# Nomor 8
print("\nPraktikum_Python_4_Nomor_8")
print("="*100)
print("Ndak tau Pak :v")

# Nomor 9
print("\nPraktikum_Python_4_Nomor_9")
print("="*100)
print("Banyak bilangan di list sebelumnya =",len(x))

# Nomor 10
print("\nPraktikum_Python_4_Nomor_10")
print("="*100)
plus = [num for num in x if num > 0]
min = [num for num in x if num < 0]
print("Positif > Negatif" if len(plus) > len(min) else "Negatif > Positif")

# Nomor 11
print("\nPraktikum_Python_4_Nomor_11")
print("="*100)
X = [[1, 9],
     [8, 6]]
Y = [[1, 2],
     [3, 4]]
result = [[0, 0], 
          [0, 0]]
for i in range(len(X)):
    for j in range(len(Y[0])):
        for k in range(len(Y)):
            result[i][j] += X[i][k] * Y[k][j]
print("Matrix X")
for r in X:
    print(r)
print("Matrix Y")  
for r in Y:
    print(r)
print("Hasil Perkalian Matrix X * Y")
for r in result:
 print(r)

# Nomor 12
print("\nPraktikum_Python_4_Nomor_12")
print("="*100)
z = (1,2,3,4,5)
x = int(input("Angka pengali : "))
for i in z:
    print(x*i, end = ' ')

# Nomor 13
print("\nPraktikum_Python_4_Nomor_13")
print("="*100)
    
dictSatu = {"nim" : "12345678",
            "nama" : "Fatih",
            "IPK" : 3.90}
dictDua = {"hobi" : "main bola",
           "alamat" : "Bandung"}
dictTiga = {**dictSatu,**dictDua}

for x,y in dictTiga.items():
    print(x,y)
```

Output

![output1](https://user-images.githubusercontent.com/92994688/142430095-b6b66e4a-30db-4ca4-9a44-a52feebb59be.png)
![output 2](https://user-images.githubusercontent.com/92994688/142430081-a4f1c075-b5ad-4e6e-ae08-f93f8002ee43.png)
![output3](https://user-images.githubusercontent.com/92994688/142430097-a6928621-fca2-4828-8217-cf83c561d76e.png)
![output4](https://user-images.githubusercontent.com/92994688/142430102-71502851-dfc6-4017-b9a6-dfc79ac51b53.png)
![output5](https://user-images.githubusercontent.com/92994688/142430109-73e027f5-2dc8-4541-8307-dfa6fb6cc983.png)

