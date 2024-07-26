> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/como-usar-objetos-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Definición de una Clase en Python
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        print(f"Hola, mi nombre es {self.nombre} y tengo {self.edad} años.")
```


## Creación de instancias
```python
juan = Persona("Juan", 30)
```


## Acceso a atributo y métodos
```python
juan = Persona("Juan", 30)
ana = Persona("Ana", 25)

juan.edad = 35;  # Cambiamos edad de Juan a 35
ana.edad = 28;   # Cambiamos edad de ana a 28

juan.saludar()  # Salida: Hola, mi nombre es Juan y tengo 35 años.
ana.saludar()   # Salida: Hola, mi nombre es Ana y tengo 28 años.
```


