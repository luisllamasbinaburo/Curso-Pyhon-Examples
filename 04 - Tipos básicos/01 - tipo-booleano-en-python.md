> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/tipo-booleano-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## tipo-booleano-en-python
```python
valor_verdadero = True

valor_falso = False
```


## Operador `and`
```python
resultado_and = True and False
print(resultado_and)  # Salida: False
```


## Operador `or`
```python
resultado_or = True or False
print(resultado_or)  # Salida: True
```


## Operador `not`
```python
resultado_not = not True
print(resultado_not)  # Salida: False
```


## Comparaciones y condiciones
```python
resultado = 10 > 5
print(resultado)  # Salida: True
```

```python
numero = 10
es_mayor_que_cinco = numero > 5
if es_mayor_que_cinco:
    print("El número es mayor que cinco")
else:
    print("El número no es mayor que cinco")
```


## Evaluación cortocircuitada
```python
# Evaluación cortocircuitada con `and`
resultado = False and funcion_que_no_se_evalua()

# Evaluación cortocircuitada con `or`
resultado = True or funcion_que_no_se_evalua()
```


## Conversión entre Tipos
```python
# Conversión de números
numero = 42
valor_booleano = bool(numero)
print(valor_booleano)  # Salida: True (cualquier número distinto de cero es True)

# Conversión de cadenas vacías
cadena_vacia = ""
valor_booleano = bool(cadena_vacia)
print(valor_booleano)  # Salida: False (una cadena vacía es False)
```


