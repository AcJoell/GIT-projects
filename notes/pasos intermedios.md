_________________________________

<h1> INTRODUCCION A RAMAS </h1>
_________________________________

<h2>COMANDOS:</h2>

<h3>MASTER</h3>

<p>
MASTER es la rama por defecto
</p>

<h3>RAMA EXPERIMENTAL O DEVELOPMENT</h3>

<p>
Puedes hacer diferentes cambios sin perjudicar la rama por defecto MASTER
</p>

<h3>RAMA BUGFIXING O HOTFIX</h3>

<p>
Haces los cambios en esa rama y luego los pruabas con la rama actual (MASTER) esa conexion se le conoce como MERGE donde unes los cambios de una rama con otra.
</p>

_________________________________

<h1> VOLVER A UN COMMIT VIEJO </h1>
_________________________________

<h2>COMANDOS:</h2>

<h3>git commit -m "message"</h3>

<p>
Te envia el mensaje escrito dentro de las comillas a la hora de guardar los cambios en el repositorio remoto
</p>

<h3>git reset || git reset --hard  || git reset --soft</h3>

<p>
Nos permite volver a un commit anterior
--hard es el mas peligroso pero el que mas se usa
--soft volvemos a la version anterior, pero lo que tengamos en staying (add) sigue ahi para el proximo commit aunque vuelva a la version anterior
</p>

<h3>git diff</h3>

<p>
Nos muestra los cambios que no han sido agregados en el staying (add) todavia.
</p>

<h3>git diff</h3>

<p>
Nos muestra los cambios que no han sido agregados en el staying (add) todavia.
</p>

<h3>git log --stat</h3>

<p>
Nos muestra los cambios especificos segun los commits donde muestran la cantidad en tamaño y los archivos
</p>

<h3>git checkout 17191a03bfee2881c5f8 archivo.txt</h3>

<p>
Nos devuelve como era el archivo segun el commit que le pasamos
</p>
________________________________________________________

<p>
EJEMPLO 1: <br>

<em>Nos devuelve la version vieja del archivo segun el commit</em><br>

 git checkout 17191a03bfee2881c5f8128e8fb17b69a5b57e67 repo-test/blogpost.html<br>

<em>Nos muestra que solo se cambio ese archivo pero aun no esta en algun estado<br>

git status

<em>Nos devuelve ese archivo a la ultima version, la version master<br>

 git checkout master repo-test/blogpost.html

<em>Nos muestra que no debemos realizar ningun cambio, puesto que tenemos el archivo exactamente igual a como se hizo el ultimo commit<br>

git status

</p>

________________________________________________________

<p>
EJEMPLO 2: <br>

<em>Nos devuelve la version vieja del archivo segun el commit</em><br>

 git checkout 17191a03bfee2881c5f8128e8fb17b69a5b57e67 repo-test/blogpost.html<br>

<em>Nos muestra que solo se cambio ese archivo pero aun no esta en algun estado<br>

git status

<em>Agregamos nuevos cambios en el archivo del viejo commit y lo guardamos<br>

git add . and git commit -m "Reemplazo"

<em>Nos devuelve ese archivo a la ultima version, la version master<br>

 git checkout master repo-test/blogpost.html

<em>Nos muestra que no debemos realizar ningun cambio, puesto que tenemos el archivo exactamente igual a como se hizo el ultimo commit<br>

git status

</p>