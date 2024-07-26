> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-try-except/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## El bloque Try-Except
```python
try:
    # Código que puede lanzar una excepción
    
except:
    # Código a ejecutar si se produce una excepción
```

```python
try:
    # Código que puede lanzar una excepción
    resultado = 10 / 0
except:
    # Código a ejecutar si se produce una excepción
    print("Se produjo una excepción.")
```


## Captura de multiples Excepciones
```python
try:
    # Código que puede lanzar una excepción
    resultado = 10 / 0
except ZeroDivisionError:
    # Código a ejecutar si se produce una excepción del tipo ZeroDivisionError
    print("No se puede dividir por cero.")
except ValueError:
    # Código a ejecutar si se produce una excepción del tipo ValueError
    print("Valor incorrecto.")
except:
    # Código a ejecutar si se produce cualquier tipo de excepción
    print("Se produjo una excepción.")
```


## Bloque `else`
```python
try:
    # Código que puede lanzar una excepción
    resultado = 10 / 2
except ZeroDivisionError:
    # Código a ejecutar si se produce una excepción del tipo ZeroDivisionError
    print("No se puede dividir por cero.")
else:
    # Código a ejecutar si no se produce ninguna excepción
    print("La división fue exitosa. El resultado es:", resultado)
finally:
    # Código a ejecutar siempre, independientemente de si se produce una excepción o no
    print("Esta línea se ejecutará siempre.")
```


## Bloque `finally`
```python
try:
    # Código que puede lanzar una excepción
    resultado = 10 / 0
except ZeroDivisionError:
    # Código a ejecutar si se produce una excepción del tipo ZeroDivisionError
    print("No se puede dividir por cero.")
finally:
    # Código a ejecutar siempre, independientemente de si se produce una excepción o no
    print("Esta línea se ejecutará siempre.")
```


## Contexto del Manejador de Excepciones
```python
try:
    archivo = open('archivo.txt', 'r')
    contenido = archivo.read()
except FileNotFoundError:
    print("El archivo no se encontró.")
except IOError:
    print("Error al leer el archivo.")
else:
    print("El archivo se leyó correctamente. Contenido:")
    print(contenido)
finally:
    if 'archivo' in locals() and not archivo.closed:
        archivo.close()
        print("El archivo ha sido cerrado.")
```


