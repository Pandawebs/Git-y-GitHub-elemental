##¿Cómo crear un repositorio?


Después de [instalar Git en nuestra computadora](http://pandawebs.net/instalacion-y-configuracion-de-git/ " target="_blank) ya podremos iniciar Git en cualquier carpeta para que ésta se convierta en un repositorio.

Para iniciar Git. En la terminal, ir a la carpeta del proyecto(practicasGit) y escribir:

`git init`

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git init

Initialized empty Git repository in /Users/agustinpfs/practicasGit/.git/
```

"Initialized empty Git repository" nos dice que ya tenemos un repositorio Git.


Lo que hace`git init` es crear un archivo .git que guardará las versiones del proyecto en los puntos que le indiquemos mientras se producen cambios en los archivos.


Para corroborar que realmente se ha creado el repositorio, tipeamos en la terminal:
`git status`

Si **no** devuelve algo como esto: `'fatal: Not a git repository...'`, está todo bien.
El repositorio ha sido creado.

> Esto funciona para cualquier proyecto por más que esté avanzado en el desarrollo.
A partir de que iniciamos Git ya se podran ir creando y controlando versiones.

[Crear un repositorio en GitHub](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/funcionamiento-de-github.md)

<br>
<br>

<!-- Inicio links índice y github -->


<span class="link-to-index-git">Git & Github elemental [ ver índice](http://pandawebs.net/git-github-elemental/)</span>

<em>[Editar este artículo](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/crear-un-repositorio.md)</em>




<!-- Fin links índice y github -->

<hr>


<br>

[siguiente - **Flujo de trabajo básico con Git**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md) 

[anterior - **Instalación y configuración**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/instalacion-y-configuracion-de-git.md) 
