> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-ambito-de-variables/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Variables locales
```python
def mi_funcion():
    variable_local = "Hola Mundo"
    print(variable_local)

mi_funcion()
# print(variable_local)  # Esto generaría un error
```


## Variables globales
```python
variable_global = "Soy global"

def imprimir_global():
    print(variable_global)

imprimir_global()  # Resultado: Soy global
print(variable_global)  # También es accesible fuera de la función
```


## Uso de la Palabra Clave `global`
```python
variable_global = "Soy global"

def modificar_global():
    global variable_global
    variable_global = "Modificado dentro de la función"
    print(variable_global)

modificar_global()  # Resultado: Modificado dentro de la función
print(variable_global)  # Ahora la variable global ha sido modificada
```


## Alcance de Variables en Funciones Anidadas
```python
def funcion_externa():
    variable_externa = "Soy de la función externa"

    def funcion_interna():
        nonlocal variable_externa
        variable_externa = "Modificado por la función interna"
        print("Desde función interna:", variable_externa)

    funcion_interna()
    print("Desde función externa:", variable_externa)

funcion_externa()
```


