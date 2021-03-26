# Ejercicio 1

Escribe un programa que contenga las siguientes variables:

- nombre: tipo string y valor "Michael Jordan"
- edad: tipo integer y valor 50
- media_puntos: tipo float y valor 28.5
- activo: False

El programa deberá mostrar en pantalla todos los valores.

# Solución

```python
nombre = "Michael Jordan"
edad = 50
media_puntos = 28.5
activo = False
print(f"""Nombre: {nombre}
Edad: {edad}
Media de puntos: {media_puntos}
Actividad: {activo}""")
```

# Ejercicio 2

Escribe un programa que solicite el nombre, DNI y edad, lo almacene en 3 variables distintas y muestre por pantalla los valores introducidos.

# Solución

```python
nombre = input("Introduce tu nombre: ")
dni = input("Introduce tu DNI: ")
edad = int(input("Introduce tu edad: "))
print(f"""Nombre: {nombre}
DNI: {dni}
edad: {edad}""")
```

# Ejercicio 3

Escribe un programa que genere un string compuesto por los primeros 3 caracteres y los últimos 3 caracteres de un string introducido por el usuario. Pista: tendrás que utilizar la función `len()` en la obtención de los últimos 3 caracteres.

- Ejemplo 1: 'aprendiendo'
- Resultado 1: 'aprndo'
- Ejemplo 2: 'escribiendo código'
- Resultado 2: 'escigo'

# Solución

```python
frase = input("Introduce un frase: ")
sub_frase = frase[:3] + frase[-3:]
print(sub_frase)
```

# Ejercicio 4

Escribe un programa que solicite al usuario dos números y una frase. El primer número introducido se corresponderá a la posición de inicio del substring que deberá mostrar el programa por pantalla. El segundo número indicará la longitud de dicho substring.

- Ejemplo 1: Posicion=4, Longitud=8, Frase='Desarrollar es mi nueva afición'
- Resultado 1: "rrollar "
- Ejemplo 2: Posicion=8, Longitud=11, Frase='Bienvenido a la clase de programación'
- Resultado 2: "do a la cla"

# Solución

```python
n1 = int(input("Introduce un número: "))
n2 = int(input("Introduce otro número: "))
frase = input("Introduce una frase: ")
sub_frase = frase[n1:n2+n1]
print(sub_frase)
```

# Ejercicio 5

Escribe un programa que solicite al usuario una frase. A continuación le solicitará la letra que quiere reemplazar y por qué letra deberá reemplazarse. Por último el programa mostrará el número de veces que la letra está presente en la frase y el resultado final tras reemplazarla.

- Ejemplo: 'Desarrollar es mi nuevo pasatiempos', 'a','e'
- Resultado: 4 apariciones. 'Deserroller es mi nueve pesetiempos'

# Solución

```python
frase = input("Introduce una frase: ")
old = input("Escribe la letra a reemplazar: ")
new = input("Escribe la letra por la que deberá reemplazarse: ")
print(frase.replace(old, new))
```
