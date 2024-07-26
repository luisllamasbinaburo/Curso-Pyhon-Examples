> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/constructores-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Ejemplo básico de Constructor
```python
# Definición de una clase con constructor
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

# Creación de instancias utilizando el constructor
persona1 = Persona("Juan", 30)
persona2 = Persona("María", 25)

# Acceso a los atributos de las instancias
print(persona1.nombre, persona1.edad)  # Salida: Juan 30
print(persona2.nombre, persona2.edad)  # Salida: María 25
```


## Definición de atributos opcionales
```python
class Coche:
    def __init__(self, marca, modelo, color="negro"):
        self.marca = marca
        self.modelo = modelo
        self.color = color

# Creación de instancias
coche1 = Coche("Toyota", "Corolla")
coche2 = Coche("Tesla", "Model S", "rojo")

print(coche1.marca, coche1.modelo, coche1.color)  # Salida: Toyota Corolla negro
print(coche2.marca, coche2.modelo, coche2.color)  # Salida: Tesla Model S rojo
```


