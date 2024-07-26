> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-parametros-funcion/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## python-parametros-funcion
```python
def nombre_de_la_funcion(parametro1, parametro2, ...):
    # bloque de código de la función que utiliza los parámetros
```

```python
def saludar(nombre):
    print("Hola", nombre)

# Llamando a la función con un argumento
saludar("Luis")  # Salida: Hola Luis
```


## Parámetros posicionales
```python
def suma(a, b):
    resultado = a + b
    return resultado

# Llamada a la función con parámetros posicionales
resultado_suma = suma(5, 3)
print(resultado_suma)  # Salida: 8
```


## Parámetros con valores predeterminados
```python
def saludar(nombre="Mundo"):
    print("Hola,", nombre)

# Llamada a la función sin proporcionar un valor para el parámetro
saludar()  # Salida: Hola, Mundo

# Llamada a la función con un valor para el parámetro
saludar("Juan")  # Salida: Hola, Juan
```


## Parámetros con nombre
```python
def saludar(nombre, saludo="Hola"):
    print(saludo + ",", nombre)

# Llamada a la función con parámetros con nombre
saludar(nombre="Ana")  # Salida: Hola, Ana
saludar(saludo="Buenos días", nombre="Pedro")  # Salida: Buenos días, Pedro
```


## Parámetros de longitud variable
```python
def suma_numeros(*args):
    resultado = sum(args)
    return resultado

# Llamada a la función con una cantidad variable de argumentos
resultado_suma = suma_numeros(1, 2, 3, 4, 5)
print(resultado_suma)  # Salida: 15
```

```python
def imprimir_info(**kwargs):
    for clave, valor in kwargs.items():
        print(clave + ":", valor)

# Llamada a la función con argumentos con nombre
imprimir_info(nombre="Juan", edad=30, ciudad="Madrid")
# Salida:
# nombre: Juan
# edad: 30
# ciudad: Madrid
```


## Uso de `*` y `**` al llamar una Función
```python
def sumar(a, b, c):
    return a + b + c

valores = [1, 2, 3]
print(sumar(*valores))  # Resultado: 6
```

```python
diccionario = {"a": 1, "b": 2, "c": 3}
print(sumar(**diccionario))  # Resultado: 6
```


## Ejemplos
```python
# Ejemplo con un tipo básico (int)
def modificar_numero(numero):
    numero = numero * 2

numero_original = 5
modificar_numero(numero_original)
print("Número original después de llamar a la función:", numero_original)  # Resultado: 5
```

```python
# Ejemplo con una referencia (lista)
def modificar_lista(lista):
    lista.append(4)

lista_original = [1, 2, 3]
modificar_lista(lista_original)
print("Lista original después de llamar a la función:", lista_original)  # Resultado: [1, 2, 3, 4]
```


