> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-operadores-logicos/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Operador `and`
```python
a = 5
b = 10
c = 15

resultado = (a < b) and (b < c)  # True, ya que ambas condiciones son True
```


## Operador `or`
```python
a = 5
b = 10
c = 3

resultado = (a > b) or (b < c)  # False, ya que ninguna de las condiciones es True
```


## Operador `not`
```python
verdadero = True
falso = not verdadero  # falso es False

numero = 5
es_mayor_a_10 = numero > 10
no_es_mayor_a_10 = not es_mayor_a_10
```


## Combinación con `and`
```python
edad = 25
tiene_licencia = True

puede_conducir = (edad >= 18) and tiene_licencia  # True
```


## Combinación con `or`
```python
esta_lloviendo = False
es_frio = True

quiere_quedarse_en_casa = esta_lloviendo or es_frio  # True
```


## Negación con `not`
```python
es_dia = True
es_noche = not es_dia  # False
```


## Combinación de operadores lógicos
```python
numero = 15

es_multiplo_de_3 = (numero % 3 == 0)
es_multiplo_de_5 = (numero % 5 == 0)

es_multiplo_de_3_o_5 = es_multiplo_de_3 or es_multiplo_de_5  # True, ya que 15 es múltiplo de 3
es_multiplo_de_3_y_5 = es_multiplo_de_3 and es_multiplo_de_5  # False, ya que 15 no es múltiplo de 3 y 5 simultáneamente
no_es_multiplo_de_3 = not es_multiplo_de_3  # False
```


