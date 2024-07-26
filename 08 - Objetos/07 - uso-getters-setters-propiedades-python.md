> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/uso-getters-setters-propiedades-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Implementación de Getters y Setters
```python
class Persona:
    def __init__(self, nombre, edad):
        self._nombre = nombre
        self._edad = edad
    
    def get_nombre(self):
        return self._nombre
    
    def set_nombre(self, nombre):
        if isinstance(nombre, str):
            self._nombre = nombre
        else:
            raise ValueError("El nombre debe ser una cadena de texto")
    
    def get_edad(self):
        return self._edad
    
    def set_edad(self, edad):
        if isinstance(edad, int) and edad > 0:
            self._edad = edad
        else:
            raise ValueError("La edad debe ser un número entero positivo")
```


## Uso de Getters y Setters
```python
persona = Persona("Juan", 25)
print(persona.get_nombre())  # Salida: Juan
persona.set_nombre("Carlos")
print(persona.get_nombre())  # Salida: Carlos

print(persona.get_edad())  # Salida: 25
persona.set_edad(30)
print(persona.get_edad())  # Salida: 30
```


