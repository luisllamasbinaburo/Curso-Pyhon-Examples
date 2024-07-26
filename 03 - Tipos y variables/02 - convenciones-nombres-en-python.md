> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/reglas-para-nombrar-variables-en-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Reglas Específicas
```python
variable = 42
  _variable_privada = "Python"
  1variable = "Error"  # Incorrecto, no debe comenzar con un número
```

```python
mi_variable = "Python"
  edad3 = 30
  mi_variable@ = "Error"  # Incorrecto, no se permite el símbolo @
```

```python
if = 10  # Incorrecto, if es una palabra reservada
  mi_if = 10  # Correcto, añadiendo prefijo o sufijo a la palabra reservada
```

```python
total_compras = 100
  num = 100  # Menos descriptivo, se desconoce el propósito
```


## Convenciones de Estilo
```python
# Ejemplos de snake_case
nombre_completo = "Juan Pérez"
calcular_total = lambda x, y: x + y

# Ejemplos de CamelCase (para nombres de clases)
class MiClase:
    def __init__(self):
        self.atributo = None
```


