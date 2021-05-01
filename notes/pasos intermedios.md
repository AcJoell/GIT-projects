- - -
# INTRODUCCION A RAMAS
- - -
### COMANDOS:

#### 1.  RAMAS
#
```sh
MASTER
```
MASTER es la rama por defecto.
#
```sh
EXPERIMENTAL O DEVELOPMENT
```
Puedes hacer diferentes cambios sin perjudicar la rama por defecto (MASTER)

```sh
BUGFIXING O HOTFIX
```
Haces los cambios en esa rama y luego los pruebas con la rama actual (MASTER) esa conexion se le conoce como MERGE donde unes los cambios de una rama con otra.

- - -
# VOLVER A UN COMMIT VIEJO
- - -

### Nota
> Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).


### COMANDOS
##### 1. Volviendo a commit anterior
#
```sh
git reset || git reset --hard  || git reset --soft
```
Nos permite volver a un commit anterior
- --hard es el mas peligroso pero el que mas se usa
- --soft volvemos a la version anterior, pero lo que tengamos en staging (add) sigue ahi para el proximo commit aunque vuelva a la version anterior

#
##### 2. Diferenciando versiones (commit)
#
```sh
git diff
```
Nos muestra los cambios que no han sido agregados en el staging (add) todavia.

#
##### 3. Mostrando cambios especificos de commits
#

```sh
git log --stat
```
Nos muestra los cambios especificos segun los commits donde muestran la cantidad en tamaño y los archivos

#
##### 4. Volviendo a una version anterior
#
```sh
git checkout 17191a03bfee2881c5f8 archivo.txt
```
Nos devuelve como era el archivo segun el commit que le pasamos

#
#### 5. Eliminando archivos I
#
```sh
git rm || git rm --cached || git rm --force
```
Este comando nos ayuda a eliminar archivos de Git sin eliminar su historial del sistema de versiones. Podemos viajar en el tiempo para recuperar el ultimo commit.

- git rm --cached: Elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro.

- git rm --force: Elimina los archivos de Git y del disco duro.

#
##### 6. Eliminando archivos II `(ES MUY PELIGROSO)`
#
```sh
git reset || git reset --soft || git reset --hard || git reset HEAD
```
Nos ayuda a volver en el tiempo sin la posibilidad de volver al futuro, borramos la historia y no hay vuelta atras.

- git reset --soft: Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging, así podemos aplicar las últimas actualizaciones a un nuevo commit.

- git reset --hard: Borra todo, toda la información de los commits y del área de staging se borra del historial. (forever)

- git reset HEAD: Este es el comando para sacar archivos del área de Staging. No para borrarlos ni nada de eso, solo para que los últimos cambios de estos archivos no se envíen al último commit, a menos que cambiemos de opinión y los incluyamos de nuevo en staging con git add, por supuesto.