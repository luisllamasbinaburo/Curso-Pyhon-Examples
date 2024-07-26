> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-operadores-pertenencia/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Operador `in`
```python
frutas = ["manzana", "banana", "cereza"]

es_banana = "banana" in frutas  # True
es_uva = "uva" in frutas  # False
```


## Operador `not in`
```python
frutas = ["manzana", "banana", "cereza"]

no_es_uva = "uva" not in frutas  # True
no_es_manzana = "manzana" not in frutas  # False
```


## Verificación de elementos en una lista
```python
colores = ["rojo", "verde", "azul"]

es_azul = "azul" in colores  # True
no_es_amarillo = "amarillo" not in colores  # True
```


## Verificación de caracteres en una cadena
```python
nombre = "Juan"

tiene_a = "a" in nombre  # True
no_tiene_z = "z" not in nombre  # True
```


## Verificación de elementos en un conjunto
```python
vocales = {"a", "e", "i", "o", "u"}

es_a_vocal = "a" in vocales  # True
no_es_y = "y" not in vocales  # True
```


