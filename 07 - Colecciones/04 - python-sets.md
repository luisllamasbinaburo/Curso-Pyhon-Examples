> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-sets/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Creación de Sets
```python
mi_set = {1, 2, 3}
```


## Crear un Set con la Función `set()`
```python
mi_otro_set = set([1, 2, 3])
```


## Agregar elementos
```python
mi_set.add(6)  # Agrega el elemento 6 al set
```


## Eliminar elementos
```python
mi_set.remove(3)  # Elimina el elemento 3 del set
mi_set.discard(2)  # Elimina el elemento 2 si está presente
```


## Unión de Sets
```python
union_set = mi_set.union(mi_otro_set)  # Une los dos sets en uno nuevo
union_set = mi_set | mi_otro_set  # Lo mismo utilizando el operador |
```


## Intersección de Sets
```python
interseccion_set = mi_set.intersection(mi_otro_set)  # Obtiene la intersección de los sets
interseccion_set = mi_set & mi_otro_set  # Lo mismo utilizando el operador &
```


## Diferencia de Sets
```python
diferencia_set = mi_set.difference(mi_otro_set)  # Obtiene la diferencia entre los sets
diferencia_set = mi_set - mi_otro_set  # Lo mismo utilizando el operador -
```


## Ejemplos prácticos
```python
lista_con_duplicados = [1, 2, 3, 4, 1, 2, 5]
  conjunto_sin_duplicados = set(lista_con_duplicados)
```

```python
if 3 in mi_set:
      print("El elemento 3 está presente en el set.")
```

```python
set1 = {1, 2, 3}
  set2 = {3, 4, 5}

  # Unión de sets
  union = set1.union(set2)  # Resultado: {1, 2, 3, 4, 5}

  # Intersección de sets
  interseccion = set1.intersection(set2)  # Resultado: {3}
  
  # Diferencia de sets
  diferencia = set1.difference(set2)  # Resultado: {1, 2}
```


