> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-slices/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## python-slices
```python
secuencia[inicio:fin:paso]
```


## Omisión de valores valores
```python
primeros_salvo_tres = numeros[3:]  # Extrae los elementos del 3 al final
primeros_tres = numeros[:3]  # Extrae los tres primeros elementos
```


## Uso de índices negativos
```python
ultimos_tres = numeros[-3:]  # Extrae los últimos tres elementos
primeros_salvo_tres = numeros[:-3]  # Extrae los elementos, salvo los tres últimos
```


## Modificación de valores con Slices
```python
frutas = ["manzana", "banana", "cereza", "dátil", "uva"]

frutas[1:3] = ["pera", "naranja"]  # Reemplaza "banana" y "cereza" por "pera" y "naranja"
```


## Ejemplos prácticos
```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```


## Sin especificar inicio, fin ni paso
```python
resultado = numeros[:]
print(resultado)  # Resultado: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```


## Especificando inicio y fin
```python
resultado = numeros[2:7]
print(resultado)  # Resultado: [2, 3, 4, 5, 6]
```


## Especificando solo fin
```python
resultado = numeros[:5]
print(resultado)  # Resultado: [0, 1, 2, 3, 4]
```


## Especificando solo inicio
```python
resultado = numeros[3:]
print(resultado)  # Resultado: [3, 4, 5, 6, 7, 8, 9]
```


## Especificando solo paso
```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

numeros_pares = numeros[::2]  # Resultado: [0, 2, 4, 6, 8]
```


## Especificando todo
```python
resultado = numeros[1:8:2]
print(resultado)  # Resultado: [1, 3, 5, 7]
```


## Índices negativos al principio
```python
ultimos_tres = numeros[-3:]  # Extrae los últimos tres elementos: [7, 8, 9]
```


## Índices negativos al final
```python
sin_ultimos_tres = numeros[:-3]  # Extrae todos los elementos excepto los últimos tres: [0, 1, 2, 3, 4, 5, 6]
```


## Paso negativo
```python
invertido = numeros[::-1]  # Invierte el orden de la lista: [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```


