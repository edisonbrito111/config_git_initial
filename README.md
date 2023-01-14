# Instalacion de Git y Github

![Instalacion Git con Homebrew](assets/img/git_logo.svg "Instalacion Git con Homebrew")

## Proceso de Configuracion de Git

### Introducción

Este documento es una guia completa para una instalacion nueva del modulo de Git; desde el gestor de paquetes, Homebrew.

### Indice

<!-- <ul>
<li><a href="#instalacion">Instalación</a>
</li>
</ul> -->

[Instalación][1], [Configuración inicial][2], [Enlace 3][3]

[1]: http:///README.md/Instalación "Instalación"
[2]: http://../README.md "Configuración inicial"
[3]: http://joedicastro.com/

#### Instalación

##### Download for macOS

There are several options for installing Git on macOS. Note that any non-source distributions are provided by third parties, and may not be up to date with the latest source release.
Homebrew

Install homebrew if you don't already have it, then:

![Instalacion Git con Homebrew](assets/img/Img01_Codigo-instalacion-Git.png "Instalacion Git con Homebrew")

## Configuracion inicial

### Configurando Git por primera vez

```
git config --global user.name “Edison Brito”
git config --global user.email edisonbrito1@gmail.com
git config --global user.ui true
git config --global init.defaultBranch main
```

### Inicializar Git en un directorio local

```
mkdir carpeta
cd carpeta
touch README.md
touch .gitignore
git init
code .
```

## Flujo básico

El flujo de Git, consta de tres estados locales, es decir en la computadora donde se esta trabajando y uno más de forma remota cuando accedemos al codigo centralizado en plataformas como GitHub, Gitlab, Bitbucket, etc.

Dichos estados son **_modified_**, **_staged_**, **_committed_** y **_remote_**.

A cada uno de ellos le corresponde un área de trabajo:

### **_1. Working Directory:_** Es el área correspondiente al estado **_modified_** y es la carpeta local de tu computadora donde almacenas los archivos de tu proyecto

### **_2. Staging Area:_** Es el área correspondiente al estado **_staged_** también se le llama index por que es el área donde git indexa y agrega los cambios realizados en los archivos previos a comprometerlos en su registro

### **_3. Local Repository:_** Es el área correspondiente al estado **_committed_**, donde los cambios ya se han registrado en el repositorio de git también se le llama **_HEAD_** por que indica en qué cambio se encuentra el puntero del repositorio

### **_4. Remote Repository:_** Es el área correspondiente al estado **_remote_** y es el directorio remoto donde almacenamos los archivos del proyecto en alguna plataforma web como GitHub, GitLab, BitBucket. Git denomina **_origin_** al repositorio remoto

![](assets/img/git-flow.png "titulo")
