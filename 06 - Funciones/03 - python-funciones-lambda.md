> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-funciones-lambda/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Funciones Lambda
```python
lambda parametros: expresion
```

```python
suma = lambda x: x * x
```


## Funciones lamba con múltiples argumentos
```python
# Sintaxis: lambda argumentos: expresión
suma = lambda x, y: x + y
print(suma(3, 5))  # Output: 8
```


## Suma de dos números
```python
suma = lambda x, y: x + y
print(suma(3, 5))  # Output: 8
```


## Filtrado de una lista
```python
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
pares = list(filter(lambda x: x % 2 == 0, numeros))
print(pares)  # Output: [2, 4, 6, 8, 10]
```


## Mapeo de una lista
```python
numeros = [1, 2, 3, 4, 5]
cuadrados = list(map(lambda x: x ** 2, numeros))
print(cuadrados)  # Output: [1, 4, 9, 16, 25]
```


