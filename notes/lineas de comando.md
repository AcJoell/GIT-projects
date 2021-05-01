- - -
# CODIGOS DE LA LINEA DE COMANDO
- - -

### COMANDOS
##### 1. Ubicandote en tu pc
#
```sh
pwd
```
Te mostrara en que carpeta estas en tu pc ahora mismo
#
##### 2. Navegando por tu pc I
#
```sh
cd || cd . || cd .. || cd ../../
```
`Son DOS puntos SIN espacios`
- cd : Navegar por la linea de comando
- cd . Es la carpeta actual (no te lleva a ningun lado)
- cd . . Te devuelve una carpeta
- cd . ./. ./ Te devuelve dos carpetas

#
##### 2. Navegando por tu pc II
#

```sh
cd name || cd (letra) || cd / || cd /c
```
- cd name : Entrar a una nueva carpeta
- cd u : Te muestra los archivos y carpetas que comienzan por u (o cualquier letra)
- cd / : Te lleva al home
- cd /c : Sirve para acceder a otro disco duro

#

##### 3. Creando una carpeta
#
#
```sh
mkdir name
```
Sirve para crear una carpeta

#
#### 4. Creando un archivo
#
```sh
touch name.txt
```
Sirve para crear un archivo vacio

#
##### 5. Listando archivos
#
```sh
ls || ls -al || ls -l  || ls -a
```
- ls : Sirve para listar los archivos que tenemos en ese momento
- -a : Muestra los archivos ocultos listados
- -l : Muestra los archivos visibles listados
- -al : Muestra todos los archivos incluso los ocultos

#
##### 6. Limpiando tu consola
#

```sh
clear || Ctrl + l
```
Deja limpia tu consola

#
#### 7. Viendo el contenido de un archivo
#
```sh
cat name.txt
```
Te muestra el contenido de un archivo

#
#### 8. Historial de comandos
#
```sh
history
```
Ver historia completa de todos los comandos hechos por consola

#### 9. Eliminando un archivo
#
`ESCRIBIR BIEN EL CODIGO O PUEDE LLEGAR A ELIMINAR EL DISCO DURO`
```sh
rm name.txt || rm --help
```
- rm name.txt : Sirve para borrar un archivo
- --help : Te muestra como funcionan todos los comandos (en este caso rm)