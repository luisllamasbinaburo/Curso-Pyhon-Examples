> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-corrutinas/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Definición de una corrutina
```python
# Ejemplo básico de una corrutina
import asyncio

async def mi_corrutina():
    print("Comenzando la corrutina")
    await asyncio.sleep(1)
    print("Corrutina finalizada")
```


## Ejecución de corrutinas
```python
import asyncio

async def saludar():
    print("Hola mundo")
    await asyncio.sleep(1)
    print("Desde LuisLlamas")

asyncio.run(saludar())

# salida:
# hola mundo
# ...(espera de un segundo)...
# Desde LuisLlamas
```


## Esperar a múltiples corrutinas
```python
import asyncio

async def tarea(numero):
    print(f"Comenzando tarea {numero}")
    await asyncio.sleep(1)
    print(f"Terminando tarea {numero}")

async def main():
    await asyncio.gather(tarea(1), tarea(2), tarea(3))

asyncio.run(main())
```


## Programación Asíncrona
```python
import asyncio
import aiohttp

async def fetch_url(url):
    async with aiohttp.ClientSession() as session:
        async with session.get(url) as response:
            return await response.text()

async def main():
    html = await fetch_url('http://www.google.com')
    print(html)

asyncio.run(main())
```


## Pipelines de Procesamiento
```python
import asyncio

async def productor(queue):
    for i in range(5):
        await queue.put(i)
        await asyncio.sleep(1)

async def consumidor(queue):
    while True:
        item = await queue.get()
        if item is None:
            break
        print(f"Consumiendo {item}")
        await asyncio.sleep(2)

async def main():
    queue = asyncio.Queue()
    await asyncio.gather(productor(queue), consumidor(queue))

asyncio.run(main())
```


