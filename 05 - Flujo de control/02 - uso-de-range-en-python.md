> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/uso-de-range-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## uso-de-range-en-python
```python
range(inicio, fin, paso)
```


## Uso básico
```python
# Generar una secuencia de 0 a 4 (exclusivo)
for i in range(5):
    print(i)
# Salida: 0, 1, 2, 3, 4
```


## Especificando Inicio y Fin
```python
# Generar una secuencia de 2 a 8 (exclusivo)
for i in range(2, 9):
    print(i)
# Salida: 2, 3, 4, 5, 6, 7, 8
```


## Especificando Paso
```python
# Generar una secuencia de 1 a 10 con paso de 2
for i in range(1, 11, 2):
    print(i)
# Salida: 1, 3, 5, 7, 9
```


## Iterar en Orden Inverso
```python
# Iterar en orden inverso
for i in range(10, 0, -1):
    print(i)
# Salida: 10, 9, 8, 7, 6, 5, 4, 3, 2, 1
```


## Crear Lista desde `range()`
```python
# Crear una lista de números pares del 0 al 9
numeros_pares = list(range(0, 10, 2))
print(numeros_pares)
# Salida: [0, 2, 4, 6, 8]
```


## Generar Índices en un Bucle
```python
# Usar range() para generar índices en un bucle
palabra = "Python"

for i in range(len(palabra)):
    print(f"Índice {i}: {palabra[i]}")
# Salida: Índice 0: P, Índice 1: y, Índice 2: t, Índice 3: h, Índice 4: o, Índice 5: n
```


## Combinar con `zip()` para Iterar en Paralelo
```python
# Usar range() junto con zip() para iterar en paralelo sobre dos listas
nombres = ["Ana", "Juan", "María"]
edades = [30, 25, 35]

for i in range(len(nombres)):
    print(f"{nombres[i]} tiene {edades[i]} años.")
# Salida:
# Ana tiene 30 años.
# Juan tiene 25 años.
# María tiene 35 años.
```


