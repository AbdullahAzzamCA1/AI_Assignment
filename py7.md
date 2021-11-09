# Tugas Python 7 - Artificial Intelligence

## Source Code
```py
from os import system
system('cls')

import csv
import mathematic
from mathematic import multiply, divide
from marketplace.plusandmin import plus, min
import random
import cowsay

# Reading file csv with blok
print("Reading file csv")
print("="*40)

data = open("data.csv", "r") # needed when we don't use with

data_csv = csv.reader(data, delimiter=",")
for row in data_csv:
        print(f"Name : {row[0]}. Magictype : {row[1]}. Guild : {row[2]}")

data.close() # needed when we don't use with


# Reading file csv with blok
print("\n\nReading file csv with blok")
print("="*40)
with open("data.csv", "r") as data: # more recomended

    data_csv = csv.reader(data, delimiter=",")

    for row in data_csv:
        print(f"Name : {row[0]}. Magictype : {row[1]}. Guild : {row[2]}")

# Module
print("\n\nModule") # Kumpulan dari fungsi fungsi
print("="*40)
# pemanggilan module ada diatas source code
print(mathematic.multiply(10,10))
print(mathematic.divide(20,  5))
print(multiply(5, 5))
print(divide(100, 5))

# Package
print("\n\nPackage") # kumpulan dari modul modul
print("="*40)
# pemanggilan module ada diatas source code
print(plus(10,30))
print(min(30, 100))

# Random
print("\n\nRandom") 
print("="*40)
# # pemanggilan module ada diatas source code
for index in range(5):
    print(random.randint(15, 25)) # Random in range
print("\n")

data_name = ['luffy','zoro','nami','usop','sanji','chopper','robin','franky', 'brook', 'jinbei']

# hell way :v
bottom_index = 0
top_index = len(data_name) - 1
# for i in range(5):
#     print(random.randint(bottom_index, top_index))
winner_index =  random.randint(bottom_index, top_index)
winner = data_name[winner_index]
print(f"The Winner : {winner}")

# piece of cake way
winner = random.choice(data_name)
print(f"The Winner : {winner}")

# Pip and virtualenv
print("\n\nPip and virtualenv") 
print("="*40)
cowsay.cow("Sepii...gooooo..!!")
cowsay.dragon("kaidoo is coming..!!!")
cowsay.ghostbusters("huuuuu....")
```

Syntax setup virtualenv on windows
```txt
 install : 
   py -m pip install --user virtualenv

create venv on windows :
  python -m virtualenv venv

activate :
  venv\Scripts\activate

deactivate :
  path\deactivate
```

Syntax setup cowsay
```txt
install : 
  pip install cowsay
    
uninstall :
  pip unsinstall cowsay
```


## Output 

![output1](https://user-images.githubusercontent.com/92994688/140887399-73133982-b45e-42b5-b3d8-2a14bb8d5963.png)
![output2](https://user-images.githubusercontent.com/92994688/140887413-dd1af629-39b8-48c2-92c1-0a699ed05c37.png)
![output3](https://user-images.githubusercontent.com/92994688/140887417-5e28823f-bd95-474b-8128-f6aa9974cf7d.png)
![setvenv](https://user-images.githubusercontent.com/92994688/140887421-60496b56-6fad-4a26-a2b5-207afcccf921.png)
