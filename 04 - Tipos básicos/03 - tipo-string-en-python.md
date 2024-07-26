> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/tipo-string-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## tipo-string-en-python
```python
cadena_simple = 'Hola, mundo!'
cadena_doble = "¡Hola, mundo!"
cadena_triple = """Este es un ejemplo
de una cadena con múltiples líneas."""
```


## Caracteres Especiales
```python
cadena_con_salto = "Primera línea\nSegunda línea"
print(cadena_con_salto)
# Salida:
# Primera línea
# Segunda línea
```


## Concatenación de Cadenas
```python
cadena1 = "Hola"
cadena2 = " mundo"
cadena_concatenada = cadena1 + cadena2
print(cadena_concatenada)  # Salida: "Hola mundo"
```


## Indexación y Segmentación
```python
mensaje = "Hola mundo"
primer_caracter = mensaje[0]
subcadena = mensaje[1:5]  # Desde el índice 1 hasta el 5 (no inclusivo)
print(primer_caracter)  # Salida: "H"
print(subcadena)  # Salida: "ola "
```


## Métodos de Formateo
```python
nombre = "Juan"
edad = 30
mensaje = "Hola, mi nombre es {} y tengo {} años.".format(nombre, edad)
print(mensaje)  # Salida: "Hola, mi nombre es Juan y tengo 30 años."

# F-string (Python 3.6+)
mensaje_fstring = f"Hola, mi nombre es {nombre} y tengo {edad} años."
print(mensaje_fstring)  # Salida: "Hola, mi nombre es Juan y tengo 30 años."
```


## Métodos de verificación
```python
cadena = "Python es genial"
print(cadena.startswith("Py"))  # Salida: True
print(cadena.endswith("al"))  # Salida: True
print(cadena.isalpha())  # Salida: False (porque hay espacios y no solo letras)
```


## Métodos de manipulación
```python
texto = "   Hola, mundo!   "
texto_mayusculas = texto.upper()
texto_sin_espacios = texto.strip()
print(texto_mayusculas)  # Salida: "   HOLA, MUNDO!   "
print(texto_sin_espacios)  # Salida: "Hola, mundo!"
```


## Métodos de transformación
```python
texto = "Hola, cómo estás?"
palabras = texto.split(", ")
print(palabras)  # Salida: ['Hola', 'cómo estás?']

lista = ['Hola', 'cómo', 'estás?']
texto_unido = ' '.join(lista)
print(texto_unido)  # Salida: "Hola cómo estás?"
```


