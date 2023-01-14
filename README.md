# Instalacion de Git y Github

![Instalacion Git con Homebrew](assets/img/git_logo.svg "Instalacion Git con Homebrew")

## Proceso de Configuracion de Git

## Introducción

Este documento es una guia completa para una instalacion nueva del modulo de Git; desde el gestor de paquetes, Homebrew

## Instalación

#### Download for macOS

There are several options for installing Git on macOS. Note that any non-source distributions are provided by third parties, and may not be up to date with the latest source release.
Homebrew install homebrew if you don't already have it, then:

![Instalacion Git con Homebrew](assets/img/Img01_Codigo-instalacion-Git.png "Instalacion Git con Homebrew")

## Flujo básico

El flujo de Git, consta de tres estados locales, es decir en la computadora donde se esta trabajando y uno más de forma remota cuando accedemos al codigo centralizado en plataformas como GitHub, Gitlab, Bitbucket, etc

Dichos estados son **_modified_**, **_staged_**, **_committed_** y **_remote_**

A cada uno de ellos le corresponde un área de trabajo:

### **_1. Working Directory:_** Es el área correspondiente al estado **_modified_** y es la carpeta local de tu computadora donde almacenas los archivos de tu proyecto

### **_2. Staging Area:_** Es el área correspondiente al estado **_staged_** también se le llama index por que es el área donde git indexa y agrega los cambios realizados en los archivos previos a comprometerlos en su registro

### **_3. Local Repository:_** Es el área correspondiente al estado **_committed_**, donde los cambios ya se han registrado en el repositorio de git también se le llama **_HEAD_** por que indica en qué cambio se encuentra el puntero del repositorio

### **_4. Remote Repository:_** Es el área correspondiente al estado **_remote_** y es el directorio remoto donde almacenamos los archivos del proyecto en alguna plataforma web como GitHub, GitLab, BitBucket. Git denomina **_origin_** al repositorio remoto

## Para reemplazar la rama **_master_** por **_main_** en GitHub

```
# Paso 1
# Crea la rama local main y pásale el historial de la rama master
git branch -m master main


# Paso 2
# Haz un push de la nueva rama local main en el repositorio remoto de GitHub
git push -u origin main


# Paso 3
# Cambia el HEAD actual a la rama main
git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main
```

## Paso 4

Cambia la rama default de master a main en tu repositorio de GitHub

Para hacerlo, sigue las instrucciones de este [Enlace](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/changing-the-default-branch)

```
# Paso 5
# Elimina la rama master del repositorio remoto
git push origin --delete master
```

## Para reemplazar la rama master por main en Git

```
git config --global init.defaultBranch main
```

## Ramas

Una rama nos permite aislar una nueva funcionalidad en nuestro código que después podremos añadir a la versión principal.

```
# crear rama
git branch nombre-rama

# cambiar de rama
git checkout nombre-rama

# crear una rama y cambiarte a ella
git checkout -b rama

# eliminar rama
git branch -d nombre-rama

# eliminar ramas remotas
git push origin --delete nombre-rama

#eliminar rama (forzado)
git branch -D nombre-rama

# listar todas las ramas del repositorio
git branch

# lista ramas no fusionadas a la rama actual
git branch --no-merged

# lista ramas fusionadas a la rama actual
git branch --merged

# rebasar ramas
git checkout rama-secundaria
git rebase rama-principal
```
