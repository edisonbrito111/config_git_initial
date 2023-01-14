# GitHub Pages

gh-pages es una rama especial para crear un sitio web a tu proyecto alojado directamente en tu repositorio de GitHub.

1. URL del repositorio: https://github.com/usuario/repositorio
2. URL del sitio: https://usuario.github.io/repositorio

Para crear esta rama especial en GitHub ejecutamos los siguientes comandos:

```
git branch gh-pages
git checkout gh-pages

git remote add origin https://github.com/usuario/repositorio.git
git push origin gh-pages

# para descargar los cambios del repositorio remoto al local
git pull origin gh-pages
```
