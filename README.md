# My_second_repo

import random
def parzyste(x):
    y = []
    for i in range(0,len(x)):
        if x[i]%2==0:
            y.append(x[i])
    return y

lista = []
for i in range(0,10):
    dodaj = random.randint(0,10)
    lista.append(dodaj)
print(lista)
print(parzyste(lista))
