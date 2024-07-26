> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-retorno-funcion/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## `return` en Python
```python
def nombre_de_la_funcion(parametros):
    # bloque de código de la función
    return valor_a_devolver
```


## Devolver un valor simple
```python
def suma(a, b):
    resultado = a + b
    return resultado

# Llamada a la función y asignación del valor devuelto a una variable
resultado_suma = suma(5, 3)
print(resultado_suma)  # Salida: 8
```


## Devolver `None`
```python
def funcion_vacia():
    pass

resultado = funcion_vacia()
print(resultado)  # Salida: None
```


## Devolver múltiples valores
```python
def tupla_colores():
    return ("rojo", "verde", "azul")

colores = tupla_colores()
print(colores)  # Salida: ('rojo', 'verde', 'azul')
```


## Salida anticipada de una función
```python
def verificar_numero_negativo(numero):
    if numero < 0:
        return "El número es negativo"
    else:
        return "El número es positivo o cero"

# Llamada a la función con diferentes valores
print(verificar_numero_negativo(-5))  # Salida: El número es negativo
print(verificar_numero_negativo(10))  # Salida: El número es positivo o cero
```


