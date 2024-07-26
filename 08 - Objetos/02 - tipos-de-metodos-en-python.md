> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/tipos-de-metodos-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Métodos de Instancia
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        return f"Hola, soy {self.nombre} y tengo {self.edad} años."

# Creación de instancia de Persona
persona1 = Persona("Juan", 30)

# Llamada al método de instancia
print(persona1.saludar())  # Salida: Hola, soy Juan y tengo 30 años.
```


## Métodos de Clase
```python
class Coche:
    descuento = 0.1  # Descuento del 10% para todos los coches

    def __init__(self, marca, modelo, precio):
        self.marca = marca
        self.modelo = modelo
        self.precio = precio

    @classmethod
    def aplica_descuento(cls, precio):
        return precio * (1 - cls.descuento)

# Uso del método de clase
precio_final = Coche.aplica_descuento(30000)
print(f"Precio final con descuento: ${precio_final}")  # Salida: Precio final con descuento: $27000.0
```


## Métodos Estáticos
```python
class Utilidades:
    @staticmethod
    def sumar(a, b):
        return a + b

# Uso del método estático
resultado = Utilidades.sumar(3, 5)
print(f"Resultado de la suma: {resultado}")  # Salida: Resultado de la suma: 8
```


