> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-diccionarios/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Creación de un diccionario
```python
mi_diccionario = {
    "clave1": valor1,
    "clave2": valor2,
    "clave3": valor3
}
```

```python
mi_diccionario = {"nombre": "Juan", "altura": 30, "profesion": "Ingeniero"}
```


## Acceso a elementos
```python
print(mi_diccionario["nombre"])  # Resultado: Juan
print(mi_diccionario["edad"])  # Resultado: 30
```


## Modificación de elementos
```python
mi_diccionario["clave1"] = nuevo_valor
mi_diccionario["nueva_clave"] = nuevo_valor
```


## Agregar elementos
```python
mi_diccionario["ciudad"] = "Madrid"  # Agrega una nueva clave-valor
```


## Verificar pertenencia de claves
```python
if "nombre" in mi_diccionario:
      print("La clave 'nombre' está presente en el diccionario.")
```


## Obtener claves y valores
```python
mi_diccionario = {"nombre": "Juan", "edad": 30, "ciudad": "Madrid"}
vista_items = mi_diccionario.items()  # Retorna una vista de los pares clave-valor
print(vista_items)  # Resultado: dict_items([('nombre', 'Juan'), ('edad', 30), ('ciudad', 'Madrid')])
```

```python
claves = mi_diccionario.keys()  # Devuelve una lista de las claves
  valores = mi_diccionario.values()  # Devuelve una lista de los valores
```


## Copia superficial del diccionario
```python
mi_diccionario = {"nombre": "Juan", "edad": 30, "ciudad": "Madrid"}
copia_diccionario = mi_diccionario.copy()  # Crea una copia superficial del diccionario

print(copia_diccionario)  # Resultado: {"nombre": "Juan", "edad": 30, "ciudad": "Madrid"}
```


## Eliminar elementos
```python
del mi_diccionario["profesion"]  # Elimina una clave y su valor
  valor_eliminado = mi_diccionario.pop("edad")  # Elimina y devuelve el valor de una clave
```


## Eliminar todos los elementos del diccionario
```python
mi_diccionario = {"nombre": "Juan", "edad": 30, "ciudad": "Madrid"}
mi_diccionario.clear()  # Elimina todos los elementos del diccionario
print(mi_diccionario)  # Resultado: {}
```


