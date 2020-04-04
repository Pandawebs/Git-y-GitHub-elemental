# Clonar un repositorio

Otra común manera de comenzar a trabajar con un repositorio es clonando uno existente. Esto crea una copia del repositorio en nuestra computadora. No necesitamos ni crear carpeta ni ejecutar `git init`. 
Clonar un repositorio es la manera rápida y eficáz de descargar un proyecto de un servidor remoto a nuestra computadora para testearlo, ejecutarlo, modificarlo, etc.

`git clone [dirección url HTTPS ó SSH]` [generar la clave SSH](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ssh-https-conexion-github.md)

## Clonar un repositorio de Github

Copiamos la dirección HTTPS en este caso:

![alt](http://pandawebs.net/assets/images/clonar-un-repositorio.png)

> Para utilizar la dirección SSH debemos [generar la clave SSH](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ssh-https-conexion-github.md)

Abrimos la terminal, vamos al directorio donde queremos que se clone el repositorio y escribimos `git clone` seguido de la dirección que copiamos. HTTPS en este caso:

`git clone https://github.com/pandawebs/practicasGit.git`

Esto creará una carpeta con el nombre de practicasGit.
Esta incluirá toda la historia del proyecto. Es decir, una copia de todos los datos que tiene el servidor de ese repositorio con sus respectivos commits y sus versiones.

Si queremos que se clone con otro nombre de carpeta agregamos un espacio y el nuevo nombre.
Supongamos que en vez de llamarse "practicasGit" queremos que se llame "practicas-Git". Cuando vayamos a clonar escribimos:

`git clone https://github.com/pandawebs/practicasGit.git practicas-Git`

<br>
<br>

<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo en Github](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/clonar-un-repositorio.md " target="_blank)</em>

<!-- Fin links índice y github -->

<hr>

<br>

[siguiente - **Fork un repositorio**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/fork-un-repositorio.md) 

[anterior - **Git fetch - git pull**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/git-fetch-git-pull.md)