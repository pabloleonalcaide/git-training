# Apuntes de GIT & GITHUB

## Comandos

* git branch -a => nos muestra las ramas ocultas

* git fetch origin => baja los cambios del repositorio remoto a la rama oculta origin/master.

* git checkout HASH => vuelve al commit indicado, creando una rama temporal en la que podemos experimentar. Si queremos mantener los cambios, deberíamos volcarlos en una nueva rama (git checkout -b NUEVARAMA).

* git reset HASH => vuelve al commit indicado, eliminando los commits que están por arriba.
	* git reset --soft => Elimina el commit pero no modifica el código.
	* git reset --hard => Elimina el commit y modifica el código.

* git commit --amend -m "descripcion" => corrige el commit previo modificando la descripcion indicada. Para subir ésta modificación a la rama remota, usamos git push con el comando '-f' (porque github interpreta que el commit es el mismo).

* git tag v1.0 => tags ligeras

* git tag -a v1.0 -m "mensaje" => tags anotadas (recomendada)

* git tag -a v1.0 -m "mensaje" HASH => aplica el tag al commit indicado

* git push origin v1.o => nos permite subir el tag indicado al repositorio remoto

* git push origin --tags => nos permite subir todos los tags de nuestro repositorio local

## Conceptos de interés

* ISSUES: Nos permiten crear notificaciones para identificar errores o mejoras en el código.

* MILESTONES: Son grupos que issues que se aplican para un proyecto, característica o periodo de tiempo (nos permiten agrupar issues).

* LABELS: Son un modo de organizar los diferentes problemas mediante 'etiquetas' (bugs, preguntas, duplicado...).

* TAGS: Puntos en la historia de neustro proyecto que se utilizan para asignar versiones.

