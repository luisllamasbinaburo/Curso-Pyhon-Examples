> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/generadores-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Qué son los generadores
```python
def generador_simple():
    yield 1
    yield 2
    yield 3
```

```python
gen = generador_simple()
print(next(gen))  # Salida: 1
print(next(gen))  # Salida: 2
print(next(gen))  # Salida: 3
```


## Generadores con Bucles
```python
def contar_hasta(n):
    contador = 1
    while contador <= n:
        yield contador
        contador += 1
```

```python
for numero in contar_hasta(5):
    print(numero)

# salida: 1 2 3 4 5
```


## Generadores combinados
```python
def generador_anidado():
    yield from range(3)
    yield from range(10, 13)

for numero in generador_anidado():
    print(numero)

# salida: 0 1 2 10 11 12
```


## Generadores con expresiones
```python
gen = (x**2 for x in range(10))

for numero in gen:
    print(numero)

# salida: 0 1 4 9 16 25 36 49 64 81
```


