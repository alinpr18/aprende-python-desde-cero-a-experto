# Ejercicio 1

Crea un programa que solicite un número al usuario y devuelva el siguiente mensaje:

- Si es mayor que 0: "Es un número positivo."
- Si es igual a 0: "Es igual a cero.
- Si es menor que 0: "Es un número negativo."

## Ejemplo

```
Introduce un número: 5
Es un número positivo
```

## Solución

```python
x = int(input("Introduce un número: "))
if x > 0:
    print("Es un número positivo")
if x == 0:
    print("Es igual a cero")
if x < 0:
    print("Es un número negativo")
```

# Ejercicio 2

Escribe un programa que solicite dos números enteros al usuario y muestre por pantalla la suma de todos los números enteros que hay entre los dos números (ambos números incluidos).

## Ejemplo

```
Introduce el número de inicio: 4
Introduce el número de fin: 8
El resultado es:  30
```

## Solución

```python
a = int(input("Introduce el número de inicio: "))
b = int(input("Introduce el número de fin: "))
c = 0
for x in range(a, b+1):
    if x % 2 == 0:
        c += x
    if x % 2 != 0:
        c += x
print(c)
```

# Ejercicio 3

Mejora el programa anterior para que muestre por separado la suma de los números pares y los impares.

## Ejemplo

```
Introduce el número de inicio: 4
Introduce el número de fin: 8
Los pares suman 18 y los impares 12
```

## Solución

```python
a = int(input("Introduce el número de inicio: "))
b = int(input("Introduce el número de fin: "))
par = 0
impar = 0
for x in range(a, b+1):
    if x % 2 == 0:
        par += x
    if x % 2 != 0:
        impar += x
print(f"Los pares suman {par} y los impares {impar}")
```

# Ejercicio 4

Escribe un programa que solicite al usuario un nombre de usuario y contraseña. El programa mostrará el mensaje "¡Bienvenido!" si el usuario introduce los siguientes datos:

- Nombre de usuario: root
- Contraseña: toor

Si los datos de acceso son incorrectos mostrará el mensaje "Acceso fallido" y el programa finalizará.

## Ejemplo

```
Introduce el nombre de usuario: root
Introduce la contraseña: toor
¡Bienvenido!
```

## Solución

```python
usuario = input("Introduce el nombre de usuario: ")
clave = input("Introduce la contraseña: ")
if (usuario and clave) == ("root" and "toor"):
    print("¡Bienvenido!")
else:
    print("Acceso fallido")
```

# Ejercicio 5

Mejora el programa anterior para que solo permita 3 intentos. Cada vez vez que el usuario introduzca datos de acceso incorrectos el programa mostrará el mensaje: "Datos incorrectos. Le quedan X intentos.", siendo X el número de intentos restantes. Tras el tercer fallo el programa mostrará el mensaje "Has agotado todos tus intentos." y finalizará.

## Ejemplo

```
Introduce el nombre de usuario: root
Introduce la contraseña: 123456
Datos incorrectos. Le quedan 2 intentos.
Introduce el nombre de usuario: root
Introduce la contraseña: abcd
Datos incorrectos. Le quedan 1 intentos.
Introduce el nombre de usuario: root
Introduce la contraseña: 123abc
Datos incorrectos. Le quedan 0 intentos.

Has agotado todos tus intentos.
```

## Solución

```python
contador = 1
while contador <= 3:
    usuario = input("Introduce el nombre de usuario: ")
    clave = input("Introduce la contraseña: ")
    if (usuario and clave) == ("root" and "toor"):
        break
    if (usuario and clave) != ("root" and "toor"):
        print(f"Datos incorrectos. Le quedan {3-contador} intentos")
        contador += 1
    if contador > 3:
        print("\nHas agotado todos tus intentos")
```

# Ejercicio 6

Crea un programa que reciba 5 números del usuario y muestre el mayor de todos por pantalla.

## Ejemplo

```
Introduce un número: 5
Introduce un número: -10
Introduce un número: 2
Introduce un número: 14
Introduce un número: 7
El número más alto es:  14
```

## Solución

```python
numeros = []
for x in range(5):
    a = input("Introduce un número: ")
    numeros.append(a)
print(f"El número más alto es: {max(numeros)}")
```

# Ejercicio 7

Mejora el programa anterior, de forma que el usuario pueda introducir tantos números como quiera. El programa solicitará números al usuario hasta que introduzca la palabra "fin". Entonces mostrará el mayor de todos por pantalla.

## Ejemplo

```
Introduce un número: 6
Introduce un número: 9
Introduce un número: 11
Introduce un número: 3
Introduce un número: 5
Introduce un número: fin
El número más alto es: 11
```

## Solución

```python
numeros = []
while True:
    a = input("Introduce un número: ")
    if a == "fin":
        break
    numeros.append(a)
print(f"El número más alto es: {max(numeros)}")
```
