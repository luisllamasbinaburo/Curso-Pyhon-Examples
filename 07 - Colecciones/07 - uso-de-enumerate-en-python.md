> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/uso-de-enumerate-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Sintaxis de `enumerate()`
```python
enumerate(secuencia, inicio=0)
```


## Ejemplo básico
```python
nombres = ['Juan', 'María', 'Carlos', 'Ana']

for indice, nombre in enumerate(nombres):
    print(f"Índice {indice}: {nombre}")

# Salida:
# Índice 0: Juan
# Índice 1: María
# Índice 2: Carlos
# Índice 3: Ana
```


## Especificando un inicio para el contador
```python
nombres = ['Juan', 'María', 'Carlos', 'Ana']

for indice, nombre in enumerate(nombres, start=1):
    print(f"Estudiante {indice}: {nombre}")

# Salida:
# Estudiante 1: Juan
# Estudiante 2: María
# Estudiante 3: Carlos
# Estudiante 4: Ana
```


## Utilizando enumerate() con Otros Tipos de Datos
```python
cadena = "Python"

for indice, caracter in enumerate(cadena):
    print(f"Índice {indice}: {caracter}")

# Salida:
# Índice 0: P
# Índice 1: y
# Índice 2: t
# Índice 3: h
# Índice 4: o
# Índice 5: n
```


## Creando un Diccionario a partir de enumerate()
```python
paises = ['España', 'Francia', 'Italia']

diccionario_paises = {indice: pais for indice, pais in enumerate(paises)}
print(diccionario_paises)

# Salida: {0: 'España', 1: 'Francia', 2: 'Italia'}
```


