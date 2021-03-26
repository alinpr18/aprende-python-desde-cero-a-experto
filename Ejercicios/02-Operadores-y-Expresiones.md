# Ejercicio 1

Crea un programa que solicite al usuario un número del 1 al 10 y muestre por pantalla la tabla de multiplicación del 1 al 10. Ejemplo:

## Ejemplo

```
Introduce un número del 1 al 10: 3
3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
3 x 4 = 12
3 x 5 = 15
3 x 6 = 18
3 x 7 = 21
3 x 8 = 24
3 x 9 = 27
3 x 10 = 30
```

## Solución

```python
x = int(input("Introduce un número del 1 al 10: "))
print(f"""{x} x 1 = {x * 1}
{x} x 2 = {x * 2}
{x} x 3 = {x * 3}
{x} x 4 = {x * 4}
{x} x 5 = {x * 5}
{x} x 6 = {x * 6}
{x} x 7 = {x * 7}
{x} x 8 = {x * 8}
{x} x 9 = {x * 9}
{x} x 10 = {x * 10}""")
```

# Ejercicio 2

Crea un programa que solicite al usuario dos números enteros y muestre por pantalla el resultado de las siguientes operaciones: suma, resta, multiplicación y división. Ejemplo:

## Ejemplo

```
Introduce el primer número: 8
Introduce el segundo número: 2
La suma es: 10
La resta es: 6
La multiplicación es: 16
La división es: 4.0
```

## Solución

```python
n1 = int(input("Introduce el primero número: "))
n2 = int(input("Introduce el segundo número: "))
print(f"""La suma es: {n1 + n2}
La resta es: {n1 - n2}
La multiplicación es: {n1 * n2}
La división es: {n1 / n2}""")
```

# Ejercicio 3

Crea un programa que solicite al usuario el radio de un círculo y calcule el área. Nota: Utiliza 3.14159 como número PI para el cálculo del área.

## Ejemplo

```
Introduce el radio: 3
El área es: 28.274309999999996
```

## Solución

```python
radio = float(input("Introduce el radio: "))
pi = 3.14159
print(f"El área es: {pi * radio**2}")
```
