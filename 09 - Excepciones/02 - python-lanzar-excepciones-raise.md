> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-lanzar-excepciones-raise/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Sintaxis básica
```python
raise ExceptionType("Mensaje de error")
```


## Ejemplo de Uso Básico
```python
def verificar_edad(edad):
    if edad < 0:
        raise ValueError("La edad no puede ser negativa.")
    print("Edad válida.")

try:
    verificar_edad(-5)
except ValueError as e:
    print(f"Se produjo un error: {e}")
```


## Volver a Lanzar Excepciones
```python
def procesar_datos(dato):
    try:
        if not isinstance(dato, int):
            raise TypeError("Se esperaba un entero.")
        print(f"Procesando {dato}")
    except TypeError as e:
        print(f"Error detectado: {e}")
        raise  # Vuelve a lanzar la excepción para que pueda ser manejada más arriba

try:
    procesar_datos("texto")
except TypeError as e:
    print(f"Excepción manejada en el nivel superior: {e}")
```


