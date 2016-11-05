#Fork un repositorio.

**Fork copia cualquier repositorio público de Github a nuestra cuenta. Éste se agregará a nuestra lista de repositorios.**

Fork nos permite trabajar sobre cualquier repositorio público de Github, sin afectar el original.

![alt](http://pandawebs.net/assets/images/fork-git.png)


La **diferencia entre fork y clone** es que fork es una copia de un repositorio remoto a otro remoto, y [clone](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/clonar-un-repositorio.md) es una copia de un repositorio remoto a nuestra computadora.

Fork nos permite editar cualquier proyecto con las herramientas de colaboración que nos ofrece GitHub. Por ejemplo trabajar remotamente con miembros de nuestro equipo sobre cualquier proyecto público o proponer cambios a los repositorios originales haciendo [pull requests](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/pull-request.md).


###Mantener actualizado nuestro repositorio fork con el original(upstream).

`upstream` es el nombre que se le da al repositorio original a la hora de hacer la conexión.

>Una conexión con `upstream` permite descargar los cambios efectuados en el repositorio original pero no permite cargar datos. Nuestros cambios los cargaremos a nuestro fork del proyecto. Luego se pueden proponer al original con un [pull requests](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/pull-request.md).

<br>

**Ejemplo práctico:**

Primero haces un fork del repositorio de nuestro ejemplo dándole al botón "fork".

![alt](http://pandawebs.net/assets/images/fork-git.png)

Luego lo [clonas](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/clonar-un-repositorio.md) en tu computadora:
<small>En este ejemplo usamos HTTPS como conexión. Para usar SSH [genera la clave](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ssh-https-conexion-github.md).</small>


`git clone https://github.com/tuNombreUsuario/practicasGit.git`

Lo conectas con tu repositorio "fork"

`git remote add origin https://github.com/tuNombreUsuario/practicasGit.git`

Ahora lo conectas con el original:

`git remote add upstream https://github.com/Pandawebs/practicasGit.git`

Verificamos si se ha guardado las conexiones `origin` y `upstream`:

`git remote -v`

```console
tuNombreUsuario@example-MacBook-Pro practicasGit $ git remote -v
origin https://github.com/tuNombreUsuario/practicasGit.git (fetch)
origin https://github.com/tuNombreUsuario/practicasGit.git (push)
upstream https://github.com/Pandawebs/practicasGit.git (fetch)
upstream https://github.com/Pandawebs/practicasGit.git (push)
```

Ahora comprobamos si ha habido cambios en el repo original y los traemos a nuestro local.

`git fetch upstream`

También podemos ver si ha habido cambios desde Github

![alt](http://pandawebs.net/assets/images/cambios-fork-original.png)



Hacemos un merge. Esto fusionará los cambios del repositorio original con nuestro repositorio local.

`git merge upstream/master`


Ahora podemos actualizar el fork de nuestra cuenta de GitHub:

`git push origin master`

Si vamos a Github y refrescamos podremos ver que se ha actualizado nuestro repositorio.

>Si queremos mantener actualizado nuestro fork con el original, los cambios o evolución por nuestra parte los debemos hacer en distintas ramas para evitar conflictos.

<br>
<br>

<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo en Github](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/fork-un-repositorio.md " target="_blank)</em>

<!-- Fin links índice y github -->

<hr>

<br>

[siguiente - **Pull request**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/pull-request.md) 

[anterior - **Git clone. Clonar un repositorio.**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/clonar-un-repositorio.md)