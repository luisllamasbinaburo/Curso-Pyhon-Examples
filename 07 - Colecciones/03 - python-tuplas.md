> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-tuplas/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Creación de una tupla
```python
mi_tupla = (1, 2, 3, 4, 5)
```

```python
mi_otra_tupla = tuple([1, 2, 3])
```


## Acceso a Elementos de una Tupla
```python
mi_tupla = (10, 20, 30, 40, 50)
print(mi_tupla[0])  # Resultado: 10
print(mi_tupla[2])  # Resultado: 30
```


## Desempaquetado de Tuplas
```python
mi_tupla = ("Juan", "Perez", 30)
nombre, apellido, edad = mi_tupla
print(nombre)  # Resultado: Juan
print(apellido)  # Resultado: Perez
print(edad)  # Resultado: 30
```


## Ejemplos prácticos
```python
def obtener_datos_persona():
      nombre = "Juan"
      edad = 30
      return nombre, edad

  datos = obtener_datos_persona()
  nombre, edad = datos
```

```python
persona1 = ("Juan", 30)
  persona2 = ("Ana", 25)

  diccionario_personas = {persona1: "Programador", persona2: "Diseñador"}
```

```python
mi_tupla = (10, 20, 30)
  for numero in mi_tupla:
      print(numero)
```


