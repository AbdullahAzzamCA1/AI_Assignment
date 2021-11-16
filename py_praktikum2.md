## Python Praktikum 2 - Artificial Intelligence

Source Code
```py
from os import system
system('cls')

print("\n")
# Nomor 1
print("Praktikum_Python_2_Nomor_1")
print("="*100+"\n")
a = int(input("Masukkan Angka 1 : "))
b = int(input("Masukkan Angka 2 : "))
print("Max Bilangan     :",max(a,b))

# Nomor 2
print("\nPraktikum_Python_2_Nomor_2")
print("="*100)
a = int(input("Masukkan Angka 1 : "))
b = int(input("Masukkan Angka 2 : "))
c = int(input("Masukkan Angka 3 : "))
print("Max Bilangan     :",max(a,b,c))

# Nomor 3
print("\nPraktikum_Python_2_Nomor_3")
print("="*100)
a = int(input("Masukkan Angka 1     : "))
b = int(input("Masukkan Angka 2     : "))
c = int(input("Masukkan Angka 3     : "))
num = [a,b,c]
def duplicate(list_num):
  for i in list_num:
    if list_num.count(i) > 1:
          return True
    return False
result = duplicate(num)
if result:
  print("Bilangan yang sama   :",result)
else:
  print("Bilangan yang sama   :",result)

# Nomor 4
print("\nPraktikum_Python_2_Nomor_4")
print("="*100)
nama = input("Nama Anda   : ")
tinggi = int(input("Tinggi Anda : "))
ideal = tinggi - 100
print(f"Saudara {nama}, berat ideal anda adalah {ideal} kg")

# Nomor 5
print("\nPraktikum_Python_2_Nomor_5")
print("="*100+"\n")
nama = "Khun Izaya"
tugas  = 95
uts = 90
uas = 90
na = (25/100*tugas) + (35/100*uts) + (40/100*uas)
if na >= 75:
      grade = 'A'
elif 60 <= na < 70:
      grade = 'B'
elif 45 <= na < 60:
      grade = 'C'
elif na <45:
      grade = 'D'

print("DATA NILAI MAHASISWA".center(80))
print('-'*80)
print(f"""                        Nama    : {nama}
                        Tugas   : {tugas}
                        UTS     : {uts}
                        UAS     : {uas} 
""")
print('-'*80+"\n\n")
print("NILAI AKHIR DAN GRADE".center(80))
print('-'*80)
print(f"""                        Nama        : {nama}
                        Nilai Akhir : {na}
                        Grade       : {grade}
""")

# Nomor 6
print("\nPraktikum_Python_2_Nomor_6")
print("="*100+"\n")
space = '-'*80
space_input = " " * 28
print("DATA PEGAWAI".center(80))
print(space)
nama = input(f"{space_input}Nama              : ")
golongan = input(f"{space_input}Golongan          : ")
total_jam_kerja = int(input(f"{space_input}Total jam kerja   : "))
print(space+"\n\n")

if golongan == 'A':
    gaji_pokok = 500000
    tunjangan  = int(gaji_pokok * 10/100)
    lembur     = int((total_jam_kerja - 200) * 5000)
elif golongan == 'B':
    gaji_pokok = 700000
    tunjangan  = int(gaji_pokok * 15/100)
    lembur     = int((total_jam_kerja - 200) * 7500)
elif golongan == 'C':
    gaji_pokok = 900000
    tunjangan  = int(gaji_pokok * 20/100)
    lembur     = int((total_jam_kerja - 200) * 10000)
total = gaji_pokok + tunjangan + lembur
print("PERHITUNGAN GAJI".center(80))
print(f"""{space}
                            Gaji pokok  : {gaji_pokok}
                            Tunjangan   : {tunjangan}
                            Lembur      : {lembur}
{space}
                            Total       : {total}
""")
```

Output

![output1](https://user-images.githubusercontent.com/92994688/141984072-b81e6e26-3391-465d-8c38-bb023d90de09.png)

![output2](https://user-images.githubusercontent.com/92994688/141984080-ee423123-9053-466b-bb96-d454e76d7168.png)

![output3](https://user-images.githubusercontent.com/92994688/141984083-b5add675-873f-46fa-980c-d20e36745abb.png)
