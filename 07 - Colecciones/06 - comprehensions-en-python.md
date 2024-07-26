> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/comprehensions-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Introducción
```python
expresion for elemento in iterable
```

```python
expresion for elemento in iterable if condicion
```


## Comprensiones de Listas
```python
[expresion for elemento in iterable if condicion]
```

```python
# Crear una lista de cuadrados de números del 0 al 9
cuadrados = [x**2 for x in range(10)]

print(cuadrados)  # Salida: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

```python
# Crear una lista de cuadrados de los numeros 0 al 9 que son pares
cuadrados_pares = [x**2 for x in range(10) if x % 2 == 0]

print(cuadrados_pares)  # Salida: [0, 4, 16, 36, 64]
```


## Comprensiones Anidadas
```python
# Crear una matriz identidad de 3x3
matriz_identidad = [[1 if i == j else 0 for j in range(3)] for i in range(3)]

print(matriz_identidad)
# Salida: [[1, 0, 0], [0, 1, 0], [0, 0, 1]]
```


## Comprensiones de Conjuntos
```python
{expresión for elemento in iterable if condición}
```

```python
# Crear un conjunto de números impares del 0 al 9
impares = {x for x in range(10) if x % 2 != 0}

print(impares)  # Salida: {1, 3, 5, 7, 9}
```


## Comprensiones de Diccionarios
```python
{clave: valor for elemento in iterable if condición}
```

```python
# Crear un diccionario con números y sus cuadrados para números del 0 al 9
cuadrados_dict = {x: x**2 for x in range(10)}

print(cuadrados_dict)
# Salida: {0: 0, 1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64, 9: 81}
```

```python
# Crear un diccionario de cuadrados solo para números pares del 0 al 9
cuadrados_pares_dict = {x: x**2 for x in range(10) if x % 2 == 0}

print(cuadrados_pares_dict)
# Salida: {0: 0, 2: 4, 4: 16, 6: 36, 8: 64}
```


## Comprensiones de Generadores
```python
(expresion for elemento in iterable if condicion)
```

```python
# Crear un generador de cuadrados de números del 0 al 9
cuadrados_gen = (x**2 for x in range(10))

print(list(cuadrados_gen))  # Salida: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```


