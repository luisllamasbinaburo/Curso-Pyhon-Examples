> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-documentar-codigo-docstrings/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Sintaxis de los docstrings
```python
def nombre_de_la_funcion(parametros):
    """
    Descripción de la función

    Parámetros:
    - parametro1: descripción del parámetro
    - parametro2: descripción del parámetro

    Retorna:
    - tipo_de_retorno: descripción del tipo de retorno
    """
    # Cuerpo de la función
```


## Ejemplo de docstring
```python
def calcular_promedio(lista):
    '''
    Esta función calcula el promedio de una lista de números.

    Args:
        lista (list): Una lista de números para calcular el promedio.

    Returns:
        float: El promedio de los números en la lista.
    '''
    suma = sum(lista)
    promedio = suma / len(lista)
    return promedio
```


## aqui el resto del código del módulo
```
**Docstrings de Clases**: Describen el propósito de una clase, sus métodos y atributos.
```


## Acceso a la documentación
```python
def suma(a, b):
    """
    Devuelve la suma de a y b.
    
    Parámetros:
    a (int, float): El primer número.
    b (int, float): El segundo número.
    
    Devuelve:
    int, float: La suma de a y b.
    """
    return a + b

print(suma.__doc__)
```


