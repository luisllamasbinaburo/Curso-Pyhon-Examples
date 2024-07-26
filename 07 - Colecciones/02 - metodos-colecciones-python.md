> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/metodos-colecciones-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Función `map()`
```python
# Uso básico de map():
def cuadrado(x):
    return x ** 2

numeros = [1, 2, 3, 4, 5]
cuadrados = map(cuadrado, numeros)

print(list(cuadrados)) # [1, 4, 9, 16, 25]
```

```python
# Uso de map() con función lambda:
numeros = [1, 2, 3, 4, 5]
cuadrados = map(lambda x: x ** 2, numeros)

print(list(cuadrados)) # [1, 4, 9, 16, 25]
```


## Función `filter()`
```python
# Uso básico de filter():
def es_par(x):
    return x % 2 == 0

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
pares = filter(es_par, numeros)
```

```python
# Uso básico de filter():
def es_par(x):
    return x % 2 == 0

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
pares = filter(es_par, numeros)

print(list(pares))  # Output: [2, 4, 6, 8, 10]
```


## Funciones `any()` y `all()`
```python
# Uso de any() y all():
valores = [True, False, True, False, True]
hay_algun_verdadero = any(valores)  # True
todos_verdaderos = all(valores)     # False
```

```python
valores = [1, 2, 3, 4, 5]
algun_mayor_que_diez = any(map(lambda x: x > 10, valores))  # False
```


## Función `sorted()`
```python
# Uso básico de sorted():
numeros = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
numeros_ordenados = sorted(numeros)

print(numeros_ordenados) # Output: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]
```

```python
# Uso de sorted() con key y reverse:
palabras = ["python", "java", "c++", "ruby", "javascript"]
palabras_ordenadas = sorted(palabras, key=len, reverse=True)

print(palabras_ordenadas) # ['javascript', 'python', 'java', 'c++', 'ruby']
```


## Función `sum()`
```python
# Uso básico de sum():
numeros = [1, 2, 3, 4, 5]

suma_total = sum(numeros)  # 15
```


## Función `enumerate()`
```python
# Uso básico de enumerate():
equipos = ["Real Madrid", "Barcelona", "Atlético de Madrid"]
enumeracion_equipos = list(enumerate(equipos, start=1))

print(enumeracion_equipos) # [(1, 'Real Madrid'), (2, 'Barcelona'), (3, 'Atlético de Madrid')]
```


## Función `reduce()`
```python
# Uso básico de reduce():
from functools import reduce

def suma(x, y):
    return x + y

numeros = [1, 2, 3, 4, 5]
suma_total = reduce(suma, numeros)

print(suma_total) # Salida: 15
```


## Función `zip()`
```python
# Uso básico de zip():
nombres = ["Juan", "María", "Pedro"]
edades = [30, 25, 35, 40]

print(personas) # [("Juan", 30), ("María", 25), ("Pedro", 35)]
```


