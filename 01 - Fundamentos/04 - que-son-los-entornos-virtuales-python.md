> Códigos de ejemplo de los tutoriales de www.luisllamas.es
>
> Enlace entrada: https://www.luisllamas.es/que-son-los-entornos-virtuales-python/
>
> Todo el contenido distribuido bajo licencia CCC, salvo indicación expresa

## ¿Qué es un entorno virtual? 
```
Entorno Virtual
├── Include
├── Libs
│   └── site-packages
└── Scripts
```


## Creación de un Entorno Virtual
```bash
mkdir mi_proyecto
cd mi_proyecto
```

```cmd
python -m venv mi_env
```

```bash
python3 -m venv mi_env
```


## Activación del Entorno Virtual
```cmd
mi_env\Scripts\activate
```

```bash
source mi_env/bin/activate
```

```
(mi_env) C:\ruta_a_mi_proyecto\mi_env >
```


## Desactivación del Entorno Virtual
```bash
deactivate
```


## Instalación de Paquetes en el Entorno Virtual
```bash
pip install requests
```


