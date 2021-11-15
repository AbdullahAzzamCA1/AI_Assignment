
## Python Praktikum 1 - Artificial Intelligence

Source Code

```py
from os import system
system('cls')

print("\n")
# Nomor 1
print("Praktikum_Python_1_Nomor_1")
print("="*100+"\n")
line = '-' * 80
print(f"""
                    UNIVERSITAS KOMPUTER INDONESIA
                  Jl Dipati Ukur 112-114, Bandung
{line}
                   Nama       : Oemar Bakri
                   NIM        : 10205088
                   Jurusan    : Teknik Komputer
                   Fakultas   : Teknik dan Ilmu Komputer
{line}
"""
)
# Nomor 2
print("\nPraktikum_Python_2_Nomor_2")
print("="*100+"\n")
print(" DATA KECEPATAN MOBIL".rjust(75))
print('-'*80)
kecepatan   = int(input("kecepatan rata-rata (km/jam)   : "))
waktu       = int(input("Waktu tempuh (jam)             : "))
jarak       = kecepatan * waktu
print("Jarak tempuh                   :",jarak)

# Nomor 3
print("\nPraktikum_Python_3_Nomor_3")
print("="*100+"\n")
print("PROGRAM MENGHITUNG PEMBELIAN".center(80))
print('-'*80)
space    = " " * 24
harga  = int(input(f"{space}Harga satuan     : Rp."))
jumlah = int(input(f"{space}Jumlah pembelian : "))
diskon = int((harga*jumlah) * 10/100)
total  = int((harga*jumlah) - diskon)
print(f"""
{space}Diskon           : Rp.{diskon}
\n{space}Harga total   : Rp.{total}
""")

# Nomor 4
print("\nPraktikum_Python_4_Nomor_4")
print("="*100+"\n")
print("PROGRAM PENJUALAN BUKU".center(80))
print('-'*80)
space    = " " * 24
harga  = int(input(f"{space}Harga satuan     : Rp."))
jumlah = int(input(f"{space}Jumlah pembelian : "))
diskon = int(input(f"{space}Diskon           : "))
total  = int((harga*jumlah) - (harga*jumlah) * diskon/100)
print(f"\n{space}Harga total   : Rp.{total}")

# Nomor 5
print("\nPraktikum_Python_5_Nomor_5")
print("="*100+"\n")
print("PROGRAM MENGHITUNG TAGIHAN TELEPON".center(80))
print('-'*80)
space    = " " * 24
print(f"{space}DATA PELANGGAN")
nama       = input(f"{space}Nama                : ")
percakapan = int(input(f"{space}Percakapan          : "))
sms        = int(input(f"{space}SMS                 : "))
abonemen     = 20000
b_percakapan = percakapan * 1000
b_sms        = sms * 300
total = abonemen + b_percakapan + b_sms
print(f"""\n{space}TAGIHAN
{space}Abonemen            : Rp.{abonemen}
{space}Biaya Percakapan    : Rp.{b_percakapan}
{space}Biaya SMS           : Rp.{b_sms}
{space}Total tagihan       : Rp.{total}
""")

# Nomor 6
print("Praktikum_Python_6_Nomor_6")
print("="*100+"\n")
print("PROGRAM GAJI PEGAWAI".center(80))
space       = " " * 3

nama        = input(f"\n{space}Nama Karyawan      : ")
jumlah_anak = int(input(f"{space}Jumlah anak        : "))
Gaji_Pokok  = int(input(f"{space}Gaji Pokok         : "))
print('-'*80)
T_kesejahtraan = int(Gaji_Pokok * 20/100)
T_keluarga     = int((Gaji_Pokok * 10/100) * jumlah_anak)
gaji_kotor     = int(Gaji_Pokok + T_kesejahtraan + T_keluarga)
pajak          = int(gaji_kotor * 10/100)
gaji_bersih    = int(gaji_kotor - pajak)

print(f"""
{space}Gaji Pokok       T. Kesejahtraan     T. Keluarga     Pajak
{space}{Gaji_Pokok}                   {T_kesejahtraan}                {T_keluarga}         {pajak}
""")
print('-'*80)
print("Gaji kotor  : ",gaji_kotor)
print("Gaji Bersih : ",gaji_bersih)

# Nomor 7
print("\nPraktikum_Python_7_Nomor_7")
print("="*100+"\n")

nilai_uang    = int(input("Nilai uang  = "))
seribuan      = nilai_uang // 1000
dua_ratusan   = (nilai_uang % 1000) // 200
lima_puluhan  =(nilai_uang % 1000) % 200 // 50
print(f"{nilai_uang} rupiah = {seribuan} (seribuan) + {dua_ratusan} (duaratusan) + {lima_puluhan} (limapuluhan)")

# Nomor 8
print("\nPraktikum_Python_8_Nomor_8")
print("="*100+"\n")

gaji         = int(input("Gaji            = "))
hutang       = int(input("Hutang          = "))
biaya_harian = int((gaji - hutang) * 70/100)
tabungan     = int((gaji - hutang) * 20/100)
infak        =int((gaji - hutang) * 10/100)
print(f"""Biaya sehari2   = {biaya_harian}
Tabungan        = {tabungan}
Infak           = {infak}
""")
```

Output

![output1](https://user-images.githubusercontent.com/92994688/141795790-f107ffde-3745-458d-a0fd-e8b71ce60bcb.png)

![output2](https://user-images.githubusercontent.com/92994688/141795804-258d9ec3-1704-4ce0-ab96-54f463a39978.png)

![output3](https://user-images.githubusercontent.com/92994688/141795814-6bbc2cbb-d10f-4f68-b837-7681673e1ad8.png)

