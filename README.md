# Sprint 1: Preparacion

 1-Primero lo que haremos sera hacer un fork del repo 
 2-Lo clonaremos con el comendo de git clone
 3-Abriremos el navegador y veremos si tenemos cuenta si no la iniciaremos
 4-Ejecutamos el siguiente comando para verificar si estás autenticado en Docker Hub:
 docker info
 Buscamos en la salida una línea similar a:
 Username: <tu_usuario>
 Si aparece nuestro nombre de usuario de Docker Hub, significa que tenemos una sesión activa.
 

 # Sprint 2: Apache 

  # Servidor Apache con Docker

En este proyecto creamos un servidor web Apache que sirve un archivo `index.html` con el mensaje "Hola Mundo".

## Pasos

### 1. Crear la estructura de directorios y archivos
Primero, creamos la carpeta llamada `apache` y dentro de ella creamos un archivo `Dockerfile` y un archivo `index.html` con el siguiente contenido:

#### Dockerfile
```dockerfile
# Usamos la imagen oficial de Apache
FROM httpd:2.4

# Copiamos el archivo index.html al directorio adecuado de Apache
COPY index.html /usr/local/apache2/htdocs/

# Exponemos el puerto 80
EXPOSE 80

  



