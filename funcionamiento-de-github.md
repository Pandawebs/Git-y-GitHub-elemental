## Funcionamiento de GitHub. Conectar con nuestro repositorio local.

### GitHub

GitHub permite publicar proyectos con Git y nos ofrece herramientas 
para compartir, colaborar en proyectos y trabajar en equipo.

Hasta ahora hemos trabajado con un repositorio local donde todo ocurre en nuestra computadora.
GitHub permite que conectemos nuestro repositorio local a su red pública para mostrarlo al mundo y acceder a colaboradores y herramientas para poder desarrollar junto a un equipo de forma remota, segura y efectiva.

Siguiendo con el ejemplo que venimos trabajando, vamos a subir nuestro repositorio a GitHub.

1. Vamos a [GitHub](https://github.com)  y nos creamos una cuenta.

2. En la página de nuestro perfil vamos a Repositories > New

[![crear-repo.png](https://i.postimg.cc/mkMXZdsV/crear-repo.png)](https://postimg.cc/D4vdBPmb)

También podemos crearlo desde el signo "+" en el ángulo superior derecho junto a la foto de perfil.

[![crear-repo2.png](https://i.postimg.cc/85YB6LH3/crear-repo2.png)](https://postimg.cc/YG1WcGTf)



Una vez que clickeamos en "New" aparecerán los campos y opciones para crear nuestro nuevo repositorio remoto.
Ponemos un nombre. En este ejemplo lo llamaremos "practicasGit".
Luego podemos poner una descripción que es opcional.

Acción siguiente nos da la posibilidad de crear un README. Esto será útil si no tuvieramos creado un repositorio en local, es decir que primero lo creamos en GitHub para luego hacerle una copia como repositorio local. 
Como nosotros ya lo tenemos y lo que queremos es subirlo a GitHub, **no** marcamos el casillero que dice "Initialize this repository with a README".

De momento dejamos en "none" Add .gitignore y Add license.

Le damos a "Create repository"

Aparece una página con varias opciones que podemos utilizar como modelo para hacer la conexión y dar inicio al repositorio remoto.
Nosotros como queremos subir un repositorio existente haremos los pasos que nos muestra la opción que dice "…or push an existing repository from the command line"

En primer lugar elegimos y copiamos la dirección HTTPS.

[![github-https.png](https://i.postimg.cc/4N6m94Kf/github-https.png)](https://postimg.cc/8jCp8SB9)

> Para utilizar la dirección SSH debemos [generar la clave SSH](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ssh-https-conexion-github.md)

Utilizamos el comando `git remote add origin` seguido de la dirección que vayamos a utilizar. HTTPS en este caso:

`git remote add origin https://github.com/Pandawebs/practicasGit.git`

*Para verificar que los repositorios están conectados:*

`git remote -v`

Al ejecutar este comando debe aparecer dos veces la dirección https que utilizamos para hacer la conexión.
Esta dirección conectará los repositorios cuando se realice fetch y push.

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git remote -v
origin https://github.com/Pandawebs/practicasGit.git (fetch)
origin https://github.com/Pandawebs/practicasGit.git (push)
```

<br>

## Git push. 
**Subir - empujar un repositorio al servidor remoto(GitHub).**

Para ir subiendo las actualizaciones de nuestro proyecto a GitHub o a cualquier otro servidor remoto.

`git push [nombre-remoto][nombre-rama]`

En nuestro caso el comando será:

`git push origin master`

**origin** es el nombre predeterminado que le da Git al servidor remoto con el que se está trabajando.
**master** porque se refiere al nombre de la rama en la que estamos trabajando.

Realizar este comando implica haber hecho antes un commit, de lo contrario nos dará un error con aviso de que hay archivos que se han cambiado y no están siendo seguidos por Git.

No es necesario hacer el `push` después de cada commit. Cuando lo hagamos subirán todos, aunque se recomienda hacerlo en cada commit, sobre todo si se está trabajando en equipo.

En nuestro ejemplo aún se encuentra vacío el repositorio remoto que creamos en GitHub.

De todas maneras es buena práctica ejecutar primero el comando `git fetch`. En el caso que nos mostara información como la siguiente:
```console
 agustin@pandawebs-MacBook-Pro practicasGit $ git fetch
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
Unpacking objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
From github.com:Cursos-IT/CITweb1.0
 * [new branch]      master     -> origin/master
 ```
significa que en el repositorio remoto (Github) existen archivos que debemos traer a nuestro repositorio local, entonces ejecutaremos el comando `git pull origin master`.
Si no nos muestra nada luego de ejecutar `git fetch` continuamos con lo siguiente.

Vamos a la terminal y escribimos `git status` para asegurarnos de que no haya cambios por agregar a git.

```console
agustin@pandawebs-MacBook-Pro practicasGit $ git status
On branch master
nothing to commit, working directory clean
```
Si existieran cambios continuamos con los comandos `git add .` y `git commit -m "mensaje"`

Ahora enviamos el repositorio a Github:

Escribimos el comando `git push origin master`

Nos pedirá nombre de usuario y contraseña de GitHub.

Luego de autenticar, nuestro repositorio remoto pasará a tener los mismos archivos que el proyecto local con sus commits asentados en la sección de commits de GitHub.


Refrescamos nuestro GitHub y vemos nuestro README.md que creamos en nuestro repositorio local ya aparece junto con los commits correspondientes. 

[![commits-github.png](https://i.postimg.cc/yYvRpXKg/commits-github.png)](https://postimg.cc/GHT9HDHd)

## Relacionado:
[**SSH - HTTPS - conexión GitHub**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ssh-https-conexion-github.md)


<br>
<br>

<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/funcionamiento-de-github.md)</em>


<!-- Fin links índice y github -->
<hr>

<br>

[siguiente - **Git fetch - git pull**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/git-fetch-git-pull.md) 

[anterior - **Git reset**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/git-reset.md)