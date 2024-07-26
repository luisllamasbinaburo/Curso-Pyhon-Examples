> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/herencia-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## herencia-en-python
```python
class subclase(superclase):
   # cuerpo de subclase
```


## Ejemplo de herencia
```python
# Definición de la clase Persona
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def mostrar_informacion(self):
        print(f"Nombre: {self.nombre}, Edad: {self.edad}")
```

```python
# Definición de la clase Estudiante que hereda de Persona
class Estudiante(Persona):
    def __init__(self, nombre, edad, nota):
        super().__init__(nombre, edad)
        self.nota = nota

# Crear una instancia de Estudiante
estudiante = Estudiante("Juan", 20, "8.7")
estudiante.mostrar_informacion()   # imprime 'Nombre: Juan, Edad: 20'
```


## Sobreescritura de Métodos
```python
# Definición de la clase Estudiante que hereda de Persona
class Estudiante(Persona):
    def __init__(self, nombre, edad, nota):
        super().__init__(nombre, edad)
        self.nota = nota
    
    # Sobreescribir el método mostrar_informacion
    def mostrar_informacion(self):
        print(f"Nombre: {self.nombre}, Edad: {self.edad}, Nota: {self.nota}")

# Crear una instancia de Estudiante
estudiante = Estudiante("Juan", 20, "8.7")
estudiante.mostrar_informacion()   # imprime 'Nombre: Juan, Edad: 20, Nota: 8.7'
```


## Llamar a métodos de la super clase
```python
# Definición de la clase Estudiante que hereda de Persona
class Estudiante(Persona):
    def __init__(self, nombre, edad, nota):
        super().__init__(nombre, edad)  # Llamada al constructor de la clase base
        self.nota = nota
    
    def mostrar_informacion(self):
        super().mostrar_informacion(self)  # Llamada a un método de la clase base
        print(f"Nota: {self.nota}")

# Crear una instancia de Estudiante
estudiante = Estudiante("Juan", 20, "8.7") # imprime 'Nombre: Juan, Edad: 20, Nota: 8.7'
estudiante.mostrar_informacion()
```


## Herencia Múltiple
```python
class A:
    def metodo_a(self):
        print("Método de clase A")

class B:
    def metodo_b(self):
        print("Método de clase B")

class C(A, B):
    def metodo_c(self):
        print("Método de clase C")

# Creación de instancia de C y uso de métodos
objeto_c = C()
objeto_c.metodo_a()  # Salida: Método de clase A
objeto_c.metodo_b()  # Salida: Método de clase B
objeto_c.metodo_c()  # Salida: Método de clase C
```


