> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-operadores-identidad/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Operador `is`
```python
a = [1, 2, 3]
b = a

es_igual = (a is b)  # True, ya que a y b se refieren al mismo objeto
```


## Operador `is not`
```python
x = 10
y = 10

no_es_igual = (x is not y)  # False, ya que x e y se refieren al mismo objeto
```


## Verificación de identidad de variables
```python
x = 100
y = x

son_iguales = (x is y)  # True, ya que x e y son el mismo objeto en memoria
```


## Verificación de identidad de listas
```python
lista1 = [1, 2, 3]
lista2 = [1, 2, 3]
lista3 = lista1

son_iguales = (lista1 is lista2)  # False, ya que lista1 y lista2 no son el mismo objeto
son_iguales2 = (lista1 is lista3)  # True, ya que lista1 y lista3 son el mismo objeto
```


## Verificación de identidad de objetos
```python
class MiClase:
    pass

objeto1 = MiClase()
objeto2 = MiClase()
objeto3 = objeto1

son_iguales = (objeto1 is objeto2)  # False, ya que objeto1 y objeto2 no son el mismo objeto
son_iguales2 = (objeto1 is objeto3)  # True, ya que objeto1 y objeto3 son el mismo objeto
```


