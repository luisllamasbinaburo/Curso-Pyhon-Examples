> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/iteradores-e-iterables-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## iteradores-e-iterables-en-python
```python
# Ejemplos de iterables
lista = [1, 2, 3, 4, 5]
cadena = "Python"
tupla = (1, 2, 3)
conjunto = {1, 2, 3}
```


## Uso de iterables
```python
# Ejemplo de uso de un iterable en un bucle for
lista = [1, 2, 3, 4, 5]

for elemento in lista:
    print(elemento)

# Salida: 1, 2, 3, 4, 5
```


## Creación de un Iterador
```python
# Ejemplo de creación de un iterador personalizado
class Contador:
    def __init__(self, inicio, fin):
        self.inicio = inicio
        self.fin = fin

    def __iter__(self):
        self.numero = self.inicio
        return self

    def __next__(self):
        if self.numero <= self.fin:
            resultado = self.numero
            self.numero += 1
            return resultado
        else:
            raise StopIteration

# Uso del iterador personalizado
contador = Contador(1, 5)
iterador = iter(contador)

for numero in iterador:
    print(numero)

# Salida: 1, 2, 3, 4, 5
```


## Creando un Iterador desde un Iterable
```python
lista = [1, 2, 3, 4, 5]

# Crear un iterador a partir de un iterable
iterador = iter(lista)

print(next(iterador))  # Salida: 1
print(next(iterador))  # Salida: 2
print(next(iterador))  # Salida: 3
print(next(iterador))  # Salida: 4
print(next(iterador))  # Salida: 5
print(next(iterador))  # Stop iteration
```


## Usando Iteradores en Funciones y Métodos
```python
# Usar iteradores en funciones y métodos
def recorrer(iterable):
    iterator = iter(iterable)
    while True:
        try:
            elemento = next(iterator)
            print(elemento)
        except StopIteration:
            break

# Ejemplo de uso
cadena = "Python"
recorrer(cadena)

# Salida: P, y, t, h, o, n
```


