## Flujo de trabajo básico con Git (basic Git workflow)

Se compone de tres pasos y son la base para trabajar con Git.
Se las conoce también como los tres estados.

1. **Directorio de trabajo (working directory)**. Es donde trabajamos con nuestros archivos,
creándolos, modificándolos o borrándolos.

2. **Área intermedia o de preparación(index - staging area)**. Es un área donde se envían todos los cambios que se hicieron en el working directory y se encuentran listos para confirmarlos.
Al staging area se envían los cambios que afectarán el próximo commit. Se utiliza el comando `git add` seguido de algunas de sus variaciones, tales como:
`git add .`(envía todos los cambios) ó `git add [nombre de archivo]`(envía un archivo en particular).

3. **Confirmación (Git directory)**. Es la última versión del proyecto hasta el último commit.
Se crea cuando hacemos un commit usando el comando `git commit -m "Descripción de los cambios"`
Con este último paso se crea una versión hasta esos cambios de manera permanente con la descripción que le hayamos puesto.

Repetiremos los pasos luego de volver a editar el proyecto y creamos conveniente que Git guarde una versión hasta esos cambios.

> Para ver una lista y descripción de las versiones de nuestro proyecto escribimos `git log`

<br>
<br>

<!-- Inicio links índice y github -->

<span class="link-to-index-git">Git & Github elemental [ver índice](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/README.md)</span>

<em>[Editar este artículo](https://github.com/Pandawebs/Git-y-GitHub-elemental/edit/master/flujo-de-trabajo-basico-con-git.md)</em>





<!-- Fin links índice y github -->

<hr>

<br>

[siguiente - **Ejemplo de flujo de trabajo con Git**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/ejemplo-de-flujo-de-trabajo-basico-con-git.md) 

[anterior - **Cómo crear un repositorio**](https://github.com/Pandawebs/Git-y-GitHub-elemental/blob/master/crear-un-repositorio.md) 


