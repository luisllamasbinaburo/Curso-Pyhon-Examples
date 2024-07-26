> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/with-statements-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Introducción a `with`
```python
with expresión as variable:
    # Código que usa la variable
```


## Ejemplo Básico
```python
# Usando with para manejar un archivo
with open('archivo.txt', 'r') as archivo:
    contenido = archivo.read()
    print(contenido)
# El archivo se cierra automáticamente al salir del bloque with
```


## Creación de un Context Manager con Clases
```python
class MiContexto:
    def __enter__(self):
        print("Entrando en el contexto")
        return self

    def __exit__(self, exc_type, exc_value, traceback):
        print("Saliendo del contexto")
        # Puedes manejar excepciones aquí si es necesario
        return False

# Usando el contexto personalizado
with MiContexto() as contexto:
    print("Dentro del bloque with")
    
# Salida:
# Entrando en el contexto
# Dentro del bloque with
# Saliendo del contexto
```


## Creación de un Context Manager con Generadores
```python
from contextlib import contextmanager

@contextmanager
def mi_contexto():
    print("Entrando al contexto")
    yield
    print("Saliendo del contexto")

with mi_contexto():
    print("Dentro del bloque with")

# Salida:
# Entrando en el contexto
# Dentro del bloque with
# Saliendo del contexto
```


