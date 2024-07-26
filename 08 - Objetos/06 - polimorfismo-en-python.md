> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/polimorfismo-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## polimorfismo-en-python
```python
# Definición de la clase Persona
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def saludar(self):
        print(f"Nombre: {self.nombre}, Edad: {self.edad}")
```

```python
# Definición de la clase Profesor que hereda de Persona
class Profesor(Persona):
    def __init__(self, nombre, edad):
        super().__init__(nombre, edad)        
    
    def saludar(self):
        print("Soy un profesor")
        
# Definición de la clase Estudiante que hereda de Persona
class Estudiante(Persona):
    def __init__(self, nombre, edad):
        super().__init__(nombre, edad)        
    
    def saludar(self):
        print("Soy un estudiante")
```

```python
# Función que usa polimorfismo
def imprimir_informacion(persona):
    persona.saludar()
```

```python
# Crear instancias de Persona y Estudiante
profesor = Profesor("María", 30)
estudiante = Estudiante("Juan", 20)

# Usar polimorfismo
imprimir_informacion(persona)     # Imprime 'Soy un profesor'
imprimir_informacion(estudiante)  # Imprime 'Soy un estudiante'
```


