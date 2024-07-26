> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-como-usar-propiedades/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Definición de Propiedades
```python
class Persona:
    def __init__(self, nombre, edad):
        self._nombre = nombre
        self._edad = edad

    @property
    def nombre(self):
        return self._nombre

    @nombre.setter
    def nombre(self, nombre):
        if isinstance(nombre, str):
            self._nombre = nombre
        else:
            raise ValueError("El nombre debe ser una cadena de texto")
    
    @property
    def edad(self):
        return self._edad

    @edad.setter
    def edad(self, edad):
        if isinstance(edad, int) and edad > 0:
            self._edad = edad
        else:
            raise ValueError("La edad debe ser un número entero positivo")
```


## Uso de Propiedades
```python
persona = Persona("Juan", 25)
print(persona.nombre)  # Salida: Juan
persona.nombre = "Carlos"
print(persona.nombre)  # Salida: Carlos

print(persona.edad)  # Salida: 25
persona.edad = 30
print(persona.edad)  # Salida: 30
```


