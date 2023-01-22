# Colaboración en GitHub

Para poder colaborar en proyectos alojados en GitHub necesitamos hacer uso de los forks y pull requests, herramientas que nos ofrece la plataforma para dicho objetivo.

A continuación describo el proceso de colaboración en GitHub.

    Forkea el repositorio en el que quieras colaborar, para hacerlo, sigue las instrucciones de este enlace.
    Una vez forkeado el repositorio en tu cuenta de GitHub, clónalo en tu equipo de cómputo.
    En el repositorio local hay que configurar los orígenes remotos de tu nueva copía para tener ambos remotos, los originales (origin) y los de tu copia, para hacerlo, sigue las instrucciones de este enlace.
    Crea una rama nueva en tu fork local para hacer tu colaboración, y sincrónizala con tu repositorio remoto, para hacerlo, sigue las instrucciones de este enlace.
    Configura tu repositorio para que acepté cambios (pull requests), para hacerlo, sigue las instrucciones de este enlace.
    Crea una pull request, para hacerlo, sigue las instrucciones de este enlace.
    Espera a que el dueño del repositorio original, acepte tus cambios.
    Una vez que acepten tu pull request, es recomendable que borres la rama en la que trabajaste el cambio y actualices tu repositorio forkeado, con los cambios del repositorio original.

Anexo un resumen de los comandos a ejecutar para colaborar en un repositorio de GitHub:

```
# forkear repositorio
git clone https://github.com/usuario/repositorio.git
git remote -v
git remote rename origin fork
git remote add origin https://github.com/usuario/repositorio.git
git checkout -b rama-nueva
git push fork rama-nueva
# solicitar el pull request
# aceptar el pull request
git checkout main
git pull origin main
git push fork main
git branch -d rama-nueva
git push fork --delete rama-nueva
```
