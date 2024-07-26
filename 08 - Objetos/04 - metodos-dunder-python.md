> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/metodos-dunder-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Método `__init__`
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

persona1 = Persona("Alice", 30)
print(persona1.nombre)  # Salida: Alice
print(persona1.edad)    # Salida: 30
```


## Métodos `__str__` y `__repr__`
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def __str__(self):
        return f"Persona: {self.nombre}, {self.edad} años"
    
    def __repr__(self):
        return f"Persona('{self.nombre}', {self.edad})"

persona1 = Persona("Alice", 30)
print(str(persona1))  # Salida: Persona: Alice, 30 años
print(repr(persona1)) # Salida: Persona('Alice', 30)
```


## Método `__len__`
```python
class Grupo:
    def __init__(self, miembros):
        self.miembros = miembros
    
    def __len__(self):
        return len(self.miembros)

grupo = Grupo(["Alice", "Bob", "Charlie"])
print(len(grupo))  # Salida: 3
```


## Métodos `__getitem__`, `__setitem__` y `__delitem__`
```python
class MiLista:
    def __init__(self):
        self.data = []
    
    def __getitem__(self, index):
        return self.data[index]
    
    def __setitem__(self, index, value):
        self.data[index] = value
    
    def __delitem__(self, index):
        del self.data[index]

mi_lista = MiLista()
mi_lista.data = [1, 2, 3, 4, 5]
print(mi_lista[2])   # Salida: 3
mi_lista[2] = 30
print(mi_lista[2])   # Salida: 30
del mi_lista[2]
print(mi_lista.data) # Salida: [1, 2, 4, 5]
```


## Métodos `__iter__` y `__next__`
```python
class Contador:
    def __init__(self, max):
        self.max = max
        self.contador = 0
    
    def __iter__(self):
        return self
    
    def __next__(self):
        if self.contador < self.max:
            self.contador += 1
            return self.contador
        else:
            raise StopIteration

contador = Contador(5)
for numero in contador:
    print(numero)
```


## Métodos Dunder para Operaciones Aritméticas
```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __add__(self, otro):
        return Vector(self.x + otro.x, self.y + otro.y)
    
    def __repr__(self):
        return f"Vector({self.x}, {self.y})"

v1 = Vector(2, 3)
v2 = Vector(4, 5)
v3 = v1 + v2
print(v3)  # Salida: Vector(6, 8)
```


