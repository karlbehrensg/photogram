<div align="center">
  <h1>Guía para proyectos en Django</h1>
</div>

## Configuración de entorno de trabajo
Primero debemos tener instalado Python. Luego de la instalacion abrimos la terminal y nos posicionamos en la ruta que deseamos establecer nuestro proyecto.

## Creacion de entorno virtual con Python
Vamos a crear un entorno virtual para nuestro proyecto, el cual contendra todas las dependencias. Es muy importante que este entorno este fuera de nuestro proyecto. Para crearlo ejecutamos:
```
python -m venv .env
```
Nota: .env sera el nombre de nuestro entorno.

## Comandos del entorno

Para **activar** nuestro entorno ejecutamos
```
source .env/bin/activate
```
Y para **desactivarlo**
```
deactivate
```
Si queremos **listar las librerias instaladas** usamos
```
pip freeze
```
## Instalación de Django
Para **instalar** la ultima version de Django ejecutamos
```
pip install django -U
```
## Django Admin
Es una interfaz instalada junto con Django que contiene subcomandos que utiles. Para listar los subcomandos utilizamos
```
django-admin
```
## Creacion de proyecto
Para **crear** un proyecto ejecutamos
```
django-admin startproject name
```
## Exploracion de los archivos
Lo primero que veremos es un folder con el nombre de nuestro proyecto, el cual contiene los archivos:

- **\_\_init_\_.py:** la unica finalidad de este archivo es declarar nuestra carpeta como un modulo de python.
- **settings.py:** es el mas importante, define todas las configuraciones de nuestro proyecto.
- **urls.py:** es el archivo de punto de entrada para todas las peticiones a nuestro proyecto.
- **wsgi.py:** es usado para el deployment a produccion y es la interfaz WSGI cuando el servidor corre en producción.
- **manage.py:** es un archivo que no tocamos, pero interactuamos con el durante todo el desarrollo.