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

numer = str(input("Podaj numer telefonu: "))
def sprawdzenie(x):
    y = ["0","1","2","3","4","5","6","7","8","9"," ","-"]
    z = [" ", "-"]
    x_lista = list(x)
    a = len(x)
    for i in range(0,a):
        if x_lista[i] not in y:
            return "Numer powinien zawierac tylko cyfry!"
    for i in range(0,a-2):
        if x_lista[i]==z[0] or x_lista[i]==z[1]:
            x_lista.remove(x_lista[i])
    x = "".join(x_lista)
    return x
print(sprawdzenie(numer))
