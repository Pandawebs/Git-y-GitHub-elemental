#Instalación y configuración de Git

##Instalar Git

Descargar Git desde [https://git-scm.com/downloads](https://git-scm.com/downloads " target="_blank) y seguir las instrucciones de instalación.

Una vez instalado, abrir la terminal y verificar la instalación. Escribir:

`git --version`

Si Git se instaló correctamente, la terminal mostrará la versión de Git instalada.

Ejemplo: `git version 2.6.0`

En terminal:

```console
agustin@pandawebs-MacBook-Pro ~ $ git --version

git version 2.6.0
```

<hr>

##Configurar Git

**Configuración de nombre y email para Git**

*Configuraremos nuestro nombre y email para asociar los cambios del repositorio(commits) a una identidad.*

<br>

###Configurar nombre:

a)**Configurar nombre de manera GLOBAL:**

Utilizará por defecto el mismo nombre para todos los repositorios que vayas a crear en tu computadora. 

`git config --global user.name "Agustin"` 

De ésta manera cada repositorio creado en cualquier directorio se le asignará este nombre.



**En terminal(cualquier directorio):**

`agustin@pandawebs-MacBook-Pro $ git config --global user.name "Agustin"`

<br>

> Esta configuración global es la mas común ya que por lo general, los repositorios locales son del único dueño de la computadora.

<br>

b)**Configurar nombre de manera ÚNICA:** Para un repositorio en particular.

`git config user.name "Agustin"` 


En terminal. En el directorio raíz del proyecto("git-curso" en este ejemplo):

`agustin@pandawebs-MacBook-Pro git-curso $ git config user.name "Agustin"`

<br>

> Podemos utilizar el comando anterior (único), aunque ya tengamos definido un usuario global. El nuevo nombre sobreescribirá el nombre definido globalmente en ese repositorio.

<br>

**Para ver el nombre de usuario de un repositorio Git.**

`git config user.name`

En terminal:

```console
agustin@pandawebs-MacBook-Pro ~ $ git config user.name

agustin
```

<br>

**Para cambiar el nombre de usuario en un repositorio Git** simplemente lo volvemos 
a crear y esta acción sbreescribirá el nombre anterior.

**Global:** `git config --global user.name [Otro Nombre]`

**Único:** `git config user.name [Otro Nombre]`

<br>

###Configurar email:

**Global**: `git config --global user.email "agustin@example.com"`

**Único**: `git config user.email "agustin@example.com"`

<br>

**Para ver el email de usuario de un repositorio Git.**

`git config user.email`

```console
agustin@pandawebs-MacBook-Pro ~ $ git config user.email

agustin@example.com
```

<br>

**Para cambiar el email de usuario en un repositorio Git** simplemente lo volvemos 
a crear y esta acción sbreescribirá el email anterior.

**Para ver todos los detalles de la configuración**

`git config --list`

<br>
<br>



<!-- Inicio links índice y github -->


<span class="link-to-index-git">Git & Github elemental [ ver índice](http://pandawebs.net/git-github-elemental/)</span>
<em>[Editar este artículo.](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/instalacion-y-configuracion-de-git.md " target="_blank)</em>


<!-- Fin links índice y github -->


<hr>

[siguiente - **¿Cómo crear un repositorio?**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/crear-un-repositorio.md) 

[anterior - **Git. Concepto - repositorios**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/git-concepto-repositorios.md) 