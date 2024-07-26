> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-bucles/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Bucle `for`
```python
for elemento in secuencia:
    # bloque de código a ejecutar para cada elemento
```


## Ejemplos bucle for
```python
frutas = ["manzana", "banana", "cereza"]

for fruta in frutas:
    print(fruta)
```

```
manzana
banana
cereza
```

```python
# Ejemplo de bucle for con range(5)
for i in range(5):
    print(i)
```

```
0
1
2
3
4
```

```python
# Ejemplo de bucle for con una cadena de texto
for letra in "Python":
    print(letra)
```

```
P
y
t
h
o
n
```


## Bucle `while`
```python
while condicion:
    # bloque de código a ejecutar mientras la condición sea verdadera
```


## Ejemplos bucle while
```python
contador = 1

while contador <= 5:
    print(contador)
    contador += 1
```

```
1
2
3
4
5
```


## Break
```python
frutas = ["manzana", "banana", "cereza", "sandía", "uva"]

for fruta in frutas:
    print(fruta)
    if fruta == "sandía":
        break
```


## Continue
```python
numeros = [1, 2, 3, 4, 5]

for numero in numeros:
    if numero % 2 == 0:
        continue
    print(numero)
```


## Bucles con `else`
```python
numeros = [1, 2, 3, 4, 5]

for numero in numeros:
    if numero == 0:
        break
else:
    print("El bucle ha terminado sin encontrar el número 0")
```


