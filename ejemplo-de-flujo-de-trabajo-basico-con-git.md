##Ejemplo de flujo de trabajo con Git.

Luego de crear una carpeta vacía e [iniciar Git](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/crear-un-repositorio.md), vamos a crear el archivo README.md con algo de información(nombre del proyecto, autor, etc) que podremos ir editando y ampliando a lo largo del proyecto.

Archivo .md escrito en [markdown](#):

```md
  ## Curso de Git y GitHub

  ### Autor

  * Agustín Palmieri
```
Archivo .md escrito en [markdown](#):

> **README** es un archivo generalmente .txt o .md(.md es la extensión de un archivo [markdown](#)). 
Un archivo README.md se utiliza comunmente para que se imprima en la página principal del proyecto en Github). Es el primer lugar que los usuarios potenciales y colaboradores van a buscar información sobre tu proyecto. Como nombre, instalación, colaboradores, licencia etc. 
Es importante y por lo general es el primer archivo de nuestro proyecto.

###Git status

Una vez creado escribiremos en la terminal, en la carpeta principal del proyecto:
`git status`

Este comando corrobora que Git hizo el seguimiento de la creación del archivo README.md 

En terminal:

```console
agustin@pandawebs-MacBook-Pro git-curso $ git status

On branch master
Initial commit

Untracked files:

(use "git add ..." to include in what will be committed)

README.md

nothing added to commit but untracked files present (use "git add" to track)
```

<br>

`git status` nos sirve para saber si hubo cambios en nuestro proyecto. Mostrará los nuevos archivos y/o los cambios realizados en archivos que hayan sido modificados.

###Git add

Con el comando `git add -A` registraremos todos los cambios. Se agregaran los nuevos archivos y/o los archivos que han sido editados.

Otras opciones comunes para `git add`:

`git add NombreArchivo.txt`. Agrega sólo el archivo que le indiquemos.
`git add .` agrega todos los archivos que se hayan modificado(no creados).

###Git commit

Con el comando `git commit -m "Creamos README.md"` confirmamos y enviamos todos los cambios al historial del repositorio.

Repetiremos los pasos cuando hayamos creado, editado y/o borrado un archivo y creamos
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
agustin@pandawebs-MacBook-Pro git-curso $ git status

(use "git add ..." to update what will be committed)

(use "git checkout -- ..." to discard changes in working directory)

modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
<br>


Vemos que nos indica que el archivo README.md ha sido modificado. **Aún este cambio no es seguido por Git**.

Agregamos los archivos que han sido editados al [staging area o área intermedia](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md).

Veamos 2 ejemplos comunes de comandos para agrgar archivos al staging area:

`git add README.md` (Agrega el archivo especificado)
ó
`git add -A` (Agrega todos los archivos que han sido editados o creados)

Ahora realizamos el commit.

`git commit -m "Agregamos contacto a README.md"`

##Git log

Ya tenemos dos versiones. Para ver una lista y descripción de las versiones de nuestro
proyecto escribimos `git log`

```console
agustin@pandawebs-MacBook-Pro git-curso $ git log

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
