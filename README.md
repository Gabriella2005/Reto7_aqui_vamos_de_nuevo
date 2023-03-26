#Reto 7

Bienvenidos, aquí podrán ver la solución que le dí a los ejercicios del reto 7,espero sea de su agrado y puedan aprender.

# 1) Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.

```
i = 1                              # asignamos 1 como el valor de i
while (i <= 100):                  #creamos un loop en donde i solo puede ser menor o igual a 100
    cuadrado = i**2                #creamos una formula para que nos de el cudrado de cada i
    print(i,"-",cuadrado)          #imprimimos i y su respectivo cuadrado
    i = i + 1                      #sumamos 1 a i y repetimos el ciclo
```

![image](https://user-images.githubusercontent.com/124614177/227801267-7ac4a070-8e09-4298-8704-ddb179153daa.png)

# 2) Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.

```
i = 1                                                                  #asignamos 1 a 'i'
print("a continuación tenemos los numeros impares de 1 hasta 999")     #imprimimos el enunciado
while (i <= 999):                                                      #abrimos un ciclo en el que 'i' debe ser menor o igual a 999
    if (i%2 > 0):                                                      #si el residuo de 'i'/2 es mayor a 0, 'i' es impar
        print(i)                                                       #imprimimos 'i'
    i = i + 1                                                          #sumamos 1 a 'i' para continuar el ciclo

n = 2                                                                  #asignamos 2 a 'n'
print("a continuación tenemos los numeros pares de 2 hasta 1000")      #imprimimos el enunciado
while (n <= 1000):                                                     #abrimos un ciclo en el que 'n' debe ser menor o igual a 1000
    if (n%2 < 1):                                                      #si el residuo de 'n'/2 es menor a 1, 'n' es par
        print(n)                                                       #imprimimos 'n'
    n = n + 1                                                          #sumamos 1 a 'n' para continuar el ciclo
```

![image](https://user-images.githubusercontent.com/124614177/227802980-aebbf5c8-13d9-46b7-b522-da16ecabdaa8.png)


# 3) Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado

```
n = int(input("ingrese un número mayor a 2: "))                                                 #asignamos un valor a 'n'
i = n                                                                                           #igualamos la variable 'i' con 'n'
print("a continuación tenemos los numeros pares en forma descendente desde ",n," hasta 2")      #imprimimos el enunciado
while (i >= 2):                                                                                 #abrimos un ciclo en el que 'i' debe ser mayor o igual a 2
    if (i%2 < 1):                                                                               #si el residuo de 'i'/2 es menor a 1, 'i' es par
        print(i)                                                                                #imprimimos 'i'
    i = i - 1                                                                                   #restamos 1 a 'i' para continuar el ciclo
```

![image](https://user-images.githubusercontent.com/124614177/227803369-6c9f7cc8-bfa3-4903-be11-aef6793b4e8b.png)


# 4) En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18:9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para informar en que año la población del país B superará a la de A.

```
A = 25000000                  #asignamos a 'A' la cantidad de habitantes del pais A
B = 18900000                  #asignamos a 'B' la cantidad de habitantes del pais B
an = 2022                     #asignamos a 'an' el año 2022

while (B <=A):                #iniciamos un ciclo si 'B' es menor a 'A'
    crec_A = ((A*2)/100)      #creamos la formula para saber el crecimiento de 'A'
    crec_B = ((B*3)/100)      #creamos la formula para saber el crecimiento de 'B'
    A = A + crec_A            #sumamos el crecimiento al valor inicial de 'A'
    B = B + crec_B            #sumamos el crecimiento al valor inicial de 'B'
    an = an + 1               #sumamos un año al valor inicial de 'an'
    print(an)                 #imprimimos el año
```

# 5) Imprimir el factorial de un número natural n dado.

```
n = int(input("ingrese un número natural: "))   #asignamos un valor a 'n'
i = n                                           #igualamos 'i' a 'n'
while n >= 2:                                   #iniciamos un ciclo en el que 'n' debe ser mayor o igual a 2
    n = n - 1                                   #restamos 1 a 'n'
    i = i * n                                   #multiplicamos 'i' por cada nueva'n'
    print(i)                                    #imprimimos 'i'
```

# 6) Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.

```
print("piensa en un número del 1 al 100, no lo cambies por favor, intentaré adivinarlo")  #imprimimos el enunciado
n = 60                                                                                    #asignamos 60 como valor de 'n'
print("el número que pensaste es 60?")                                                    #imprimimos una pregunta
i = input("por favor responde si es 'mayor','menor' o 'igual'").lower()                   #pedimos al usuario que nos indique si el número que pensó es mayor, menor o igual al dado

while i!= 'igual':                                                                        #iniciamos un ciclo si i es diferente a igual
    if i=='menor':                                                                        #miramos si el usuario nos dijo que el número que pensó es menor
        n = n-1                                                                           #restamos 1 a 'n'
    elif i=='mayor':                                                                      #miramos si el usuario nos dijo que el número que pensó es mayor
        n = n+1                                                                           #sumamos 1 a 'n'
    print("el número que pensaste es ",n,"?")                                             #preguntamos si el número dado es el pensado
    i = input("por favor responde si es 'mayor','menor' o 'igual'").lower()               #pedimos al usuario que nos indique si el número que pensó es mayor, menor o igual al dado
print("el número que pensaste es",n)                                                      #si el número dado es igual al pensado, lo imprimimos
```

# 7) Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.

```
n = int(input("ingrese un número de 2 a 50"))  #pedimos un numero entre 2 y 50
i = 1                                          #asignamos el valor 1 a 'i'

while (i <= n):                                #iniciamos un ciclo en el que 'i' debe ser menor o igual a 'n'
    if n%i==0:                                 #si el residuo de 'n'/'i' es 0, i es divisor
        print(i)                               #imprimimos 'i'
    i = i + 1                                  #sumamos 1 a 'i'
```

# 8) Implementar el algoritmo que muestre los números primos del 1 al 100. nota: use funciones

```
def primo():                #definimos primo()
    n = 1                   #asignamos el valor 1 a 'n'
    while (n<=100):         #iniciamos un ciclo si 'n' es menor o igual a 100
        i = 1               #asignamos el valor 1 a 'i'
        x = 0               #asignamos el valor 0 a 'x'
        while i <= n:       #iniciamos un ciclo si 'i' es menor o igual a 'n'
            if n%i==0:      #si el residuo de 'n'/'i' es 0, 'i' es divisor de 'n'
                x = x + 1   #sumamos 1 a 'x'
            i = i + 1       #sumamos 1 a 'i'
        if x == 2:          #si x es igual a 2, 'n' es primo
            print(n)        #imprimimos 'n'
        n = n + 1           #sumamos 1 a 'n'

primo()                     #ejecutamos la función primo
```
