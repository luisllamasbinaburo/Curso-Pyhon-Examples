> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/python-como-usar-pip/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## Verificar si pip está instalado
```bash
pip --version
```


## Instalar pip
```cmd
python get-pip.py
```

```bash
sudo apt-get install python3-pip  # Para Python 3
```


## Instalar un Paquete
```bash
pip install requests
```


## Desinstalar un Paquete
```bash
pip uninstall requests
```


## Listar Paquetes Instalados
```bash
pip list
```


## Actualizar un Paquete
```bash
pip install --upgrade requests
```


## Fichero requirements.txt
```
Flask==2.0.2
requests==2.26.0
numpy==1.21.2
```

```bash
pip install -r requirements.txt
```


