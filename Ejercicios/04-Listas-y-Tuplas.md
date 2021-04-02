# Ejercicio 1

Dada la siguiente lista `[12, 23, 5, 29, 92, 64]` realiza las siguientes operaciones y vete mostrando la lista resultante por pantalla:

1. Elimina el último número y añádelo al principio.
2. Mueve el segundo elemento a la última posición.
3. Añade el número `14` al comienzo de la lista.
4. Suma todos los números de la lista y añade el resultado al final de la lista.
5. Fusiona la lista actual con la siguiente: `[4, 11, 32]`
6. Elimina todos los números impares de la lista.
7. Ordena los números de la lista de forma ascendente.
8. Vacía la lista.

## Resultado

```
[64, 12, 23, 5, 29, 92]
[64, 23, 5, 29, 92, 12]
[14, 64, 23, 5, 29, 92, 12]
[14, 64, 23, 5, 29, 92, 12, 239]
[14, 64, 23, 5, 29, 92, 12, 239, 4, 11, 32]
[14, 64, 92, 12, 4, 32]
[4, 12, 14, 32, 64, 92]
[]
```

## Solución

```python
lista = [12, 23, 5, 29, 92, 64]
lista.pop()
lista.insert(0, 64)
print(lista)
lista.pop(1)
lista.append(12)
print(lista)
lista.insert(0, 14)
print(lista)
suma = sum(lista)
lista.append(suma)
print(lista)
lista1 = [4, 11, 32]
lista.extend(lista1)
print(lista)
impar = []
for x in lista:
    if x % 2 == 0:
        impar.append(x)
print(impar)
impar.sort()
print(impar)
impar.clear()
print(impar)
```

# Ejercicio 2

Crea un programa que solicite al usuario 5 números y los guarde en una lista. A continuación el programa pedirá otros 5 números al usuario almacenándolos en una segunda lista. El programa mostrará al usuario una lista que contenga los números que tienen en común las dos listas anteriores.

- Ejemplo: Lista 1 = `[6,14,11,78,5]` y Lista 2 = `[3,14,22,78,9]`
- Resultado: `[14, 78]`

## Solución

```python
lista1 = []
for x in range(5):
    a = int(input("Introduce un número list 1: "))
    lista1.append(a)

lista2 = []
for x in range(5):
    a = int(input("Introduce un número list 2: "))
    lista2.append(a)

comparacion = []
for x in lista1:
    if x in lista2:
        comparacion.append(x)
print(comparacion)
```
