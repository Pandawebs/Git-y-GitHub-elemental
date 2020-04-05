## Ejemplo de flujo de trabajo con Git.

Luego de [crear una carpeta vacía (practicasGit) e iniciar Git](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/crear-un-repositorio.md), vamos a crear en ella un archivo donde escribiremos algo de información sobre el proyecto (nombre del proyecto, autor, etc). Este archivo lo llamaremos README.md y escribiremos la siguiente información:

```md
  ## Curso de Git y GitHub

  ### Autor

  * Agustín Palmieri
```

Este tipo de archivo con extensión **.md** está escrito en un lenguaje de marcado llamado [Markdown](https://guides.github.com/features/mastering-markdown/).
[Sintaxis Markdown](https://guides.github.com/features/mastering-markdown/)

> **README** es un archivo generalmente .txt o .md con información sobre el software.
El archivo README.md se imprime en la página principal del proyecto en Github. Es el primer lugar que los usuarios y potenciales colaboradores van a buscar información sobre tu proyecto. Como nombre, instalación, colaboradores, licencia etc. 
Es importante y por lo general es el primer archivo de nuestro proyecto.

<br>

### Git status (working directory)

Una vez creado escribiremos en la terminal, en la carpeta principal del proyecto:
`git status`

Este comando corrobora que Git hizo el seguimiento de la creación del archivo README.md 

En terminal:

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git status

On branch master
Initial commit

Untracked files:

(use "git add ..." to include in what will be committed)

README.md

nothing added to commit but untracked files present (use "git add" to track)
```

<br>

`git status` nos sirve para saber si hubo cambios en nuestro proyecto. Mostrará los nuevos archivos y/o los cambios realizados en archivos que hayan sido modificados.

### Git add (staging area)

Con el comando `git add .` registraremos todos los cambios. Se agregaran los nuevos archivos y/o los archivos que han sido editados.

`git add NombreArchivo.txt`. Agrega sólo el archivo que le indiquemos.

### Git commit(confirmación)

Con el comando `git commit -m "Creamos README.md"` confirmamos y enviamos todos los cambios al historial del repositorio. Junto con una descripción de los cambios realizados.

Repetiremos estos pasos cuando hayamos creado, editado y/o borrado un archivo y creamos
conveniente que Git guarde una versión hasta ese cambio.

**Nuevos cambios en el proyecto:**

Supongamos que agregamos información al archivo README.md de nuestro ejemplo.

Agregamos contacto y lo guardamos.

```md
  ## Curso de Git y GitHub

  ### Autor

  * Agustín Palmieri

  ## Contacto

  * email: agustinpfs[at]gmail[dot]com
```

Hacemos `git status`

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git status

(use "git add ..." to update what will be committed)

(use "git checkout -- ..." to discard changes in working directory)

modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
<br>


Vemos que nos indica que el archivo README.md ha sido modificado. **Aún este cambio no es seguido por Git**.

Agregamos los archivos que han sido editados al [staging area o área intermedia](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md).
`git add -A`

Ahora realizamos el commit.
`git commit -m "Agregamos contacto a README.md"`

## Git log

Ya tenemos dos versiones. Para ver una lista y descripción de las versiones de nuestro
proyecto escribimos `git log`

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git log

commit 57oc67af0e2d8d825a7c47b45c5adbea615170ed

Author: agustin 

Date: Mon Oct 24 19:09:54 2016 -0300

      Agregamos contacto a README.md

commit 57b46c2aaboc67af0e2d8c825a7c47ea915170fd

Author: agustin 

Date: Mon Oct 24 19:15:14 2016 -0300

      Creamos README.md
 ```

<br>
<br>


<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/ejemplo-de-flujo-de-trabajo-basico-con-git.md)</em>

<!-- Fin links índice y github -->



<hr>

<br>

[siguiente - **Ramas (branches)**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/trabajar-con-ramas-git.md) 

[anterior - **Flujo de trabajo básico con Git**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md) 
