##Reset

_**Lo que hace reset es reiniciar Git en el punto o estado que indiquemos.**_

**Veremos:**

- git reset <br>

- git reset --soft <br>

- git reset --mixed <br>

- git reset --hard <br>

</div>

<br>

**git reset** (quitar archivos del staging area)

Luego de enviar modificaciones al [staging area o área de preparación](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md) con
el comando `git add` en alguna de sus variaciones, tales como
`git add -A` o `git add [Nombre de archivo]`. 

Es posible que nos arrepintamos y querramos volver atrás y quitarlas del "staging area". Lo podemos hacer con el comando:

`git reset HEAD`

Si solo queremos quitar un archivo determinado del "staging area" lo hacemos con el comando:

`git reset HEAD [nombre del archivo]`

<br>

**git reset --soft**

Borra el commit pero los datos del [directorio de trabajo (working directory)](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md)  y el
[área de preparación (staging area)](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md) no se tocan.

`git reset --soft [numero de commit anterior al que se quiere borrar]`

<br>

**git reset --mixed**

Borra el commit y los archivos del [staging area](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md) pero no toca los datos del [working directory (directorio de trabajo)](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md)

`git reset --mixed [numero de commit anterior al que se quiere borrar]`

<br>

**git reset --hard** 

Elimina todo de [los tres estados](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/flujo-de-trabajo-basico-con-git.md), del working area, del staging area y del area de confirmaciones(commit).
Hay que tener cuidado porque pueden llegar a ser irrecuperables.

`git reset --hard [numero de commit anterior al que se quiere borrar]`

<br>

[Revertir un `git reset --hard`](#)


<br>
<br>

<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/git-reset.md)</em>

<!-- Fin links índice y github -->

<hr>

<br>

[siguiente - **Github. Funcionamiento**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/funcionamiento-de-github.md) 

[anterior - **Ramas (branches)**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/trabajar-con-ramas-git.md)