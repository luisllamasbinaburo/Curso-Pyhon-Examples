> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/pattern-matching-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Sintaxis del Pattern Matching
```python
def analizar_dato(dato):
    match dato:
        case 1:
            return "Uno"
        case 2:
            return "Dos"
        case 3:
            return "Tres"
        case _:
            return "Otro valor"
```


## Listas y Tuplas
```python
def analizar_lista(lista):
    match lista:
        case [1, 2, 3]:
            return "Caso 1: 1 a 3"
        case [1, *resto]:
            return f"Caso 2: Empieza con 1 y luego {resto}"
        case _:
            return "Otro tipo de lista"

print(analizar_lista([1, 2, 3]))  # Salida: 'Caso 1: 1 a 3'
print(analizar_lista([1, 4, 5]))  # Salida: 'Empieza con 1 y luego [4, 5]'
print(analizar_lista([7, 8]))     # Salida: 'Otro tipo de lista'
```


## Diccionarios
```python
def analizar_diccionario(diccionario):
    match diccionario:
        case {"nombre": nombre, "edad": edad}:
            return f"Caso 1: Nombre: {nombre}, Edad: {edad}"
        case {"nombre": nombre}:
            return f"Caso 2: Nombre: {nombre}"
        case _:
            return "Otro tipo de diccionario"

print(analizar_diccionario({"nombre": "Ana", "edad": 30}))
# Salida: 'Caso 1: Nombre: Ana, Edad: 30'

print(analizar_diccionario({"nombre": "Luis"}))
# Salida: 'Caso 2: Nombre: Luis'
print(analizar_diccionario({"ciudad": "Madrid"}))
# Salida: Otro tipo de diccionario
```


## Patrones de Clase
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

def analizar_persona(persona):
    match persona:
        case Persona(nombre="Ana", edad=30):
            return "Persona Ana de 30 años"
        case Persona(nombre, edad):
            return f"Persona: {nombre}, Edad: {edad}"
        case _:
            return "Otro tipo de objeto"

persona1 = Persona("Ana", 30)
persona2 = Persona("Luis", 25)

print(analizar_persona(persona1))  # Salida: Persona Ana de 30 años
print(analizar_persona(persona2))  # Salida: Persona: Luis, Edad: 25
```


