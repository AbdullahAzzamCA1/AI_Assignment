
## Tugas Python 3 - Artificial Intelligence

Source code 
```py
from os import name, system
system('cls')

# Condition (if,elif,else)
print("\n\nCondition")
print("="*40)
day = False
night = True

if day:                     #example
    print("Good morning")
elif night:
    print("Good night")
else:
    print("Hello")
print("Enjoy your day...!!")

# Comparison (>,<,==,>=,<=,!=)
print("\n\nComparison")
print("="*40)
rank = 1200

if rank >= 1000:            #example
    print("you're pro ")
elif rank >= 500:
    print("standart")
else:
    print("nooooooooob")

# Logic Operator (or,and,not)
print("\n\nLogic Operator")
print("="*40)
name = "Izaya Orihara"
validation = True

if len(name) > 3 or validation: #example
    print("Wlecome",name)
else:
    print("Nama terlalu pendek")

# While Loop (while condition)
print("\n\nWhile Loop")
print("="*40)
index = 1

while index <= 3:                       #example
    print("The program is running...")
    index += 1 # if there is not this syntax, the program will run without stop. (condition is still true)

print("Finish")

# Guess Number
print("\n\nGuessNumberProgram")
print("="*40)

chance = 0
secret_number = 4
limit = 3

while chance < limit:
    guess_number = int(input("Input number (1 - 9) : "))
    if guess_number == secret_number:
        print(f"YOU WIN, secret number = {guess_number}")
        break
    chance += 1
    if chance == 3:
        print("YOU LOSE")

# Calculator Application
print("\n\nCalculator Application")
print("="*40)
# Operation
oprtn = ""

while oprtn != "exit":
    
    oprtn = input("Masukkan Operasi          : ")

    if oprtn == "exit":
        print("\nTerima Kasih Telah Menggunakan Aplikasi Kami\n")
        break
    
    if oprtn != '+' and oprtn != "-" and oprtn != "*" and oprtn != "/":
        print("Perintah Tidak Dikenali\n")
        continue
        
    num1      = int(input("Masukkan Angka Pertama    : "))
    num2      = int(input("Masukkan Angka Kedua      : "))

    if oprtn == '+' :
        value = num1 + num2
    elif oprtn == '-' :
        value = num1 - num2
    elif oprtn == '*' :
        value = num1 * num2
    else:
        value = num1 / num2
    
    print(f"Hasil : {value}\n")      
```

Output

![outputpy3](https://user-images.githubusercontent.com/92994688/140634322-2f601468-67af-41c4-ab13-510eefb01fc1.png)

