# Estaciones Nivel
# Por Juan Sebastian Quintero H.


**Codigo Fuente**: <a href="https://github.com/JuanseQH/LosContenedores/" target="_blank">https://github.com/JuanseQH/LosContenedores/</a>


# Acerca de

Repositorio con los artefactos de despliegue (contenedores de Docker)

Este repositorio contiene las aplicaciones/contedores usadas en el proyecto de Estaciones Nivel: 
  - Web (Ubuntu image)  https://github.com/JuanseQH/LosContenedores/web
  - Bd (mysql image)    https://github.com/JuanseQH/LosContenedores/bd
  - API (Ubuntu image)  https://github.com/JuanseQH/LosContenedores/api

<br>

# Ejecutar Estaciones Nivel



- Para acceder desde nuestro computador:
    1. Debemos de acceder al archivo web.py en VS Code.
    2. Simplemente le damos en ejecutar en una terminal y accedemos a uno de los links que nos genera. 

<br>
    
- Para acceder desde amazon AWS:
    1. Debemos de acceder a la instancia "prueba1" 
    2. luego de conectarnos a la instancia debemos de acceder a "LosContenedores" con el comando "cd Los contenedores/"
    3. Ya en "LosContenedores", debemos de editar el archivo "web.py", con el siguiente comando "sudo nano web/web.py"
    4. Una vez detro del archivo debemos de cambiar la ruta del localhost por la direccion ip publica de nuestre instancia, 
    5. una vez hecho el paso anterior debemos guardar y ya si podremos correr los contenedores con el comando " sudo docker-compose up"
    6. Ya con esto solo debemos de copiar y pegar la direccion ip publica en una ventana nueva del navegador y ingresaremos al sitio con normalidad.




<br>

# Autenticar servidor remoto a GitLab
### Clonar el repo y los subrepos

$ git config --global credential.helper cache
$ git clone --recursive git@gitlab.com:JuanseQH/abc-cloud.git
