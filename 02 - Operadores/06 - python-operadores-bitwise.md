> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-operadores-bitwise/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Ejemplo
```python
# Ejemplo de operador AND
a = 10  # 1010 en binario
b = 3   # 0011 en binario
resultado = a & b
print(resultado)  # Salida: 2
# Explicación: 1010 & 0011 = 0010 (decimal 2)
```


## Ejemplo
```python
# Ejemplo de operador OR
a = 10  # 1010 en binario
b = 3   # 0011 en binario
resultado = a | b
print(resultado)  # Salida: 11
# Explicación: 1010 | 0011 = 1011 (decimal 11)
```


## Ejemplo
```python
# Ejemplo de operador XOR
a = 10  # 1010 en binario
b = 3   # 0011 en binario
resultado = a ^ b
print(resultado)  # Salida: 9
# Explicación: 1010 ^ 0011 = 1001 (decimal 9)
```


## Operadores de Desplazamiento
```python
# Ejemplo de desplazamiento izquierda
a = 5   # 101 en binario
resultado = a << 2
print(resultado)  # Salida: 20
# Explicación: 101 << 2 = 10100 (decimal 20)
```

```python
# Ejemplo de desplazamiento derecha
a = 20   # 10100 en binario
resultado = a >> 2
print(resultado)  # Salida: 5
# Explicación: 10100 >> 2 = 101 (decimal 5)
```


## Operador de Complemento (~)
```python
# Ejemplo de operador de complemento
a = 5   # 101 en binario
resultado = ~a
print(resultado)  # Salida: -6
# Explicación: ~101 = -110 (en complemento a dos, -6 en decimal)
```


