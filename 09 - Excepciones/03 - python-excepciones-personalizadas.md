> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-excepciones-personalizadas/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Definición de excepciones personalizadas
```python
class MiExcepcionPersonalizada(Exception):
    def __init__(self, mensaje):
        super().__init__(mensaje)
```

```python
class ErrorDeValidacion(Exception):
    def __init__(self, campo, mensaje):
        self.campo = campo
        self.mensaje = mensaje
        super().__init__(f"Error en '{campo}': {mensaje}")

# Lanzar la excepción
raise ErrorDeValidacion("nombre", "El nombre no puede estar vacío.")
```

```python
class ErrorDeConexion(Exception):
    def __init__(self, mensaje):
        super().__init__(mensaje)

class ErrorDeTiempoDeEspera(ErrorDeConexion):
    def __init__(self, tiempo):
        self.tiempo = tiempo
        super().__init__(f"Tiempo de espera excedido: {tiempo} segundos")
```


## Usando Excepciones personalizadas
```python
try:
    raise MiExcepcionPersonalizada("Este es un error personalizado.")
except MiExcepcionPersonalizada as e:
    print(f"Se capturó mi excepción personalizada: {e}")
```

```python
try:
    # Código que puede lanzar una excepción
    resultado = 10 / 0
except MiExcepcionPersonalizada:
    print(f"Se capturó mi excepción personalizada: {e}")
except OtraExcepcionPersonalizada:
    print(f"Se capturó otra excepción personalizada: {e}")
except Exception:
    print("Excepcion desconocida")
```


