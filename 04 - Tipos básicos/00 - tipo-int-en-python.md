> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/tipo-int-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## tipo-int-en-python
```python
numero_entero = 42

numero_negativo = -10
```


## Operaciones con Enteros
```python
# Suma
suma = 10 + 5
print(suma)  # Salida: 15

# Resta
resta = 10 - 5
print(resta)  # Salida: 5

# Multiplicación
multiplicacion = 10 * 5
print(multiplicacion)  # Salida: 50

# División
division = 10 / 5
print(division)  # Salida: 2.0 (resultado siempre es un float en Python 3)
```


## División Entera y Módulo
```python
# División entera
division_entera = 10 // 3
print(division_entera)  # Salida: 3

# Módulo
modulo = 10 % 3
print(modulo)  # Salida: 1 (el resto de la división 10 / 3 es 1)
```


## Potenciación
```python
# Potencia
potencia = 2 ** 3
print(potencia)  # Salida: 8 (2 elevado a la 3)
```


## Desbordamiento de Enteros
```python
import sys

numero_grande = sys.maxsize + 1
print(numero_grande)  # Salida: 9223372036854775808 (entero muy grande)
```


## Precisiones con Punto Flotante
```python
resultado = 10 / 5
print(resultado)  # Salida: 2.0 (float)
```


## Representación Binaria, Octal y Hexadecimal
```python
# Binario
binario = 0b1010  # Representa el número 10 en binario
print(binario)  # Salida: 10

# Octal
octal = 0o52  # Representa el número 42 en octal
print(octal)  # Salida: 42

# Hexadecimal
hexadecimal = 0x2A  # Representa el número 42 en hexadecimal
print(hexadecimal)  # Salida: 42
```


## Conversión entre Tipos
```python
texto = "42"
numero = int(texto)  # Convierte el texto "42" a un entero 42
print(numero)  # Salida: 42
```


## Funciones y métodos útiles
```python
# Ejemplo de uso de funciones incorporadas
valor_absoluto = abs(-10)
print(valor_absoluto)  # Salida: 10
```


