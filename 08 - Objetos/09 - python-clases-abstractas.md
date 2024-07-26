> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-clases-abstractas/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## python-clases-abstractas
```python
from abc import ABC, abstractmethod
```


## Definiendo una Clase Abstracta
```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def hacer_sonido(self):
        pass

    def dormir(self):
        print("El animal está durmiendo.")
```


## Implementando Clases Derivadas
```python
class Perro(Animal):
    def hacer_sonido(self):
        print("El perro ladra.")

class Gato(Animal):
    def hacer_sonido(self):
        print("El gato maúlla.")
```


## Clases mixtas
```python
class Vehiculo(ABC):
    @abstractmethod
    def conducir(self):
        pass

    def encender(self):
        print("El vehículo está encendido.")

class Coche(Vehiculo):
    def conducir(self):
        print("El coche está conduciendo.")

class Moto(Vehiculo):
    def conducir(self):
        print("La moto está conduciendo.")
```


