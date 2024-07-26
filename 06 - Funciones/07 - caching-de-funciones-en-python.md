> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/caching-de-funciones-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Implementación de Caching con `functools.lru_cache`
```python
from functools import lru_cache

@lru_cache(maxsize=128)
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)

print(factorial(10))  # Cálculo normal
print(factorial(10))  # Resultado cacheado
```


## Implementación Manual de Caching
```python
cache = {}

def factorial(n):
    if n in cache:
        return cache[n]
    if n == 0:
        result = 1
    else:
        result = n * factorial(n-1)
    cache[n] = result
    return result

print(factorial(10))  # Cálculo normal
print(factorial(10))  # Resultado cacheado
```


