# Instalacion de Git y Github

<?xml version="1.0" encoding="UTF-8" standalone="no"?><!-- Generator: Gravit.io --><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" style="isolation:isolate" viewBox="0 0 150 150" width="50pt" height="50pt"><defs><clipPath id="_clipPath_QbHlRAjcH2GtXF5FvmFIzyUBduQjtFaU"><rect width="150" height="150"/></clipPath></defs><g clip-path="url(#_clipPath_QbHlRAjcH2GtXF5FvmFIzyUBduQjtFaU)"><circle vector-effect="non-scaling-stroke" cx="75" cy="75" r="65" fill="rgb(241,78,50)"/><path d=" M 108.677 71.879 L 78.112 41.318 C 76.351 39.56 73.498 39.56 71.731 41.318 L 65.399 47.662 L 73.449 55.712 C 75.33 55.085 77.471 55.508 78.958 56.999 C 80.463 58.501 80.878 60.668 80.236 62.54 L 87.988 70.299 C 89.87 69.648 92.034 70.071 93.53 71.567 C 95.633 73.667 95.633 77.062 93.53 79.162 C 91.433 81.26 88.044 81.26 85.947 79.162 C 84.375 77.585 83.981 75.263 84.768 73.341 L 77.509 66.119 L 77.509 85.15 C 78.022 85.401 78.506 85.743 78.932 86.165 C 81.012 88.268 81.012 91.658 78.932 93.749 C 76.835 95.852 73.422 95.852 71.322 93.749 C 69.225 91.652 69.225 88.268 71.322 86.171 C 71.853 85.646 72.451 85.25 73.087 84.987 L 73.087 65.769 C 72.454 65.504 71.85 65.122 71.337 64.599 C 69.747 63.01 69.365 60.685 70.182 58.74 L 62.272 50.792 L 41.313 71.737 C 39.562 73.501 39.562 76.357 41.313 78.121 L 71.879 108.679 C 73.641 110.441 76.494 110.441 78.255 108.679 L 108.677 78.258 C 110.441 76.5 110.441 73.644 108.677 71.879 Z " fill="rgb(255,255,255)"/></g></svg>

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

Este documento también se encuentra en este repositorio con el nombre de configuracion.git
