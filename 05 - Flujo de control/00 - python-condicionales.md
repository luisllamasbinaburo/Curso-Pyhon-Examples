> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-condicionales/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Sentencia `if`
```python
if condicion:
    # bloque de código si la condición es verdadera
```

```python
numero = 15

if numero > 10:
    print("El número es mayor que 10")
```


## Sentencia `else`
```python
if condicion:
    # bloque de código si la condición es verdadera
else:
    # bloque de código si la condición es falsa
```

```python
numero = 5

if numero > 10:
    print("El número es mayor que 10")
else:
    print("El número es menor o igual a 10")
```


## Sentencia `elif`
```python
if condicion_1:
    # bloque de código si la condicion_1 es verdadera
elif condicion_2:
    # bloque de código si la condicion_1 es falsa y la condicion_2 es verdadera
else:
    # bloque de código si todas las condiciones anteriores son falsas
```

```python
numero = 5

if numero > 0:
    print("El número es positivo")
elif numero < 0:
    print("El número es negativo")
else:
    print("El número es cero")
```


## Condiciones múltiples
```python
x = 10
y = 5
z = 0

if x > y and y > z:
    print("Todas las condiciones son verdaderas")
```


