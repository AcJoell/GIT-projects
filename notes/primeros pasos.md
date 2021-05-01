> GIT: Es un sistema de control de versiones, donde se guardan cambios dejando claro donde occurrieron, cuando ocurrieron, quien los hizo y volver a esa version pasada.
#
#
- - -
# CONFIGURANDO GIT POR PRIMERA VEZ
- - -

### NOTAS
> (-) usas letras (l, a)
> (--) usas palabras (global)

### COMANDOS
##### 1. Encontrar todas las configuraciones de git
#
#
```sh
git config || git config --list || git config --list --show --origin
```
- git config permite obtener y establecer variables de configuración
- --list para mostrar todas las propiedades que Git y tu han configurado
- --list --show --origin muestra la ubicacion de las configuraciones guardadas

##### 2. Configura tu nombre para que cualquier colaborador o tu lo puedan ver
#
#
```sh
git config --global user.name "Your Name" |or| user.email "user@example.com"
```
- user.name  "..." para establecer tu nombre de usuario
- user.email  "..." para establecer tu correo electronico

#
#

- - -
# CREANDO UN REPOSITORIO
- - -

### NOTA:
> ( GIT ADD . ) al ejecutarlo el archivo esta en estado STAGING
> ( GIT COMMIT -M "..." ) al ejecutarlo el archivo se va al repositorio local 

### COMANDOS:

##### 1. Crear repositorio local
#
#
```sh
git init
```
Crearas un repositorio en tu carpeta, es decir, una base de datos en donde se van a guardar los cambios de tus archivos, junto con una carpeta .git (carpeta oculta)

##### 2. Archivo en estado staging (area de preparacion)
#
#
```sh
git add name.txt || git add .
```
- git add agregar tu archivo dando un seguimiento a este (Staging)
- . agrega todos tus archivos nuevos o con algun cambio

##### 3. Eliminar archivo o deshacer git add .
#
#
```sh
git rm name.txt || git rm --cached name.txt
```
- git rm sirve para eliminar un archivo
- --cached significa que esta en RAM y podemos quitarle el seguimiento a nuestro archivo

#
#
- - -
# HACIENDO TU PRIMET COMMIT
- - -
### NOTA:
> si hiciste commit y alteraste un archivo que quieres guardar o hiciste otra accion tienes que repetir el proceso haciendo:
> git add .
> git commit -m "Newmessage"

### COMANDOS:

#### 1. Subiendo un commit
#
```sh
git commit -m "message"
```
Envia los ultimos cambios del archivo y un mensaje respectivo a la base de datos del sistemas de control de versiones.

#### 2. Diferenciando commits
#
```sh
git diff numLargoDelCommit1 numLargoDelCommit2 (indicador del commit)
```
Sirve para comparar los cambios hechos entre commits. El texto largo es el indicador del commit que se crea al subir un commit al repositorio.
#
- - -
# OTROS
- - -
### COMANDOS:
> CC
> SS
> AA

#### 1. Observar el estado de tu repositorio local
#
```sh
git status
```
Ver el status de la base de datos (repositorio local) asi como tus cambios añadidos

#### 2. Observar el estado de tus archivos completamente
#
```sh
git show name (optional)
```
Muestra el estado del directorio de trabajo y del área del entorno de ensayo
Permite ver:
- estado del directorio
- estado del entorno de ensayo
- cambios en Staging
- cambios sin seguimiento
- cuando se cambiaron
- quien las cambio

#### 3. Observar la historia de tus archivos, recorrido por commits
#
```sh
git log name
```
Ver la historia completa de un archivo. Muestra todos los commits y su informacion.

#### 4. Subir tu repositorio local a uno remoto
#
```sh
git push
```
- Permite enviar a un repositorio remoto (en linea) lo que estas haciendo localmente
- Permite traer una version de un commit o archivo de un repositorio remoto (en linea)