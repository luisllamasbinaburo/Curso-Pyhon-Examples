> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-modificadores-acceso/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Acceso público
```python
class Persona:
    def __init__(self, nombre):
        self.nombre = nombre  # Atributo público

    def saludar(self):
        return f"Hola, soy {self.nombre}"  # Método público

# Uso de la clase Persona
persona = Persona("Juan")
print(persona.saludar())  # Salida: Hola, soy Juan
```


## Acceso protegido
```python
class CuentaBancaria:
    def __init__(self, saldo):
        self._saldo = saldo  # Atributo protegido

    def mostrar_saldo(self):
        return f"Saldo disponible: {self._saldo}"  # Método protegido

# Uso de la clase CuentaBancaria
cuenta = CuentaBancaria(5000)
print(cuenta.mostrar_saldo())  # Salida: Saldo disponible: 5000
print(cuenta._saldo)  # Acceso protegido (no recomendado pero posible)
```


## Acceso privado
```python
class Estudiante:
    def __init__(self, nombre):
        self.__nombre = nombre  # Atributo privado

    def __presentarse(self):
        return f"¡Hola! Soy {self.__nombre}"  # Método privado

# Uso de la clase Estudiante
estudiante = Estudiante("María")
# print(estudiante.__nombre)  # Error: AttributeError (no se puede acceder directamente)
# estudiante.__presentarse()  # Error: AttributeError (no se puede llamar directamente)
```


