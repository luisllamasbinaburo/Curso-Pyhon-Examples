> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-tipos-valor-referencia/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Tipos de Valor
```python
# Asignación de un entero a una variable
x = 10
# Se crea una nueva copia del valor 10 en la memoria para la variable x
y = x
# Ahora x e y tienen valores independientes en la memoria
```


## Tipos de referencia
```python
# Asignación de una lista a una variable
lista1 = [1, 2, 3]
# lista2 apunta al mismo objeto en la memoria que lista1
lista2 = lista1
# Modificar lista2 también modifica lista1
lista2.append(4)
print("lista1:", lista1)  # Resultado: [1, 2, 3, 4]
```


## Pasando tipos de valor
```python
def duplicar_numero(num):
    num *= 2
    print("Dentro de la función:", num)

x = 10
duplicar_numero(x)
print("Fuera de la función:", x)  # x sigue siendo 10, no se modificó
```


## Pasando tipos de referencia
```python
def modificar_lista(lista):
    lista.append("Nuevo elemento")
    print("Dentro de la función:", lista)

mi_lista = [1, 2, 3]
modificar_lista(mi_lista)
print("Fuera de la función:", mi_lista)  # mi_lista se modifica
```


