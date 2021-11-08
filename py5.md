
## Tugas Python 5 - Artificial Intelligence

source code

```py
from os import name, system
system('cls')

# Aplikasi Terbilang
print("\n\nAplikasi Terbilang")
print("="*40)
num = input("Masukkan Angka : ")
num_map = {
    "1" : "Satu",
    "2" : "Dua",
    "3" : "Tiga",
    "4" : "Empat",
    "5" : "Lima",
    "6" : "Enam",
    "7" : "Tujuh",
    "8" : "Delapan",
    "9" : "Sembilan",
}
output = ""
for i in num:
    terbilang  = num_map.get(i, "Invalid")
    output += terbilang + " "
print(output)

# Emoji converter
print("\n\nEmoji converter")
print("="*40)
msg = input(">>> ")
emoji_map = {
    ":)" : "🙂",
    ":D" : "😀",
    ":|" : "😐",
}
words = msg.split(" ")
output = ""
for i in words:
    output += emoji_map.get(i, i) + " "
print(output)

# Function, Parameter, Keyword Argumen
print("\n\nFunction, Parameter, Keyword Argumen")
print("="*40)
def greet(name, point):
    print(f"\n    Hello {name} [point : {point}]")  
    print("    Good luck on your python learning..😃\n")

print("Start..")
greet("Izaya",1000)           #usingpotionalargument
greet(point=5000,name="Khun") #usingkeywordargument
print("..Finish")

# Return Value
print("\n\nReturn Value")
print("="*40)
def multiply(a, b):
    return a * b

result = multiply(10,10)
print(result)

print("\n\n")
```

output

![outputpy5](https://user-images.githubusercontent.com/92994688/140670555-d3c8a639-f8bd-47c3-b7d1-b868589f7b6c.png)
