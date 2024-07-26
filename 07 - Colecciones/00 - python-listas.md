> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-listas/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Crear una Lista con Corchetes `[]`
```python
mi_lista = [1, 2, 3, 4, 5]
```


## Crear una lista vacía
```python
lista_vacia = []
```


## Acceso a elementos de una Lista
```python
mi_lista = [10, 20, 30, 40, 50]

print(mi_lista[0])  # Resultado: 10
print(mi_lista[2])  # Resultado: 30
```


## Agregar Elementos
```python
mi_lista.append(60)  # Agrega 60 al final de la lista
mi_lista.insert(2, 25)  # Inserta 25 en la posición 2
```


## Concatenar listas
```python
lista1 = [1, 2, 3]
lista2 = [4, 5, 6]

lista_concatenada = lista1 + lista2  # lista_concatenada es [1, 2, 3, 4, 5, 6]
lista_repetida = lista1 * 3  # lista_repetida es [1, 2, 3, 1, 2, 3, 1, 2, 3]
```


## Eliminar Elementos
```python
mi_lista.remove(20)  # Elimina el valor 20 de la lista
mi_lista.pop(3)  # Elimina y devuelve el elemento en la posición 3
del mi_lista[1]  # Elimina el elemento en la posición 1
```


## Ordenar
```python
mi_lista.sort()  # Ordena la lista en orden ascendente
mi_lista_sorted = sorted(mi_lista)  # Crea una nueva lista ordenada
```


## Longitud
```python
longitud = len(mi_lista)  # Devuelve la longitud de la lista
```


## Listas Anidadas
```python
lista_anidada = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

print(lista_anidada[0][1])  # Resultado: 2
```


