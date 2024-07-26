> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/que-son-modulos-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Creando un módulo
```python
# operaciones.py

def suma(a, b):
    return a + b

def resta(a, b):
    return a - b

def multiplicacion(a, b):
    return a * b

def division(a, b):
    if b != 0:
        return a / b
    else:
        return "Error: División por cero"
```


## Importando un Módulo Completo
```python
import operaciones

resultado_suma = operaciones.suma(5, 3)
print("Resultado de la suma:", resultado_suma)

resultado_resta = operaciones.resta(10, 4)
print("Resultado de la resta:", resultado_resta)
```


## Importando funciones específicas de un módulo
```python
from operaciones import multiplicacion, division

resultado_multiplicacion = multiplicacion(6, 2)
print("Resultado de la multiplicación:", resultado_multiplicacion)

resultado_division = division(15, 3)
print("Resultado de la división:", resultado_division)
```


## Alias en la Importación
```python
import operaciones as ops

resultado_suma = ops.suma(5, 3)
print("Resultado de la suma:", resultado_suma)

from operaciones import resta as restar

resultado_resta = restar(10, 4)
print("Resultado de la resta:", resultado_resta)
```


## Ejemplo básico
```python
# main.py

import operaciones as ops

resultado_suma = ops.suma(5, 3)
print("Resultado de la suma:", resultado_suma)

resultado_resta = ops.resta(10, 4)
print("Resultado de la resta:", resultado_resta)
```


