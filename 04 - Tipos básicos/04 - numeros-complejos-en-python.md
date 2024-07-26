> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/numeros-complejos-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## numeros-complejos-en-python
```python
numero_complejo1 = complex(1, 2)
print(numero_complejo1)  # Salida: (1+2j)

numero_complejo2 = 3 + 4j
print(numero_complejo2)  # Salida: (3+4j)
```

```python
numero = 1 + 2j
parte_real = numero.real
parte_imaginaria = numero.imag
print(parte_real, parte_imaginaria)  # Salida: 1.0 2.0
```


## Operaciones con Números Complejos
```python
# Suma
suma = (1 + 2j) + (3 + 4j)
print(suma)  # Salida: (4+6j)

# Resta
resta = (5 + 6j) - (2 + 1j)
print(resta)  # Salida: (3+5j)

# Multiplicación
multiplicacion = (2 + 3j) * (4 + 5j)
print(multiplicacion)  # Salida: (-7+22j)

# División
division = (5 + 6j) / (2 + 1j)
print(division)  # Salida: (4+1j)
```

```python
# Conjugado
numero = 3 + 4j
conjugado = numero.conjugate()
print(conjugado)  # Salida: (3-4j)

# Magnitud
magnitud = abs(numero)
print(magnitud)  # Salida: 5.0 (raíz cuadrada de 3^2 + 4^2)

# Argumento (fase)
argumento = cmath.phase(numero)
print(argumento)  # Salida: 0.9272952180016122 (en radianes)
```


## Conversión entre Tipos
```python
# Conversión de enteros
numero_entero = 5
numero_complejo = complex(numero_entero)
print(numero_complejo)  # Salida: (5+0j)

# Conversión de flotantes
numero_float = 3.14
numero_complejo = complex(numero_float)
print(numero_complejo)  # Salida: (3.14+0j)
```


