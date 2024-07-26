> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/decoradores-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Definir un decorador
```python
def mi_decorador(func):
    def wrapper():
        print("Algo se hace antes de la función")
        func()
        print("Algo se hace después de la función")
    return wrapper
```


## Usando un decorador
```python
@mi_decorador
def saludar():
    print("¡Hola desde LuisLlamas.es!")

saludar()

# Salida:
# Algo se hace antes de la función
# ¡Hola desde LuisLlamas.es!
# Algo se hace después de la función
```


## Decoradores con argumentos
```python
def repetir(n):
    def decorador(func):
        def envoltura(*args, **kwargs):
            for _ in range(n):
                func(*args, **kwargs)
        return envoltura
    return decorador

@repetir(3)
def decir_adios():
    print("Adiós!")

decir_adios()

# Salida:
# Adiós!
# Adiós!
# Adiós!
```


## Decoradores en múltiples niveles
```python
def decorador1(func):
    def envoltura():
        print("Decorador 1 antes")
        func()
        print("Decorador 1 después")
    return envoltura

def decorador2(func):
    def envoltura():
        print("Decorador 2 antes")
        func()
        print("Decorador 2 después")
    return envoltura

@decorador1
@decorador2
def funcion():
    print("Función ejecutándose")

funcion()

# Salida:
# Decorador 1 antes
# Decorador 2 antes
# Función ejecutándose
# Decorador 2 después
# Decorador 1 después
```


