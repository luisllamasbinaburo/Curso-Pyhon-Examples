> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/tipo-float-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## tipo-float-en-python
```python
numero_float = 3.14159
```

```python
numero_cientifico = 6.022e23  # 6.022 × 10^23
```


## Operaciones con Números de Punto Flotante
```python
# Suma
suma = 3.14 + 2.71
print(suma)  # Salida: 5.85

# Resta
resta = 10.5 - 4.2
print(resta)  # Salida: 6.3

# Multiplicación
multiplicacion = 2.5 * 4.0
print(multiplicacion)  # Salida: 10.0

# División
division = 10.0 / 3.0
print(division)  # Salida: 3.3333333333333335 (precisión limitada por la representación binaria)
```

```python
import math

# Potenciación
potencia = math.pow(2.0, 3.0)
print(potencia)  # Salida: 8.0

# Seno
seno_valor = math.sin(math.pi / 2)
print(seno_valor)  # Salida: 1.0 (seno de 90 grados en radianes)
```


## Precisión y Redondeo
```python
# Suma con precisión limitada
suma_precisa = 0.1 + 0.2
print(suma_precisa)  # Salida: 0.30000000000000004 (precisión limitada)
```

```python
a = 0.1 + 0.2
b = 0.3
print(a == b)  # Salida: False (debido a la precisión limitada)
```


## Infinito y Not-a-Number (NaN)
```python
# Infinito positivo
infinito_positivo = float('inf')
print(infinito_positivo)  # Salida: inf

# Not-a-Number
nan_valor = float('nan')
print(nan_valor)  # Salida: nan
```


## Conversión entre Tipos
```python
texto = "3.14"
numero_float = float(texto)
print(numero_float)  # Salida: 3.14
```

```python
numero = 3.0
print(numero.is_integer())  # Salida: True (el número 3.0 es un entero)
```


