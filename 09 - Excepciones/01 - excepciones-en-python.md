> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/excepciones-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Excepciones de Error en Tiempo de Ejecución
```python
try:
    resultado = 1 / 0
except ZeroDivisionError as e:
    print(f"Error de división por cero: {e}")
```


## Excepciones de Operaciones de Entrada/Salida
```python
try:
    with open('archivo_que_no_existe.txt', 'r') as archivo:
        contenido = archivo.read()
except FileNotFoundError as e:
    print(f"Archivo no encontrado: {e}")
```


## Excepciones de Argumentos
```python
try:
    numero = int("abc")
except ValueError as e:
    print(f"Error de valor: {e}")
```


## Excepciones de Variables y Atributos
```python
try:
    print(variable_no_definida)
except NameError as e:
    print(f"Nombre de variable no encontrado: {e}")
```


