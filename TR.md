# Tugas Rekoknisi - Artificial Intelligence
<br><br/>


## Program luas dan keliling persegi panjang
   <br><br/>
   ![lkpp](https://user-images.githubusercontent.com/92994688/139077084-c185bb85-8be7-483f-b597-0ecaeeadea72.png)
   <br><br/>
   
## Program suhu
   <br><br/>
   A. Reamur ke celcius
   <br><br/>
   ![rtc](https://user-images.githubusercontent.com/92994688/139077174-12965e5d-db84-4820-834c-a6fdebf47cb3.png)
   <br><br/>
   B. Fahrenheit ke celcius
   <br><br/>
   ![ftc](https://user-images.githubusercontent.com/92994688/139078313-d7a47753-af37-4a3c-83ee-6e44ba4e9629.png)
   <br><br/>
   C. Celcius ke reamur
   <br><br/>
   ![ctr](https://user-images.githubusercontent.com/92994688/139078375-2858c0f1-97bc-45de-9610-5915afb4c771.png)
   <br><br/>
   D. Celcius ke fahrenheit
   <br><br/>
   ![ctf](https://user-images.githubusercontent.com/92994688/139078443-3c1d10fb-9785-4876-a0fc-cd98ffa25a5b.png)
   <br><br/>
   
##Visual Studio Code
   <br><br/>
   ![vscodee](https://user-images.githubusercontent.com/92994688/139091305-670e0b97-52e6-4c45-801d-053063ce75a8.png)
   
   Source code :
   
   # Luas Dan Keliling Panjang
   print("\nProgram Luas Dan Keliling Persegi Panjang")
   print("======================================")

   print("Masukkan Panjang")
   panjang = int(input())
   print("Masukkan Lebar")
   lebar = int(input())
   luas = panjang * lebar
   keliling = 2 * (panjang + lebar)
   print("Luas persegi panjang adalah      : " + str(luas))
   print("Keliling persegi panjang adalah  : " + str(keliling))


   # Suhu Konventer
   print("\n\n\nProgram Suhu Konventer")
   print("======================================")

   # ReamurToCelcius
   print("\nReamur Ke Celcius")
   r = float(input("Masukkan Nilai Reamur : "))
   c = float(5) / 4 * r
   print("Maka suhu dalam Celcius : " + str(c))


   # FahrenheitToCelcius
   print("\nFahrenheit Ke Celcius")
   f = float(input("Masukkan Nilai Fahrenheit : "))
   c = (f - 32) * (float(5) / 9)
   print("Maka suhu dalam Celcius : " + str(c))

   # CelciusToReamur
   print("\nCelcius Ke Reamur")
   c = float(input("Masukkan Nilai Celcius : "))
   r = float(4) / 5 * c
   print("Maka suhu dalam Reamur : " + str(r))

   # CelciusToFahrenheit
   print("\nCelcius Ke Fahrenheit")
   c = float(input("Masukkan Nilai Celcius : "))
   f = c * (float(9) / 5) + 32
   print("Maka suhu dalam Fahrenheit : " + str(f),"\n\n")











  
